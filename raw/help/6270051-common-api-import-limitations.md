[Skip to main content](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#main-content)

# Common API Import Limitations

Learn the limitations of each API integration in the CoinLedger app

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over 11 months ago

CoinLedger supports many exchanges through API, but in some cases exchanges do not export the complete range of transaction history. This guide outlines current limitations with API import for each exchange and recommended steps that you can take to get your full transaction history imported.

- [Binance](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_0762c83c05)

- [Binance.US](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_eb30de1ecb)

- [Bibox](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_e2d6b4b09f)

- [BitMart](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_1fa6318198)

- [Bittrex](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_67a89054ba)

- [CoinSpot](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_1d309812b4)

- [Kraken](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_0d21bd5325)

- [KuCoin](https://help.coinledger.io/en/articles/6270051-common-api-import-limitations#h_4741c67360)


# **Exchange API Limitations**

## **Binance**

These transaction types are not returned by Binance's API:

- Fiat deposits and withdrawals

- Leveraged trades


Further, Binance restricts API imports for US traders. Any Binance user who previously had a working API import from Binance may try to re-sync their API and see a generic error message. It's recommended that you switch to a [file import](https://help.coinledger.io/en/articles/4935722-binance-us-file-import-guide) instead.

If you're struggling to access your Binance account as a US trader, there are a few tips to try. One method that has worked for US traders in the past is messaging Binance support and asking them to enable access to your account for a specific window of time. This way, you can export copies of all your trade files from Binance and keep them for your records. Make sure to download the Trade History file which is the version accepted by our software, but you might also want to download other copies of the Transaction History file as well just to have a backup.

Another thing to try is to log in to your account with a VPN. This does not always work, but we have seen that some customers have success with this.

## **Binance.US**

Binance.US has a limitation that do not allow the importing of crypto purchases made directly using a debit card, credit card, or bank account (ACH). As a result, these purchases are excluded entirely from the API import and will not appear in CoinLedger. If you've used Binance US to purchase crypto via the payments methods above, it is recommended you switch to the file import method. Please refer to the [Binance US File Import Guide](https://help.coinledger.io/en/articles/4935722-binance-us-file-import-guide) for further details.

Two alternative ways to add your Binance US fiat purchases are by using the Universal Import CSV (ideal for several transactions) or by adding individual transactions directly in CoinLedger (ideal for few transactions).

Fiat purchases using your USD account balance on Binance US do get exported correctly by Binance US. This limitation only applies to purchases made directly on Binance US with debit/credit/ACH.

## **Bibox**

Bibox's API only returns trades from the past 4 months. To get access to your complete trade history, we recommend switching to a [file import.](https://help.coinledger.io/en/articles/5397368-bibox-file-import-guide%5C)

## **BitMart**

These transaction types are not returned by BitMart's API:

- Staking rewards


Please note BitMart has a date range limit on their API calls **which means they only return data from the past 30 days.** As a workaround, we recommend importing via our [Universal CSV template](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide) instead.

## **CoinSpot**

These transaction types are not returned by CoinSpot's API:

- [Bundle trades](https://www.coinspot.com.au/bundles)


Additionally, CoinSpot's API may not return timestamps for certain trades, which can cause the import to fail. This issue is actively being worked on by the exchange.

## **Kraken**

These transaction types aren't currently supported by CoinLedger, and will cause your import to fail:

- Futures


## **KuCoin**

These transaction types are not returned by KuCoin's API:

- [Staking rewards](https://pool-x.io/) and POL credits

- NFT transactions

- KCS [dust conversion](https://www.kucoin.com/assets/trade-account/convertKCS/record) trades


These transaction types aren't currently supported by CoinLedger, and will cause your import to fail:

- Contract (Futures) trades

- [Lending](https://www.kucoin.com/margin/lend?lang=en_US) transactions


Additionally, U.S. users may not have access to API Keys on KuCoin.New U.S. customers are not able to complete KYC on KuCoin. According to recent [KuCoin policy changes](https://www.kucoin.com/support/360015102254), this means U.S. users may not have the ability to create API keys on KuCoin. For this reason, we recommend all U.S. users of KuCoin [switch to using a CSV File Import](https://help.coinledger.io/en/articles/8196376-kucoin-file-import-guide) instead.

Furthermore, due to technical limitations on KuCoin's end, their API is now limited to only retrieving data from the past year (going back 365 days from the date of the API sync). Transactions before that 365 day period may not be imported into CoinLedger. We recommend KuCoin users affected by this change [switch to using a CSV File Import](https://help.coinledger.io/en/articles/8196376-kucoin-file-import-guide) when importing their data instead.

Moreover, KuCoin trading account API Keys cannot access data from KuCoin sub-accounts. To import transactions from sub-accounts, log into every sub-account and create a new API Key. The process of creating a new API Key for the sub-account is exactly the same as for the main account, and can be found [here.](https://help.coinledger.io/en/articles/5603669-kucoin-api-import-guide)

Finally, due to a limitation within KuCoin's API, transactions before 2/18/2019 may not be imported. If you need to import trades prior to this date, follow [this](https://help.cryptotrader.tax/en/articles/5064627-kucoin-v1-file-import-guide) guide to export your KuCoin CSV files prior to 2/18/2019, or send a request for your complete trade history to KuCoin support.

Did this answer your question?

😞😐😃