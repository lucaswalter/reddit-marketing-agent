[Skip to main content](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#main-content)

# My capital gains/losses don't look correct. What should I do?

Learn why your capital gains or losses may look different than you expected, and how to troubleshoot

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 8 months ago

If your capital gains or losses shown on the Tax Reports page don't match your expectations, there could be a few explanations for this. The most common is missing transaction history data. Other reasons can include uncategorized transactions, ignored transactions, gains from stablecoin or crypto-to-crypto trades, or simply underestimating the value of the crypto you sold in a given tax year. Below, we'll jump into each of these reasons and provide some helpful solutions for troubleshooting your capital gains.

## **Jump Ahead Table of Contents**

- [Missing transaction history data (MCB Warning)](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_330e47ad6b)





  - [Where to check if you have missing data](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_8d9e0c2342)

  - [How to fix](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_e837294cf6)


- [If you are not missing any transaction history data](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_1d436a3a98)





  - [Report calculation method](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_1d7a6d480e)

  - [Uncategorized and ignored transactions](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_62330a1df7)

  - [Review your transactions with the highest capital gains](https://help.coinledger.io/en/articles/2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do#h_aa296dfcbb)


# You may be missing transaction history data which is inflating your gains (Missing Cost Basis Warning)

The most common reason for your capital gains or losses looking inaccurate is that you are missing transaction history data which is inflating your gains. CoinLedger crunches numbers based on the data that you import into our platform. In other words, our software works by importing all of your buys, sells, trades, and crypto related transactions across _all_ of your cryptocurrency platforms. The application normalizes all of this data and sorts it chronologically.

When CoinLedger detects that you are selling or trading a cryptocurrency that it does not have any record of you ever acquiring, it flags the transaction as a **Missing Cost Basis** (as you are missing your cost basis for this sale/trade of the particular cryptocurrency). Most of the time CoinLedger is able to establish your cost basis automatically, as long as you have imported ALL of your crypto transactions, from ALL years of your trading history. But if this data is not imported, we are not able to properly calculate your cost basis, which can lead to inflated capital gains.

**For example:** let's say I purchased 0.5 BTC on Gemini for $10,000, and then I sent it to Coinbase months later where I sold it for $20,000. If I _just imported my Coinbase data_ into CoinLedger, the software will have no way of knowing _where_ I bought my BTC, _how much_ I acquired it for, and _when_ I purchased it. To CoinLedger, it will look like this 0.5 BTC just appeared in my Coinbase account. Therefore, when I sell it, CoinLedger will assume I acquired it for $0 - **meaning my capital gain on this transaction would be $20,000.**

I could resolve this by importing my Gemini data into CoinLedger. Now, CoinLedger will be able to see that I originally purchased this 0.5 BTC for $10,000 prior to sending it to Coinbase and selling it - and can accurately calculate the correct capital gain for this sale: $20,000 - $10,000 = $10,000.

## Where can I see if I have missing data?

If your account has any assets with a missing cost basis, you’ll see these flagged on the [Transactions](https://app.coinledger.io/individual/transactions) page with a Missing Cost Basis banner.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1401661271/0012ff0cbccf3c705b9a2a0f6d0c/image.png?expires=1776713400&signature=d8a0d90483b7619f44b515a836e6fcd66ec40cae97767a99daf21ddeb949d6f1&req=dSQnF894nINYWPMW1HO4zY3DblAiRhNzIXJKHCxW%2BUOGt8XkQNTwdKwdADJD%0APLLhIVz%2Btad7cX7IICE%3D%0A)

## How do I fix a Missing Cost Basis Warning?

- **Step 1:** [Import](https://help.coinledger.io/en/articles/9174597-i-m-a-first-time-coinledger-user-how-do-i-get-started#:~:text=Import%20Your%20Accounts) your missing transaction history data - be sure to import all the exchanges, blockchains and wallets you have used to buy, sell and swap crypto over the years

- **Step 2:** If this does not resolve your Missing Cost Basis Warning, you can enter a [Manual Position](https://help.coinledger.io/en/articles/10080173-can-i-manually-enter-an-asset-s-cost-basis-aka-a-manual-position) to manually resolve your missing cost basis


Learn more about resolving Missing Cost Basis Warnings [here](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-to-fix).

# If you are not missing any transaction history data

If you are not missing any transaction history data and do not have any Missing Cost Basis Warnings flagged on the Transactions page, but are still seeing inaccurate capital gains, you should proceed with the following troubleshooting steps.

## Try changing your report calculation method

A report calculation/accounting method helps you determine the order in which you dispose of your cryptocurrency. This method can have a big impact on your capital gains and losses. When troubleshooting inaccurate capital gains, it's helpful to review the method applied on your account. The default method for US customers is HIFO, but in some cases you may see that your capital gains change after trying out a different calculation method. To learn more about changing your report calculation method, [please see this guide](https://help.coinledger.io/en/articles/3130354-which-crypto-tax-accounting-methods-does-coinledger-support).

## Make sure you don't have any ignored or uncategorized transactions

If your wallet transacted with a smart contract or decentralized app that we don’t have a native integration with yet, the transaction will be classified as **Uncategorized** in CoinLedger. Uncategorized transactions are treated as a non-taxable events that are not factored into your report calculations. To include them in your tax report, you'll need to categorize them. Check out [this guide](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions) for more information!

Likewise, ignoring a transaction will remove it from your tax report calculations. We recommend double-checking on the [Transactions page](https://app.coinledger.io/individual/transactions) to ensure that you haven't ignored any transactions on accident. You can check for both ignored and uncategorized transactions using the **Filters** on the Transactions page, as shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1401698538/9a0d59c816eb9518b661ffd7e39d/Screenshot+2025-02-28+at+12_45_50%E2%80%AFPM.png?expires=1776713400&signature=47c5ce89e83911b22dbf7fbb1e79f6f2d936db0f2951985adf1d53914e019a31&req=dSQnF893lYRcUfMW1HO4zcDEStXnEINWoMXR0gkXGiVQANHQZuzp80Z21Ob5%0ANxNhiqiOiOnG7Qb6L3Q%3D%0A)

## Use the Tax Reports page to review your transactions with the highest capital gains

Using the [Tax Reports page](https://app.coinledger.io/individual/reports), you can review the transactions on your account which are increasing your capital gains the most. Navigate to the Tax Reports page and then scroll down to the **Capital Gains Summary** section. Then, click on either **Short** or **Long Term** (we suggest reviewing both) **.** This will open up a breakdown of your capital gains for the year, and will show in detail how they were calculated.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1401696143/311a11c2903d4c620b11e7ba11b9/Screenshot%2B2025-02-28%2Bat%2B12_31_08-E2-80-AFPM.png?expires=1776713400&signature=b09448e4d760a4b300c58df84f717e47b81e86c62ff572e0f280ee1c6b4332b8&req=dSQnF893m4BbWvMW1HO4zXVn2aB8RJrgIywDTjJ7wXN20V9fAZKmaVNzYUuy%0AV2eY6goBecZ0BVo41fc%3D%0A)

Next, click on the Gain/Loss column twice to filter for the transactions which are increasing your capital gains the most.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1401696146/c0fc3490c9466bdf612a55d03e6c/Screenshot%2B2025-02-28%2Bat%2B12_33_04-E2-80-AFPM.png?expires=1776713400&signature=5288f7d40e8ab0a1bfbf6fd662f9d8a8e4d83c1edf985ce22d6389f7680aec5e&req=dSQnF893m4BbX%2FMW1HO4zcJPdnYPEfRcbuw7iMJzn4fF6QGqWg3j4iG%2FFsYa%0AHtPdZhFTNOuD6iie1DU%3D%0A)

Here, you will see a breakdown of how CoinLedger calculated your capital gains. If you believe your capital gains are inaccurate, we recommend thoroughly reviewing each of these transactions to see how they were calculated. **If you have imported all of your transaction history into CoinLedger, including all of the exchanges you have used and all years of your transaction history, then the calculations shown here are most likely correct.**

As a note, these calculations represent capital gains from both selling your crypto for fiat AND trading your crypto for other crypto assets. Please remember that both of these are considered taxable events according to the IRS, and they will trigger capital gains or losses.

According to US law, the IRS counts crypto to crypto trades as taxable events, meaning you will always have to pay taxes on these trades. Any trade of one crypto asset for another is still a taxable event, even if you are trading a stablecoin for another crypto asset. Please see this blog for more info: [https://cryptotrader.tax/blog/the-traders-guide-to-cryptocurrency-taxes](https://cryptotrader.tax/blog/the-traders-guide-to-cryptocurrency-taxes)

Did this answer your question?

😞😐😃