[Skip to main content](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange#main-content)

# How to edit a deposit into a buy to fix incomplete data exported by a crypto exchange

Learn how fix your tax report when crypto exchanges exclude important data

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over a year ago

CoinLedger integrates with hundreds of exchanges, blockchains and wallets. Unfortunately, some exchanges do not export all the data required in order for CoinLedger to calculate both sides of a crypto transaction.

For example, if you purchase crypto with fiat, some exchanges will not export the fiat amount spent in the transaction and instead only export the _crypto amount received_. This means your transaction would get imported into CoinLedger incorrectly as a simple deposit.

This is especially the case for exchanges that use third-party payment platforms such as Ramp, Gem, Simplex, or Moonpay to facilitate debit, credit or ACH bank transfer purchases of crypto.

When exchanges only export the crypto amount received, CoinLedger does not have enough data to parse the transaction as a Buy. Instead, the transaction will be imported as one-sided crypto **Deposit** transaction (meaning it is excluded from your report calculations), which can cause [missing cost basis warnings](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-to-fix).

CoinLedger allows you to fix this by reclassifying any Deposit into a Buy.

# How to change a Deposit into a Buy within CoinLedger

In the CoinLedger app, a **Buy** refers to any transaction where fiat currency is exchanged for crypto. Purchasing crypto with fiat currency is not a taxable event in that there is no profit or loss to report until the crypto is sold or traded away. However, it is still critically important that all buys are imported in order to ensure that the original cost basis for the coin is included in your tax calculations.

Within CoinLedger you can reclassify any Deposit into a Buy if the exchange imported the transaction incorrectly. Check out the step-by-step walkthrough on this process below, or watch our short walkthrough video documenting the steps:

Reclassifying Deposits Into Buy Transactions

Copy link

[Open video in Loom](https://www.loom.com/share/f8890e64e36e484f995e1e110ffc9a9e)

0

1×

4 min⚡️4 min 51 sec3 min 53 sec3 min 14 sec2 min 35 sec2 min 17 sec1 min 56 sec1 min 33 sec

![](https://cdn.loom.com/sessions/thumbnails/f8890e64e36e484f995e1e110ffc9a9e-6b75d92220c16c20.jpg)

Copy link

[Open video in Loom](https://www.loom.com/share/f8890e64e36e484f995e1e110ffc9a9e)

0

1×

4 min⚡️4 min 51 sec3 min 53 sec3 min 14 sec2 min 35 sec2 min 17 sec1 min 56 sec1 min 33 sec

## Filter your transactions to look for one-sided Deposits

If you know that you purchased crypto with fiat currency on any of the exchanges listed above, the first step is to confirm whether those buy transactions have been imported as Deposits within CoinLedger.

Navigate to the **Transactions** stage and select filters for the exchange and the transaction type **Deposit**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1375688805/95dbd5b4b4e043cbcf6ea964ef84/Screenshot+2025-02-11+at+11_33_35%E2%80%AFAM.png?expires=1776713400&signature=04196f0ca0690b9f06d0bd03210ea693409138480e8cb1ec7b318075349fc045&req=dSMgE892lYlfXPMW1HO4zQcJzPabrBxgXaBrpEkbnLQVVnuTMi2zxeSsr4in%0A9hECXegmJL6xt3sI0E0%3D%0A)

_In the above example, some of the transactions labeled as Deposits are actually debit card fiat purchases made through a fiat-onramp provider on Exodus._

## Locate the original buy within your exchange account

Log in to your exchange account and search for the original buy transactions. The timestamp and the crypto amount displayed in your exchange account should match up with the timestamp and the crypto amount on the Deposit in CoinLedger.

_Here is an example of a buy transaction on Exodus:_

![](https://downloads.intercomcdn.com/i/o/610883805/b085a288ac34776f35e790f4/Screen+Shot+2022-11-04+at+9.58.26+PM.png?expires=1776713400&signature=ca473857fc9331fc175527ceb79cc411fb973a3ed61f150326c158c65acfedf7&req=ciEnHsF9lYFaFb4f3HP0gCB4S7EWezG6jzsTNLQrvUIxB2SIz39ehCccZWM5%0AXBlMRAx9uevv1hqwcw%3D%3D%0A)

_Here is how the Deposit transaction appears within CoinLedger:_

![](https://downloads.intercomcdn.com/i/o/610884210/8c2d006e85cdfa59e3e1a744/Screen+Shot+2022-11-04+at+9.59.34+PM.png?expires=1776713400&signature=bf2be991c77490d313afaae0a1eb69f84ae26c598b52e38f7f49e439cb2af352&req=ciEnHsF6n4BfFb4f3HP0gGBDfgM%2FSxft5UGgtyRRHQPXow2eqkWhpb67YE%2BR%0AiBdgekoe02yHtplB9g%3D%3D%0A)

## Change the Deposit transaction to a Buy and enter the fiat currency amount

You can now change the Deposit transaction to a Buy _in one of two ways:_

1. Click on the three dots next to the transaction, select **Change Classification** and select **Buy** (this is the easy method)

2. Click on the three dots next to the transaction, select **Edit transaction**, and edit the transaction into a Buy by adding in the fiat currency and amount as the _Asset Sent + Amount Sent_


Either of these methods is acceptable. Here are instructions on both processes:

### Reclassify the Transaction as a Buy (the easy method)

Locate the Deposit transaction that is actually a Buy.

Click on the three dots next to the transaction, select **Change Classification** and then select **Buy.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1375673094/321ac61f52b9c34f1a016ac97c30/Screenshot+2025-02-11+at+11_32_59%E2%80%AFAM.png?expires=1776713400&signature=e6469d1562f33eb9458f93be12060e48ff8c6ec8b8fac8b2577a03d8a77a1eb1&req=dSMgE895noFWXfMW1HO4zXt406fp6Yfgktv4Msdaz3tv7fUdpOPZxvbESAoQ%0ApYrWGhKAyomythYJyPo%3D%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1375672511/03791cd3b8845398f6c573405c81/Screenshot+2025-02-11+at+11_33_16%E2%80%AFAM.png?expires=1776713400&signature=99e7b16325dd5e4fc338df25ce6f649886116e2760bbecef4b5c28fbfaa10e74&req=dSMgE895n4ReWPMW1HO4zcC%2BMKpU6WEPCI7zlLswBRtu0nwQNVvXOHh43hux%0A5dXTRTAcuEAz5s3YF%2Fo%3D%0A)

Then, press **Save**. Now this Deposit has been changed to a Buy.

**CoinLedger will use the fair market value of that asset at the time it was received as your cost basis moving forward.**

### Edit the Transaction into a Buy

Click the three dots and select **Edit Transaction.**

![](https://downloads.intercomcdn.com/i/o/610887132/8b69482081fe8e0a4c5afef5/Screen+Shot+2022-11-04+at+10.03.02+PM.png?expires=1776713400&signature=36019dc2c86e34a651111f18f288927c306e13191a14bb5dae31af32ca4989b9&req=ciEnHsF5nIJdFb4f3HP0gCaTR3IHoJQ48iJJBLyw3OxZrK6zxqTU06Hry73D%0A655j03n0ysQH9VpJ5A%3D%3D%0A)

From the Edit Transaction window change the Classification to **Buy**, select a fiat currency as the **Sent** asset and enter in the amount of fiat currency you paid. You can also enter in any associated transaction fees.

![](https://downloads.intercomcdn.com/i/o/610886929/609356563168b11aebeb4a47/Screen+Shot+2022-11-04+at+10.05.50+PM.png?expires=1776713400&signature=1f6e8efd3df8291a660454d1c1d75424938ff745720fbc9f477fdb48944b63c9&req=ciEnHsF4lINWFb4f3HP0gMEjzLZBQWsp5qrLRTvS2M0Battv33DszE1REOUO%0AiKV%2FBcAwLwRcBCVxUw%3D%3D%0A)

## Repeat these steps for any other Buys that the exchange exports as one-sided deposits

It's important to carefully review all your original transactions within the exchange app to confirm which Deposit transactions should be changed to Buys (exchanging fiat for crypto). If you transferred crypto from one wallet to another, this should be left as Deposit.

_Have any questions? Our [support team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) would be happy to help :)_

​

Did this answer your question?

😞😐😃