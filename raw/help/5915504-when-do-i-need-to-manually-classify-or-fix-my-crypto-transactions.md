[Skip to main content](https://help.coinledger.io/en/articles/5915504-when-do-i-need-to-manually-classify-or-fix-my-crypto-transactions#main-content)

# When do I need to manually classify or "fix" my crypto transactions?

Occasionally you may need to classify or fix your transactions in CoinLedger - learn how to do this here

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 6 months ago

CoinLedger integrates with hundreds of exchanges, blockchains and wallets. Most of the time, your transactions will be classified correctly the first time you import them. However, some exchanges or blockchains report data in an incomplete state.

For example, if you purchase crypto with fiat, some exchanges will not export the fiat amount spent in the transaction and instead only export the _crypto amount received_. This means your transaction would get imported into CoinLedger incorrectly as a simple deposit.

On the other hand, some blockchains may report a transaction type to CoinLedger that we do not automatically integrate with yet, and this will lead to it being imported as an uncategorized transaction.

In these rare cases, you'll need to manually classify these transactions into the correct type so that the proper tax treatment gets applied. We will discuss how and when to do this below.

# When do I need to manually classify transactions?

You may need to manually classify a transaction when:

- You see [Uncategorized transactions](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions) on your account

- A buy of crypto was [imported as a simple deposit](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange), leading to a missing cost basis

- A sell of crypto was imported as a simple withdrawal

- A transaction where you received crypto income was imported as a simple deposit

- CoinLedger flagged a [Potential Trade, Bridge or Transfer](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab) within your account

- You want to change a standalone deposit or withdrawal into a Transfer to resolve an inaccurate portfolio tracker balance or missing cost basis warning


# How can I classify my transactions?

You can review, edit and classify your transactions on the [Transactions page](https://app.coinledger.io/individual/transactions). You classify transactions one-by-one or in bulk.

Click on the drop-down sections below to learn how to classify your transactions in each of the following scenarios.

## Uncategorized Transactions

If your wallet transacted with a smart contract or decentralized app that we don’t have a native integration with yet, the transaction will be classified as **Uncategorized** in CoinLedger. Uncategorized transactions may also appear when you import a transaction type that CoinLedger doesn't automatically recognize.

Uncategorized transactions are treated as non-taxable events that are not factored into your report calculations. Learn how to classify these transactions in [this guide.](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions)

If you have questions specifically about classifying NFT Mint transactions which were imported as Uncategorized, those can be answered here: [How to classify NFT Mint transactions](https://help.coinledger.io/en/articles/6105647-how-to-classify-nft-mint-transactions-and-remove-missing-cost-basis-warnings)

## Fix a Buy that was imported as a deposit

If you are looking to fix a buy which was imported into CoinLedger as a simple deposit, you can learn more about that process here: [How to edit a deposit into a buy to fix incomplete data exported by a crypto exchange](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange)

## Fix a Sell that was imported as a withdrawal

To fix a sale of crypto that was imported as a withdrawal, select the 3 dots next to the withdrawal transaction, click Change Classification, and then select Sell. After that, hit **Save**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1751673223/374a1029047080a05077a572e110/Screenshot+2025-09-29+at+4_59_06%E2%80%AFPM.png?expires=1776713400&signature=add6b3a920fb20b6866f7a38dd83632a0349e5353a10d379ef548fd3af3ee3fc&req=dSciF895noNdWvMW1HO4zXDQMn%2FSVjCC2eCMXqBZkqmLiUIeiPVUramCCDAZ%0A2lz0%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1751673237/93d259aa0a8a27e9e20a28bca893/image.png?expires=1776713400&signature=5e27dfa4f35efb4edf0aa124aaa3517d747e102e73b558acab7b1b6c449ca142&req=dSciF895noNcXvMW1HO4zVgG7grOuhZNx5%2FqNLz4q%2FQjX2jfK6KXvbiOifEp%0AkjKV%0A)

Your Withdrawal will now automatically be converted into a Sell.

**CoinLedger will use the fair market value of that asset at the time it was received as your cost basis moving forward.**

## Crypto income transaction imported as a deposit

A transaction which appears to be a simple deposit could actually be an instance of you receiving crypto income. Crypto income transactions can include:

- airdrop

- staking reward

- mining reward

- received gift

- interest income


If you believe that a crypto income event was imported into CoinLedger as a deposit, you can resolve this by reclassifying the transaction. We recommend reviewing the transaction history of the exchange or wallet the transaction occurred in before doing so to ensure you select the right transaction type.

**Step 1**

Locate the transaction you would like to classify. Then, click on the three dot menu and select **Change classification**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1532925797/2f36edfd80565e9f8173ef4d049e/Screenshot+2025-05-20+at+3_26_35%E2%80%AFPM.png?expires=1776713400&signature=422612380d6ff855e99f150e0f441ceff9d21588ac29e4b3f4f9c3e5d3c9b5da&req=dSUkFMB8mIZWXvMW1HO4zbm9DuznF%2B1URJgp6w02Jq9wDN84UOO5IRSqPRyy%0AvNwQ%0A)

**Step 2**

Select the transaction type you would like to reclassify it to, and then press **Save**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1532926258/5c6cdfedb92514dd2bcb17535c42/image.png?expires=1776713400&signature=732287898aff9a49e4291b2f81373e2e55a8c8d752194cd36145ea18cb6ae6bf&req=dSUkFMB8m4NaUfMW1HO4zXpgEcXDugCKQng9avwB3BjXM2WXVutpuT1%2Fwnt4%0A%2F7r5%0A)

You can also reclassify multiple transactions at once by checking the box next to each transaction and then clicking **Mark as**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1532929530/377912c007def7d926c1b0734f39/Screenshot+2025-05-20+at+3_28_29%E2%80%AFPM.png?expires=1776713400&signature=f2a4357eef1ff80f78c4dd7793064450533cc3aefa762aa7bdbf733d45b834c1&req=dSUkFMB8lIRcWfMW1HO4zdtlUOQRePZyaGHFDv5vCHvyh1rFt7yca1vbLxaw%0AXkvr%0A)

Finally, select the transaction type you would like to reclassify the transactions to. Each of the transactions you selected will now be reclassified.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1532936201/dd99cd59f3ed74a9a243e4accc92/image.png?expires=1776713400&signature=aafa9a0fc55044332aecf388a133593a27d667b562a4a5ad5f38a77456c6131f&req=dSUkFMB9m4NfWPMW1HO4zcEB0fvbFde4XehdRtsYrXlcVFgu%2BEWYUlxCp6SK%0ACdHw%0A)

## Classify a Potential Bridge, Trade or Transfer

CoinLedger will identify any potential bridge, transfer or trade transactions that were not automatically mapped upon import on the **[Transactions page](https://app.coinledger.io/individual/transactions)**. If our system flags any of these potential transactions on your account, we recommend merging them together to ensure that your capital gains are calculated correctly. You can easily merge these transaction together by following the process [here](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab).

## Changing a standalone deposit or withdrawal into a Transfer

In CoinLedger, you can easily reclassify a standalone deposit or withdrawal into a **Transfer** by following [these steps](https://help.coinledger.io/en/articles/11426960-how-can-i-reclassify-transactions-in-coinledger?q=manually+fix+#:~:text=supports%20here.-,Changing%20a%20Deposit%20or%20Withdrawal%20into%20a%20Transfer,-In%20CoinLedger%2C%20you). This is useful for resolving data issues such as inaccurate balances on the Portfolio Tracker or missing cost basis warnings.

Did this answer your question?

😞😐😃