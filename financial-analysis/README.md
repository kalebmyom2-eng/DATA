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

Incoming transfers are not necessarily earned income, and outgoing transfers are not necessarily consumption. Self-transfer and savings-transfer detection uses description rules and requires manual review. Early exploratory credit totals include movements that later sections attempt to filter. Missing-value and debit/credit conventions depend on the statement format. This notebook is exploratory work, not a validated financial reporting system or investment strategy.

Keep your workbook, exports, and executed notebook outputs private. Clear outputs before publishing a rerun.
