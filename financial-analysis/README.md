# Personal Financial Transaction Analysis

A Python notebook for cleaning wallet and savings transactions and exploring monthly inflows, spending, internal transfers, and cash-flow patterns using pandas and Matplotlib.

## What is included

The original analysis code, with personal identifiers replaced and all saved outputs removed. This is a code-only portfolio version; no real transaction records, balances, charts, or account statements are published. It has been checked for Python syntax but has not been rerun in this publication step. No financial results are claimed here.

## Run locally

1. Install dependencies: `python3 -m pip install -r requirements.txt`.
2. Place your own compatible workbook at `data/transactions.xlsx` relative to this folder.
3. The workbook must contain `Wallet Account Transactions` and `Savings Account Transactions` sheets, with the table header on Excel row 7. Expected columns include `Trans. Date`, `Value Date`, `Description`, `Debit(₦)`, `Credit(₦)`, `Balance After(₦)`, `Channel`, and `Transaction Reference`.
4. Replace `YOUR ACCOUNT NAME` in the notebook with the account-holder name used in your workbook before running locally.
5. Launch Jupyter from this folder and run the notebook in order. Cleaned exports go to `outputs/`.

## Interpretation and limitations

The analysis describes transaction activity in the supplied wallet and savings statements. Incoming transfers do not necessarily represent earned income, and outgoing transfers do not necessarily represent spending: transfers between an account holder's own accounts can appear on both sides.

- **Classification requires review.** Self-transfers and savings transfers are identified using rules based on transaction descriptions. Incomplete or ambiguous descriptions can lead to incorrect classifications.
- **Totals depend on the analysis stage.** Early exploratory credit totals include account movements that later sections attempt to filter. These totals should not be interpreted as confirmed income or compared with filtered summaries without accounting for that difference.
- **Statement formats affect the results.** Missing values and debit/credit conventions depend on the source workbook. The cleaning assumptions may need adjustment for statements from other providers.
- **The public version demonstrates the method.** Personal identifiers have been replaced and saved outputs removed. Real transaction records, balances and account statements are not included, so this repository does not present financial findings that readers can independently verify.

This notebook is an exploratory portfolio project, not a validated financial reporting system or an investment strategy.
