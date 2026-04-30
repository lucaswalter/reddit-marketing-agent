[Skip to main content](https://help.coinledger.io/en/articles/6811823-how-to-fix-first-inflow-missing-basis-warnings#main-content)

# How to fix First Inflow Missing Basis warnings

Learn why First Inflow Missing Basis warnings occur and how to fix them

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 11 months ago

**First Inflow Missing Basis** warnings occur when CoinLedger detects that you have deposited or transferred crypto into your wallet, but you haven't shown us how you **originally** purchased or acquired it. When the original acquisition for the asset has not been imported, there is no way for CoinLedger to calculate what your cost basis is for that asset. Therefore, it is flagged with a Inflow Missing Basis warning.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1431049261/6397ae9543a190599df808bb8383/image.png?expires=1776713400&signature=4b64a9264ca3b60c7c3b7bc780833f724c805867c598d2c883db24cc90fb9d9c&req=dSQkF8l6lINZWPMW1HO4zSCARwPxdCa27fznB0h3Zh%2BpQTKZFit4NU9Z3iFx%0AZPVb%2FAM1XppUQqUTsbI%3D%0A)

If you are missing cost basis for an asset in your CoinLedger account and your **first imported transaction** for that asset is a **Deposit** or **Uncategorized** transaction, it will be flagged for a First Inflow Missing Basis.

### Example

Let's run through an example to better illustrate how First Inflow Missing Basis Warnings occur:

- You buy 10,000 MIM tokens on a centralized exchange: Kucoin

- You then send 2,294.10 MIM tokens to your self-custodied Arbitrum wallet

- You import **only** your self-custodied Arbitrum wallet to CoinLedger—you **do not** import from Kucoin


In this case, you haven't imported the original BUY transaction of your MIM tokens, and thus, CoinLedger does not know your cost basis for MIM.

If you import only your Arbitrum wallet into CoinLedger, the deposits of MIM tokens from Kucoin will be flagged with First Inflow Missing Basis Warnings (pictured below).

In the picture below, the first detected transaction for MIM is an inflow—a **Deposit**. However, there are no other prior BUY, TRADE, or INCOME transactions to set the cost basis for these tokens and to show how the MIM was originally acquired.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534590496/d141ced1e8afdd5827f32e76bd5c/Screen%2BShot%2B2023-02-22%2Bat%2B7_47_48%2BAM.png?expires=1776713400&signature=6dad8b8d381331af2bc49dafe1a7712a019b20eae38fc797fe836d300baa502f&req=dSUkEsx3nYVWX%2FMW1HO4zcWGKhT0h0L89YgCMQ6dDX9NlxkWQo43j8XUS88o%0ADMwi%0A)

# **How Do I Fix a First Inflow Missing Basis Warning?**

There are two ways to show CoinLedger how the asset was originally acquired:

1. [Edit the flagged Deposit or Uncategorized transaction and change the classification to a different transaction type that assigns cost basis](https://help.coinledger.io/en/articles/6811823-how-to-fix-first-inflow-missing-basis-warnings#h_cc63713424)

​

2. [Import additional data that shows how the asset was acquired](https://help.coinledger.io/en/articles/6811823-how-to-fix-first-inflow-missing-basis-warnings)


# **Editing a Transaction to Resolve the First Inflow Warning**

There are some scenarios when CoinLedger does not automatically classify a transaction when it is imported. Such transactions need to be classified further in order to properly assign cost basis.

Here are some situations where you will need to do this:

### Changing the classification to crypto income

If a flagged Deposit transaction is actually an instance of you receiving crypto income (like income from staking, interest, mining, airdrops, etc.), you can reclassify it by selecting the three dots next to the transaction and clicking **Change Classification**. From there, you can select the appropriate transaction type and then select **Save**.

### Changing the classification to a Buy

In some cases exchanges do not export complete data for fiat buys (purchasing crypto with fiat currency) so the transaction gets imported as a Deposit into CoinLedger. To resolve this, you can reclassify the Deposit transaction into a Buy. Learn more about that process [here](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange).

### Changing the classification to a Trade

If you transacted with DeFi protocols that CoinLedger does not yet natively support, some trade transaction types will need to be classified further in order to be included in report calculations. For tax purposes, **Trades** include all scenarios where you swapped one or more crypto tokens for another digital asset.

- **Trade** \- swapping one crypto asset for another crypto asset

- **Multi Asset Swap** \- a trade where there are multiple crypto tokens on one or both sides of the trade

- **NFT Mint** \- swapping crypto for an NFT

- **Adding/Removing Liquidity** \- swapping crypto for an LP token or vice versa


### Classifying an Uncategorized Transaction

If your wallet transacted with a smart contract or decentralized app that we don’t have a native integration with yet, the transaction will be classified as **Uncategorized** in CoinLedger. Uncategorized transactions may also appear when you import a transaction type that CoinLedger doesn't automatically recognize. They are excluded from your report calculations, which can lead to missing cost basis warnings. Learn how to classify Uncategorized Transactions [here](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions).

# **Importing Additional Data to Resolve the First Inflow Warning**

CoinLedger needs access to all your historical data in order to calculate your gains and losses. The software cannot generate accurate calculations based on inaccurate or incomplete data. Follow these steps to review your imported data and ensure that all original fiat buys, trades, and crypto income transactions have been imported completely into CoinLedger.

1. Confirm that you imported historical data for ALL exchanges, wallets, and platforms that you used to buy, sell, trade, and earn crypto income

​

2. Confirm that you imported for ALL of the years that you transacted with crypto

3. Review all exchanges, wallets, and platforms that you used to purchase the asset with fiat currency

​

4. Review all exchanges, wallets, and platforms where you received the asset as crypto income

​

5. Review all exchanges, wallets, and platforms where you acquired the asset by trading for it


### Adding a new import source

To import from an exchange, wallet or blockchain, go to **the Import page**, select **Add Account,** choose your platform, and follow the step-by-step instructions on your screen to complete your import.

If you don't know which platform to import, CoinLedger can help. In some instances, CoinLedger will flag the source (i.e. crypto exchange or wallet) where a deposit was sent from. In this example below, I have a First Inflow Missing Basis warning for ETH in my MetaMask. When I click on the transaction and expand it further, I can see that this ETH was originally sent from my Coinbase account. This means that I can resolve my Inflow Missing Basis warning by simply importing my Coinbase transactions.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534594729/e8346451c33322e8dfe7f4acca59/Screenshot-2B2025-03-19-2Bat-2B4_55_06-E2-80-AFPM.png?expires=1776713400&signature=8cbf70b0c70f61b1d2a2d883b828f786150a2461044b8a4ea2e42d7d6d9e9d45&req=dSUkEsx3mYZdUPMW1HO4zc8LmUT979aqFML8Qs%2FhfOopDmZ0s6CFU1E3Empn%0A2FpB%0A)

### Adding transactions manually

If you transacted on an exchange or blockchain that we do not currently support you can import the data using our [Universal Manual Import Template](https://help.cryptotrader.tax/en/articles/6028758-universal-manual-import-template-guide) or you can [add single transactions in-app](https://help.coinledger.io/en/articles/6125080-how-to-add-single-transactions-in-app).

# **Can You Run a Tax Report with a First Inflow Missing Basis Warning?**

Yes.

CoinLedger will still run your tax report in spite of missing cost basis data. In many circumstances, First Inflow Missing Basis warnings _will not_ have any significant effect on your gains and losses, particularly if you are simply holding the asset and do not sell or trade it away. This is because there is no gain or loss to report until you dispose of the asset by selling or trading it away.

However, if you later dispose of the asset without entering the original acquisition, it's possible that your report could be impacted. Our platform treats missing data with a zero cost basis, which is the most conservative approach but can inflate your gains if left unresolved. Learn how how missing cost basis data will effect your tax report in [this article here](https://help.cryptotrader.tax/en/articles/2865416-what-happens-if-i-run-my-report-with-a-negative-balance-warning).

_Have any questions? Our support team would be happy to help :)_

Did this answer your question?

😞😐😃