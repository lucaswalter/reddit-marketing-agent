[Skip to main content](https://help.coinledger.io/en/articles/10302709-how-are-cost-basis-numbers-in-the-portfolio-tracker-calculated#main-content)

# How are cost basis numbers in the Portfolio Tracker calculated?

Learn how CoinLedger calculates the cost basis of your assets.

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over a year ago

Within the Portfolio Tracker tab, there are two separate cost basis fields displayed:

1. Total cost basis

2. Cost basis per coin


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1303504110/b22580781ff7bee31b0c0db56583/AD_4nXdIfUGPxtILyc6L007H18eXHsS3Skvr8BpvGuqvif5v1DID4nSZDF0LnPGJ405Gb0NXDrNbbzTe2h_lLZPZrdyTJK_F08PXCu62bo8NtBR41QLOCF4PWBrlHl4N_MCZeJkJzYvB?expires=1776713400&signature=ab30a4a38b9fd1a17e037bf3bf0d3b158c21fbcb013f8f4b39364fdf761d4aed&req=dSMnFcx%2BmYBeWfMW1HO4zaGVgRSFmImdeSoXySUgPF7LcEHrytH8fh1gNJY5%0AjiGR1ZyxofVSjfTM6xA%3D%0A)

Additionally, within the hover text displayed while hovering over a specific cost basis field, two additional numbers are displayed:

1. Calculated {Coin} balance

2. {Coin} with known cost basis


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1303504460/d36a925c307c3c93466adff29d0f/Screenshot+2024-12-18+at+3_11_14%E2%80%AFPM.png?expires=1776713400&signature=f18ef9a444df4ca16f05e1ed8e9413dfbdc2a124895f5def1cbfc0bd4c1cc7ac&req=dSMnFcx%2BmYVZWfMW1HO4zds5Lf02nD1%2BEMScTKbnHXIrKgMfvtARKbBnZhcn%0ARhVxKjeMcH7KbxkZLx8%3D%0A)

Let’s drill into how these numbers get calculated.

## Total cost basis

Total cost basis (the bolded number on the left in the first image above) represents the total costs incurred to acquire the amount of assets held in your portfolio.

In the picture above, the total cost basis for this user’s BTC holdings is **$22,339.12**.

**Example of total cost basis:**

Let’s say I have the following transaction history:

- Buy 1 BTC for $60,000

- Trade 1 ETH ($4,000) for 0.1 BTC

- Sell 0.15 BTC


What is the total cost basis for my BTC?

In this example, I am currently holding 0.95 BTC (1 + 0.1 - 0.15). Summing up this taxable activity, we can see that my total costs incurred to acquire this 0.95 BTC were: $60,000 for 1 BTC, $4,000 for an additional 0.1 BTC, and then we have to remove the cost basis for the 0.15 BTC that we sold. If we are using the [First in, First out](https://coinledger.io/blog/cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained) calculation method (FIFO), this would give a cost basis of $9,000 (0.15 \* 60,000) for the 0.15 BTC we sold. We thus need to subtract $9,000 from $64,000 to arrive at a total outstanding cost basis of **$55,000**.

## Cost basis per coin

Cost basis per coin represents your total cost basis divided by the amount of the asset with known cost basis or _{Coin} with known cost basis_.

In the picture above, the cost basis per BTC for this user’s BTC holdings is **$20,884.74**.

This concept can get slightly more confusing, but for now, let’s look at a simple example calculation.

**Example of cost basis per coin:**

Let’s say I again have the following transaction history:

- Buy 1 BTC for $60,000

- Trade 1 ETH ($4,000) for 0.1 BTC

- Sell 0.15 BTC


In this example, my total cost basis is **$55,000**(using [FIFO](https://coinledger.io/blog/cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained)). My total BTC with known cost basis is 0.95 BTC (1 + 0.1 - 0.15). This gives me a cost basis per coin of **$57,894.74 per BTC** (55,000 / 0.95).

This cost basis per coin metric gives me a quick sense of how my holdings are performing relative to the current spot price of BTC. In this example, if BTC is trading above $57,894.74, I know I am in the green and am sitting on unrealized gains. If BTC is trading below $57,894.74, I’m in the red sitting on unrealized losses.

## Calculated {Coin} Balance

Calculated {Coin} Balance is the sum of all debits and credits, or all inflows and outflows of a coin, across your wallet(s).

In the second picture above, the calculated ETH balance for this user was **34.95781133.**

**Example of calculated {coin} balance:**

Let’s say I have the following transaction history:

- Buy 1 ETH for $2,000

- Deposit 2.5 ETH

- Buy 2 ETH for $6,000

- Withdraw 1 ETH


To calculate ETH balance in this wallet, we simply sum the inflows and outflows to arrive at a calculated balance of **4.5 ETH** (1 + 2.5 + 2 - 1). Buying and depositing ETH adds to your balance, while withdrawing or transferring out ETH deducts from your balance.

## {Coin} with known cost basis

{Coin} with known cost basis is a global calculation for the total amount of {Coin} across all of your wallets that have known cost basis.

Transactions that have an effect on your cost basis (i.e. taxable disposals, purchases, trades, income events, and gifts) are included in your {Coin} with known cost basis calculation. Transactions that do not impact your cost basis (i.e. deposits, withdrawals, and uncategorized transactions) are not included in your {Coin} with known cost basis calculation.

In the picture above, the ETH with known cost basis for this user was **53.24600475 ETH**.

**Example of {Coin} with known cost basis calculation:**

Let’s say I again have the following transaction history:

- Buy 1 ETH for $2,000

- Deposit 2.5 ETH

- Buy 2 ETH for $6,000

- Withdraw 1 ETH


In this example, our ETH with known cost basis is **3 ETH**. The only transactions in the above transaction history that are altering this user’s total cost basis calculations are the two purchases of ETH (1 for $2,000 and 2 for $6,000). Thus, we have **3 ETH** with known cost basis of $8,000.

Deposits and withdrawals are considered self-wallet transfers by default within CoinLedger. Thus, they are not cost basis altering transactions, and they do not impact this calculation.

## Why do my Calculated {Coin} Balance and {Coin} with known Cost Basis differ?

When **{Coin} with Known Cost Basis** varies drastically from your **Calculated {Coin} Balance**, it’s an indicator that there is incomplete data or improperly classified data in your CoinLedger account.

**Example of differing cost basis vs calculated balance:**

Let’s say I again have the following transaction history:

- Buy 1 ETH for $2,000

- Deposit 2.5 ETH

- Buy 2 ETH for $6,000

- Withdraw 1 ETH


My ETH with known cost basis is **3 ETH**; however, my calculated ETH balance is **4.5 ETH**. This difference is occurring because I have not imported or [classified data](https://help.coinledger.io/en/articles/5915504-when-do-i-need-to-manually-classify-my-crypto-transactions) which would otherwise tell CoinLedger what my cost basis is for the additional 1.5 ETH that I am holding in this wallet.

To further explore this discrepancy, we could ask questions like, “Where did the 2.5 deposited ETH actually come from? Was that actually a purchase? A trade? An airdrop? A gift?” If so, I need to edit or add data showing how I acquired that 2.5 ETH for tax purposes. Adding or further classifying this data will impact the ETH with known cost basis calculation.

The **most common reasons** for differing Calculated Balance vs Cost Basis Balance include:

- Missing transaction data from an exchange or wallet that you did not import to CoinLedger

- Withdrawals or deposits to a wallet without a matching deposit/withdrawal into another wallet

- **Deposits** that should actually be classified as **airdrops**

- **Deposits** that should actually be classified as **income**

- **Deposits** that should actually be classified as **gifts**

- **Deposits** that should actually be edited to **Trades** or **Fiat buys**


_Still have questions? Reach out to our support team, and we'll be happy to assist you!_

Did this answer your question?

😞😐😃