[Skip to main content](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#main-content)

# How does the Portfolio Tracker work?

Learn how CoinLedger's Portfolio Tracker calculates your asset balances.

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over a year ago

![](https://downloads.intercomcdn.com/i/o/958630270/379c3041366829a9d373051e/image.png?expires=1776713400&signature=bc2c659784d3278949cffed54174b211e7008e687df878bf23da35109f59883c&req=fSUvEMp%2Bn4ZfFb4f3HP0gDhFuEVK0jM0x4x%2F41Oeggadfu7FRnSGDAT3JBZW%0Aegs9ljbT9OjDLkHMZg%3D%3D%0A)

CoinLedger’s Portfolio Tracker tracks the amount, price, market value, cost basis, percentage change, and unrealized return of the cryptocurrencies held across all of your imported wallets. Learn more about the Portfolio Tracker below and use the **Jump Ahead Table of Contents** to navigate this article.

# Jump Ahead

- [How does the Portfolio Tracker calculate my asset balances?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_7354892df3)

- [Does CoinLedger use a Global Wallet for asset balance calculations?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_a93f1b862c)

- [Does CoinLedger use “reported balances” from exchanges or blockchains to display asset balance?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_3c42b26cde)

- [Why are my asset balances incorrect?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_3283049323)

- [Why am I getting a Negative Balance Warning?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_7821f80199)

- [Why am I getting a Missing Cost Basis Warning?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_0ac8953b10)

- [Why does the price of this asset on my account look incorrect?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_b9fd059903)

- [What is market value, cost basis and unrealized return?](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#h_e7af64c9ad)


## How does the Portfolio Tracker calculate my asset balances?

CoinLedger calculates your asset balances based on the imported transaction data across all of your wallets. If you do not import all of your historical transactions into the system, your tracked balances will not be correct.

**Example:**

Suppose you have the following transaction history imported into CoinLedger:

- Deposit 1 BTC

- Trade 0.5 BTC for 1 ETH

- Withdrawal 0.25 BTC


In this example, your calculated balances would be 0.25 BTC and 1 ETH. CoinLedger sums together all of the debits and credits for each asset to arrive at the calculated balance.

## Does CoinLedger use a Global Wallet for asset balance calculations?

Yes. CoinLedger sums the transactions across all of your imported wallets to arrive at a “Global Wallet” asset balance. This global asset balance is what gets reported on the portfolio tracker.

## Does CoinLedger use “reported balances” from exchanges or blockchains to display asset balance?

No. All balances displayed in the portfolio tracker are calculated based on your imported transaction data.

## Why are my asset balances incorrect?

CoinLedger calculates your asset balance based on your imported transaction data.

If your asset balances are incorrect, this means that the sum of the debits and credits from your imported transaction data do not add up to your current holdings. This could be because one or all of your data imports are missing or out of date. In other words, there is probably missing or inaccurate transaction data imported to your CoinLedger account. As a first step, we recommend checking that your imports are up-to-date, and even re-syncing them on your account by navigating to the Import stage of the CoinLedger app and then pressing the **🔁 Sync All** button shown below. If this does not fully resolve your incorrect balances, you may need to import a missing data source into your CoinLedger account.

![](https://downloads.intercomcdn.com/i/o/1123461777/f6a6d28abc506f2b34905859/Screenshot+2024-07-24+at+11_27_08%E2%80%AFAM.png?expires=1776713400&signature=2ad371ef3c60b68e098623a41cc6b7ffc292438ea9af8416f6098f8960fe5f93&req=dSElFc14nIZYXvMW1HO4zce2%2BRyDMwex35yJdqfepGRhwQ5wvUWttASvQAfQ%0A5KkN9RsAnFJC8o9UX1w%3D%0A)

We also recommend double-checking that you have not ignored any transactions on your account, as ignoring a transaction would exclude it from the calculations our portfolio tracker uses to display your asset balances.

You can troubleshoot your asset balances in the Portfolio Tracker by using the [Asset Balance Report](https://app.coinledger.io/individual/asset-balance-report). The Asset Balance Report allows you to view each of the transactions that CoinLedger uses to calculate your balances. To locate the Asset Balance Report, click on the [direct link](https://app.coinledger.io/individual/asset-balance-report) to it in the top right of your Portfolio Tracking page.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338574442/49bc17f6f99f09a87c724afa041a/Screenshot-2B2025-01-16-2Bat-2B12_23_23-E2-80-AFPM.png?expires=1776713400&signature=c911c29d880ace2b8d75881469878196c7f54982f95ecfd7c5cee56fdd26df99&req=dSMkHsx5mYVbW%2FMW1HO4zVx9f2pN%2BQvkhxD0wFZD6lDesjr8CStiZVcIGs25%0Au%2B2qx3Jx2INTXE9U1A4%3D%0A)

From there, you can drill down into each of the transactions influencing your asset balance calculations, including taxable transactions such as trades and sells, and nontaxable transactions like deposits and withdrawals.

## Why am I getting a Negative Balance Warning?

If the debits and credits associated with your imported transaction data add up to a negative number for a particular asset, you will see a Negative Balance Warning reported on your asset holdings breakdown.

**Example:**

Suppose you have the following transaction history imported into CoinLedger:

- Deposit 100 SOL

- Trade 25 SOL for 1 ETH

- Withdrawal 100 SOL


In this example, your calculated balances would be (-25) SOL and 1 ETH. In this case, CoinLedger will flag a Negative Balance Warning for your SOL holdings.

**How can I fix a Negative Balance Warning?**

As illustrated in the example above, Negative Balance Warnings are the result of inaccurate or incomplete imported transaction data. To fix them, you should review all of your imported transactions. Transaction data can be added, edited, and altered on the **Transactions** tab, but you can also view the transactions factoring into your asset balances on the **Asset Balance Report**.

As shown below, using the Asset Balance Report you can pull up the first instance of a negative balance for an asset on your account, making it easy to pinpoint the reason for that negative calculated balance.

![](https://downloads.intercomcdn.com/i/o/958640966/a5674526efa5ee1e9c9d7df0/Screenshot+2024-02-09+at+10.29.22%E2%80%AFAM.png?expires=1776713400&signature=fbf05d9cd484cca81cf86f9fe539c7b672bcaaae399e2b096db4881edc46997a&req=fSUvEM1%2BlIdZFb4f3HP0gAMLBxjpE93Grr6LwAqE%2BqcQKj7dlvAYz8gR6c3Q%0AK0NlhGM7w7rlseNdbQ%3D%3D%0A)

Here we can see that Bitcoin on my account has a negative calculated balance. Using the Asset Balance Report, I was able to discover the first transaction with a negative calculated balance for that asset. I can see that the cause of this negative balance was a Sell on Crypto.com.

![](https://downloads.intercomcdn.com/i/o/958645102/c90c5a1860095dcfa1b70db3/Screenshot+2024-02-09+at+10.34.30%E2%80%AFAM.png?expires=1776713400&signature=5074e17add4f2e283b2f7e586a6ef794e2bb80c96159f88fb3d5b2e7e21831bb&req=fSUvEM17nIFdFb4f3HP0gMeIfYV2p4Gws%2BjqZVXaozOWYo4O%2Ff9esR9MzA%2FU%0Awa8O8bAsqu6zEYUzKA%3D%3D%0A)

![](https://downloads.intercomcdn.com/i/o/958645405/527ad82b9e36cfd217dcc3b5/Screenshot+2024-02-09+at+10.35.07%E2%80%AFAM.png?expires=1776713400&signature=55ec494e12525de6c9f4fe5d977e465e9da8f2c285c445a98dff3507a56528c9&req=fSUvEM17mYFaFb4f3HP0gFzmYMuwn8UhZIAATg2BWUZ7d0dYZqk8WIjeL4xx%0A3AwdUAi63YJlJupHDg%3D%3D%0A)

This likely means that I'm missing transaction history data for one of the platforms or exchanges I used to buy, sell and trade Bitcoin. I can resolve this Negative Balance by simply importing that missing data.

## Why am I getting a Missing Cost Basis Warning?

CoinLedger calculates the cost basis for your assets based on your imported transaction data. If you have not imported data showcasing how you originally acquired some of your crypto, you will see a Missing Cost Basis Warning on your asset holdings breakdown.

**Example 1:**

Suppose you have the following transaction history imported into CoinLedger:

- Deposit 1 BTC


In this example, you will have a Missing Cost Basis warning for 1 BTC flagged. A simple deposit does not tell CoinLedger how you originally acquired that 1 BTC. Thus, there is not enough information to set the cost basis for the asset.

Did you originally buy it with dollars? Did you earn it as income from a job? Did you receive it as a gift? If any of these are true, you need to edit the deposit transaction into its true transaction type (income, buy, gift, etc.) on the **Transactions** tab. Doing so will properly set the cost basis for the asset.

**Example 2:**

Suppose you have 2 primary wallets with the following transaction history:

Coinbase Exchange:

- Buy 10 ETH for $15,000 USD

- Withdrawal 10 ETH


MetaMask Wallet:

- Deposit 10 ETH

- Trade 5 ETH for 0.5 BTC


For this example, let’s say you only imported your MetaMask wallet to CoinLedger. If this is the case, your ETH will be flagged with a Missing Cost Basis Warning. If solely the MetaMask transaction data gets imported, CoinLedger will be missing your original Buy of 10 ETH for $15,000 USD. This is the transaction needed to properly set the cost basis for your held ETH.

To learn more about how you can troubleshoot Missing Cost Basis Warnings, please review our [Missing Cost Basis Warning help guide](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning).

## Why does the price of this asset on my account look incorrect?

Prices in CoinLedger's Portfolio Tracker are refreshed automatically on an hourly basis. The latest prices, grabbed directly from the market indexes we use for our historical pricing, should show up automatically when you first log into the app. If prices don't seem to be updated or accurate on your account, please hit the " **Refresh Data" button** in the top right corner of the screen. This should refresh the prices for you account.

![](https://downloads.intercomcdn.com/i/o/991939361/a93104be6a3c9c9f98f8807c/Screenshot+2024-03-14+at+2_11_45%E2%80%AFPM.png?expires=1776713400&signature=17416b619902da3d371e4b7901703784b40365124bc7a8b2706ccb5ea134e245&req=fSkmH8p3nodeFb4f3HP0gI%2FZq6JJdv1ytLzOL7RgF%2Fd5grRMDSSJwdQYEeJ6%0AmrEMJdRtVMIJW%2FFxbw%3D%3D%0A)

Please not that, as our prices are refreshed on an hourly basis, it's reasonable to expect some small, slight variations in pricing from time to time.

## What is market value, cost basis and unrealized return?

CoinLedger's Portfolio Tracker displays each asset in your account as well as the market value, cost basis and unrealized return for each. Here's a brief definition for each of those terms:

1. Costs basis represents the original value of an asset for tax purposes. Put another way, it typically represents how much money you put into purchasing your crypto.

2. Market value is the current fair market value of an asset, expressed in fiat currency.





1. Ex: 1 BTC=$40,000 USD


3. Unrealized return is the difference between the market value and cost basis fields. It's what your return would be if you disposed of the assets, given what you invested to acquire them.


## Other questions?

CoinLedger’s Portfolio Tracker is still a new product. If you have other problems, suggestions, or questions, please reach out to our support team. We will be thrilled to hear from you!

Did this answer your question?

😞😐😃