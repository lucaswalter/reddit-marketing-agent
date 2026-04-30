[Skip to main content](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#main-content)

# Gate - File Import Guide

How to import your Gate trading history into CoinLedger

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 5 months ago

Gate does not export an "All Transactions" file that includes all transaction types. Instead, Gate exports three different file types: **Trade History, Deposits, and Withdrawals**. Each of these files contains completely separate transactions.

For this reason, it is very important to carefully review all transaction types that you had on Gate and then export each file that contains these transaction types. This guide includes descriptions of the data included in each file as well as step-by-step instructions for importing each file into CoinLedger.

Jump ahead with this table of contents:

1. [Import Walkthrough](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#h_1a79b33155)

2. [Gate Import Limitations](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#h_5895ee24c3)


### Trade History File

The Trade History file contains crypto-to-crypto spot trades and sells (exchanging crypto for fiat currency such as USD) The Trade History file does NOT include fiat purchases made on Gate using debit/credit or ACH bank wire.

- [Trade History File Import Instructions](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#h_1a79b33155)


### Deposits File

The Deposits file contains crypto deposit transfers into Gate. Fiat purchases (buying crypto with fiat currency such as USD) are exported in the file as one-sided crypto deposits. This is because Gate does NOT include the fiat amount spent, but only exports the amount of crypto received. If you purchased crypto directly on Gate, follow these instructions for fixing these one-sided crypto deposits so that they are properly calculated as Fiat Buys within CoinLedger.

- [Deposits File Import Instructions](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#h_439c18350a)

​

- Editing one-sided deposits within CoinLedger


### Withdrawals File

The Withdrawals file contains crypto withdrawals out of Gate.

- [Withdrawals File Import Instructions](https://help.coinledger.io/en/articles/2897126-gate-file-import-guide#h_9491628288)


# **Import Walkthrough**

## **Importing the Trade History File**

#### **Step 1:**

Follow the steps detailed here: [Gate Trade History Guide](https://www.gate.io/help/guide/16560)

Step 2: Hit the "Add Account" button on the bottom left, then drag & drop your trade history file, or browse your computer for the folder where the file is located.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810699766/b6ebb6db979831962adbd172679b/image+%281%29.png?expires=1776713400&signature=fa3777875dfd1e9136503a656cdfd6693cad5a0da74a3d4fe7e97abee0d15a35&req=dSgmFs93lIZZX%2FMW1HO4zV0D7C7eZi0c7%2B9P34g9G%2BiYv9QCUfmHPquqdW9p%0AleRLGf5SaOCaQMTuqDs%3D%0A)

## **Importing the Deposits File**

**Step 1:**

In the upper right corner, select **Assets** and then click on **Funds Overview**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810638815/c5980b215c62b919904d7f14c0a6/0d7d04b2-9736-4a7f-be62-a77e59ee90c4.png?expires=1776713400&signature=bd4c4b74a9d8ecd0f7a347952a31541621ede858b64ae0f760452f916498e718&req=dSgmFs99lYleXPMW1HO4za6WKMUrvBhMyNv%2FRfHkqc5PkmidHF0X3%2BVftXQS%0A%2FNFOxCFKZnAUt03eAzA%3D%0A)

**Step 2:**

In the menu on the left, select **Deposit/Withdrawals** and then click on **Deposit**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810640212/609d022eaf13b72976b71731eabd/f26fbaf6-e934-4431-bef0-58d91c41408a.png?expires=1776713400&signature=01daf329562b41b4e96bd9e422d84e7de17298829bcd93797fe5246420a603f2&req=dSgmFs96nYNeW%2FMW1HO4zdyI%2F2sul46qySPtS6Kurbs7A8NEmfr5IxgFJhNA%0AFN9gjHP7ytPT1tJe4dM%3D%0A)

**Step 3:**

In the **Deposit** tab, select the date range that includes your entire time you transacted on Gate and click in Download.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810642163/2a876bbd9ed7818205c43b944946/fc5970aa-e92d-468b-ba97-67478a87375d.png?expires=1776713400&signature=8a8be21c1ac6dbb8e8a81b4073d410e0382ad9e77e5c9ba9604d7f928915e265&req=dSgmFs96n4BZWvMW1HO4zXfQGAGAuyij%2F2jpGwLkQsY107JKEcbKtsh56jhb%0AZXO4TB0XpNPDjSmW5%2FU%3D%0A)

## **Importing the Withdrawals File**

**Step 1:**

In the upper right corner, select **Assets** and then click on **Funds Overview**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810663318/a188fbc56115233f82dc3036c544/7cf18455-0c97-4eb1-baa8-86c08cc726c6.png?expires=1776713400&signature=a1337197e372b62e12b5972d4e70fb9b2c148a79f279e477443f737430bf081f&req=dSgmFs94noJeUfMW1HO4zRZFBb24oTxEApo0IfsY0zVFjHA1ocuDb8JWH51i%0A0RKF4OFZQzsL8fVjgJo%3D%0A)

**Step 2:**

In the menu on the left, select **Deposit/Withdrawal** s.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810664816/c1e2401ca4395d32dac2eb77e5a9/406f153a-238b-4c68-a186-fd941f82a984.png?expires=1776713400&signature=2a75c579c2cb1f0d94036c3232d87ac474cf7abf3a22555038886e6e4f13c1d6&req=dSgmFs94mYleX%2FMW1HO4zfMg7m2qK4OyPnyrRH7AI0YOf7vrD%2FXNFXHN7kO9%0AQZqcJCOpVTmZyLghmok%3D%0A)

**Step 3:**

Switch tab to **Withdrawal**, select the date range that includes your entire time you transacted on Gate and click in Download.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1810666411/652f5eaacf5b2e4a1e6bd974f4d4/e0fde454-f15b-49b1-819d-5de2717b9019.png?expires=1776713400&signature=857771715c904c302d8aea1cd86fb23f81dc02fd33ef64b4a303115b86dc0cc5&req=dSgmFs94m4VeWPMW1HO4zWDm0VzgcJFmYkloRQ3DlKSQLCypIVx3SNE2g%2BDu%0AHWAtNuQRU0tqjl9kK5I%3D%0A)

### **Final Step: Import all 3 files into CoinLedger**

You will receive files in **.csv** format. Navigate to **Step 1. Import**. Select **Add Account** then choose the **Gate** tab on CoinLedger. Click on **Upload File** and drag each of your CSV files into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/503424050/0759631903d1a17c3e7e9ac9/Screenshot+2022-04-26+at+21.21.34.png?expires=1776713400&signature=60cb94e5841e2baefc20b4710cf59e275951247112a32658216bf89bd752c162&req=cSAkEst6nYRfFb4f3HP0gLh%2B8nGmGjeX8jyRXEOv%2FryUdUJO2QJrJ9ZQbr8y%0AjM6VwPMkKvSVes%2Fs8w%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

# **Gate Import Limitations**

- Due to limitations with Gate file export, if you have margin transactions they will appear as spot trades. This is because Gate does not distinguish between margin trades or spot trades on their official Trade History file. Please review these transactions prior to submitting your tax reports.

- If you use the POINT currency to pay for fees when trading on Gate, all your POINT fees will show up as USDT fees.

- Transactions from Gate's Earn program are not exported through any of their files nor through an API connection. If you had income from their Earn program, make sure you [enter them manually](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide) on our software.

- Fiat buys are exported as one-sided crypto deposits. Review the Deposits section below to learn how to fix it in-app.


​

Did this answer your question?

😞😐😃