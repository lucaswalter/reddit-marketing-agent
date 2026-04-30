[Skip to main content](https://help.coinledger.io/en/articles/2535271-poloniex-file-import-guide#main-content)

# Poloniex - File Import Guide

How to import your Poloniex trading history into CoinLedger

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 11 months ago

CoinLedger only supports automatic imports of margin transactionsfrom Kraken, with support for margin trades on additional exchanges going live in the future. In the meantime, you can import leveraged buys and sells from any exchange into CoinLedger manually using the **Add Transaction** button on the Transactions page. Find step-by-step instructions for this process [here.](https://help.coinledger.io/en/articles/9505113-how-can-i-import-my-margin-transactions-into-coinledger#h_f5df514af0)

**Step 1:**

​ [Login To Your Poloniex Account](https://poloniex.com/login)

**Step 2:**

Select **Activity** in the upper-right corner.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550079186/0a02098d55e493a0ec376f7bc740/step+2.png?expires=1776713400&signature=a4791e2a7dc308fcd3e2ea5a9621ed6857524a7b51241fe8fe6230a728db3925&req=dSUiFsl5lIBXX%2FMW1HO4zYAS%2FReYRS3IOlC4BXcaGg4fwILNS9XOVEgucu9t%0AzgRXKi5cFOg%2FyKNLEyM%3D%0A)

**Step 3:**

Then, click **Export**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550079074/5e902296a9438f8f106752eea797/step+3.png?expires=1776713400&signature=d783e93a182b41fba2f87a036b68d686153a33794967f2cc7330be4e1cc2af49&req=dSUiFsl5lIFYXfMW1HO4zasREKHEMGK%2F14L%2B38PxPIozxZl8f4ogS639kAZt%0ADLmeuYd2Y5sttHLZcig%3D%0A)

**Step 4:**

Next, you will generate your Deposit and Withdrawal files. You will need to export each separately. Under Type, select "Deposit" or "Withdraw," and under Time Range select a date range that captures as much of your transaction history as possible.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550082313/ed507762d85d8677364b1b155a29/step+4b.png?expires=1776713400&signature=b18a59d9e7dcfe9b0173c8c8904641c866a65ed46003308c27b195a8383eac19&req=dSUiFsl2n4JeWvMW1HO4zQ6NAkPAX9%2Bmh8tvxIEtp7kJXJTXE9QWY7%2FUH7C4%0A71gF3E%2FvPJZ8vgAAYNo%3D%0A)

After that, press **Download**.

You may have to export multiple files to capture all of your history. Please make sure dates do not overlap to avoid duplicate transactions.

Step 5

Next, you will need to generate your Trade History file. On the menu on the left side of your screen, navigate to the **Spot** section. Then, click on the **Trade History** tab.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550102579/b6bd692cc87a40f9cc6e66aff42b/Step+5+a.png?expires=1776713400&signature=72c8f94a30fc07e9deb7da7b066f0f0bbb153183505f74415ef69291b27f5882&req=dSUiFsh%2Bn4RYUPMW1HO4zUX1xxVRlHfua0T2AJFP5vthWw6nq8WbQLsKREvC%0A%2B3vFXCsJtGMCAYu4x5E%3D%0A)

Select the **Trade History** option, and click **Export**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550103392/a70c72f787bd942dca7d231def90/Step+5+b.png?expires=1776713400&signature=9191dd8a6ba49c5b0a15cbc6a78a15aa603bb9fd623a38420c44b74a4aea2def&req=dSUiFsh%2BnoJWW%2FMW1HO4zXTeMErD5yLGrXL9pfnVgJNr%2BUG5%2FenGDkQI43aS%0Ar7ayQvYHr8doa46KGDo%3D%0A)

As for your date range, make sure to select one that captures as much of your transaction history as possible. You can edit this by clicking the **1 year (custom)** option on the menu shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1550104709/a72e61cfe4705ecb52fcea3aa88f/step+5c.png?expires=1776713400&signature=bd883f6d1326d603bb38af5b0846282209af290928dfe4024b0a45acf2b33910&req=dSUiFsh%2BmYZfUPMW1HO4zRRyYrgBWlIu4oN5rBOgYTYDtP4vW41UUVXwc1D6%0ApXS3F9RRNUB8NkO8Smo%3D%0A)

Finally, press **Generate** and then **Download** to export your file.

DO NOT open the file in Excel and "save as" a new file.

It's important to upload the raw file that Poloniex exports straight from your "Downloads" folder. This avoids rounding errors and corrupting the file. If you need to edit your CSV, please use Google Sheets.

**Step 6:**

You will receive a file in **.csv** format. Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Poloniex** tab on CoinLedger. Click on _Upload File_ and drag each of your **CSV** files into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/503432144/481c9c0316c4b7d3256c9425/Screenshot+2022-04-26+at+21.36.11.png?expires=1776713400&signature=8293feb351e460533dd3921bda325da4d4729f8ade1bc03eb050acea90b3f24e&req=cSAkEsp8nIVbFb4f3HP0gAQufRoYWS4OswoLIP58ipAuQ4HA515%2B%2BTiiLNzC%0ALRwk0lDC08Co%2Bq9eyw%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

​

Did this answer your question?

😞😐😃