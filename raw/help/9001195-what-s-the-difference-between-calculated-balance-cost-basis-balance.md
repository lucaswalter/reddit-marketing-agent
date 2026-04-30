[Skip to main content](https://help.coinledger.io/en/articles/9001195-what-s-the-difference-between-calculated-balance-cost-basis-balance#main-content)

# What's the difference between Calculated Balance & Cost Basis Balance?

Learn how CoinLedger's Portfolio Tracker calculates these two values

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 4 months ago

CoinLedger’s Portfolio Tracker tracks the amount, price, market value, cost basis, percentage change, and unrealized return of the cryptocurrencies held across all of your imported wallets. It draws its information from the transaction data that _you have imported_. This means that if you do not import all of your historical transactions into the system, your tracked balances may not look correct.

One essential tool to troubleshooting your account balances is the Asset Balance Report. **[The Asset Balance Report](https://app.coinledger.io/individual/asset-balance-report)** allows you to view each of the transactions that CoinLedger uses to calculate your balances. To locate the Asset Balance Report, click on the [direct link](https://app.coinledger.io/individual/asset-balance-report) to it in the top right of your Portfolio Tracking page.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338558911/408d9557775a96982bc709663254/Screenshot%2B2025-01-16%2Bat%2B12_23_23-E2-80-AFPM.png?expires=1776713400&signature=caa36c541b2ca759dd1dcd63e986de94ecef9b3fc5065eaaf91b0a2975ea0e4a&req=dSMkHsx7lYheWPMW1HO4zdqHo1c5GfEA8K%2BucJk8Q%2BCwh%2BKgF6soxKZmXgUy%0AWMT%2FxrYGWAjFStC3CRY%3D%0A)

On the Asset Balance Report, you'll notice two fields: **Calculated Asset Balance** and **Asset with known cost basis**. Below, we'll breakdown what each of these fields mean and how they can help you troubleshoot your balances.

This report is particularly useful for distinguishing between balances serving portfolio tracking purposes and those used for tax reporting.

![](https://downloads.intercomcdn.com/i/o/974765421/76d451ceb02a64ef887bbbaa/CoinLedger-Review-Asset-Balances.png?expires=1776713400&signature=355d1757d4bdab6051ab19e7e8fb67abef7b08ec180505389211c9a312e452cc&req=fScjEc97mYNeFb4f3HP0gAKPbKV9OE0nqIv4lkb3TB2KSr7E%2BC2jLZSgGaNe%0AucyynaMM16WFqS%2BOlw%3D%3D%0A)

## What is Calculated Asset Balance?

**Calculated Asset Balance** is the total amount of a crypto asset we detect in your account across all your wallets (based on your imported transaction data).

Moreover, this balance is not utilized for direct tax calculations, serving instead as an overview of your total cryptocurrency holdings across your wallets.

CoinLedger breaks down Calculated Asset Balance into two types: **global** and **wallet-specific balances.** Your Calculated Asset Balance (Global) is the amount of a crypto asset you hold across all wallets on your CoinLedger account, while your wallet-specific Asset Balance is the amount of an asset held in just that particular wallet.

![](https://downloads.intercomcdn.com/i/o/974769413/5a0d2ea085e1e8f33a9ef468/image.png?expires=1776713400&signature=ac054dd76b9e8ee59d40b07c2b41ea80aabdefe8aee7ece149e08114520bc0b7&req=fScjEc93mYBcFb4f3HP0gPvUnxqNus73MOTUoTBkb8KosN5yw5hcfWaOy6To%0A4U%2ByYn%2Bmt4cs41LQEg%3D%3D%0A)

For example, if I have 5 BTC in my Ledger wallet and 2 BTC in my Coinbase wallet, my total Calculated Asset Balance (Global) would be 7 BTC, while my _wallet-specific balances_ for BTC would be the following:

- Calculated BTC Balance (Ledger): 5 BTC

- Calculated BTC Balance (Coinbase): 2 BTC


## What is Asset with known cost basis?

**Asset with known cost basis** is the current balance of a crypto asset in your CoinLedger account with known cost basis information (based on your imported transaction data).

[Cost basis](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning#h_b3f1286066:~:text=calculating%20your%20taxes.-,What%20is%20Cost%20Basis%3F,-Costs%20basis%20represents) represents the original value of an asset for tax purposes. It is used to determine your capital gains/losses incurred whenever you dispose of your crypto, and is vitally important to making sure your crypto transaction history is accurate.

For each asset on your account's Asset Balance Report, you'll see an **Asset with known cost basis** breakdown (shown below). This value simply represents the amount of an asset with a known cost basis based on your imported transactions.

![](https://downloads.intercomcdn.com/i/o/974780472/7b97a184f312f78373273c30/image.png?expires=1776713400&signature=3f64270eacf9c5c38da935e23e0aff1c703ec08fdf99b7cc5ebe140be82c176a&req=fScjEcF%2BmYZdFb4f3HP0gDCxoxVNNX4TPXDtdj4dGkvrH93pNwd6hX8sM50u%0AyD%2BWAunOW7tbVE0p1w%3D%3D%0A)

**This value may not always match your Calculated Asset Balances.** When calculated balance and cost basis balance do not match, this is a signal that there may be discrepancies or incomplete imported data.

# Cost Basis Tracking Methods

CoinLedger employs different cost basis tracking methods to keep up with regulatory tax requirements:

- **Universal Cost Basis Tracking:** This was used for tax filings in earlier years (2024 and prior years), allowing the cost basis to be calculated across all wallets.

- **Per-Wallet Cost Basis Tracking:** Implemented in alignment with updated IRS regulations (starting in January 2025), this method calculates gains and losses for each wallet independently.


These methods ensure accurate and regulation-compliant financial reporting.

Consider the following transaction history as an example:

1. Scott buys 1 BTC in Coinbase.

2. He withdraws 0.5 BTC to his Ledger Wallet.

3. Scott then buys another 1 BTC on Coinbase.


With this transaction history, Scott is missing a Deposit transaction to his Ledger Wallet. He has only imported the 0.5 withdrawal from Coinbase, but there should be a corresponding 0.5 deposit to his Ledger wallet.

Based on the above, CoinLedger is going to calculate BTC with known cost basis balance of 2 BTC. The Calculated Balance for his Coinbase wallet as well as the Calculated Balance for his Global wallet will be 1.5 BTC.

This balance discrepancy between calculated balance and cost basis balance exists due to missing data.

​

If Scott adds in the 0.5 deposit transaction to his Ledger into CoinLedger, his global calculated balance would be 2 BTC, which would match his known cost basis balance.

## Withdrawals and Deposits are treated as self-wallet transfers by default

CoinLedger treats Deposit & Withdrawal transactions as self-wallet transfers by default. This means the software assumes a withdrawal or deposit is you sending crypto to another wallet you have possession over.

Thus, these transaction do not alter your Known Cost Basis Balance because they are assumed to not be taxable events.

If your deposit or withdrawal **was** actually a taxable event, i.e. a payment, gift, or income event, you need to classify it as such. Classifying your deposits & withdrawals into their true transaction type will ensure that your Known Cost Basis balance is getting updated correctly.

## **Conclusion**

CoinLedger's Portfolio Tracker calculates it's asset balances based on the transaction data that _you have imported_. Your tracked balances may not look correct if your transaction history is not up to date. We recommend taking advantage of the [Asset Balance Report](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#:~:text=Why%20are%20my%20asset%20balances%20incorrect%3F) to make sure that all of your calculated balances, including your cost basis balance, are correct.

_Still need further assistance?_ Reach out to our Support Team at anytime at [help@coinledger.io](mailto:help@coinledger.io)!!

​

Did this answer your question?

😞😐😃