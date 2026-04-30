[Skip to main content](https://help.coinledger.io/en/articles/5042261-binance-com-file-import-guide#main-content)

# Binance.com - File Import Guide

How to import your Binance transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over a year ago

Jump ahead with this table of contents:

1. [File Import Walkthrough](https://help.coinledger.io/en/articles/5042261-binance-com-file-import-guide#h_77c737be03)

2. [Binance Import Limitations](https://help.coinledger.io/en/articles/5042261-binance-com-file-import-guide#h_2ffc71408b)


Binance File Import Walkthrough

## File Import Walkthrough

**Step 1:**

​ [Log in To Your Binance Account](https://accounts.binance.com/en/login?return_to=aHR0cHM6Ly93d3cuYmluYW5jZS5jb20vZW4=)

**Step 2:**

Navigate to the **Orders** page by selecting your Profile icon, then navigating to Orders on the dropdown menu. Then, head to the **Spot Order** section on the left side of your screen.

Next, hit **Trade History.**

Finally, select the **Export Recent Trade History** button:

![](https://downloads.intercomcdn.com/i/o/1121500722/6cd7d4d414cafcc7c0ad5f92/image.png?expires=1776713400&signature=61b10255a260fd02691782ba63419dda81d341066015ea6203d205ed2001fc46&req=dSElF8x%2BnYZdW%2FMW1HO4zZYOxZB89M%2FitT1w0zkvTE25BEzWOY9sEhm6CAMl%0ARnmCruNI%2B9lf98uNUJE%3D%0A)

_Note: Make sure **Spot Order History** is selected. Binance offers lots of file types, but it is the **Spot Order History** file that should be exported._

**Step 3:**

The max range for file exports on Binance is 12 months (1 year). Export as many files as needed to cover the full date range of your transaction history on Binance.

![](https://downloads.intercomcdn.com/i/o/1121503719/409f8c8167857f99d49fddb5/image+%281%29.png?expires=1776713400&signature=13f9cc1b27f1cd707f5c74b605b3b691de8bcc0fa6ee091d44efc80401f70f10&req=dSElF8x%2BnoZeUPMW1HO4zc26BBnzCDcaQUEnr9qgUkYW%2FvIhrOaPYISAHLug%0Aa7dGtN7qrTMDFtH%2BUDk%3D%0A)

**Step 4:**

You will receive files in **.csv** format. Navigate to **Step 1. Import**. Select **Add Account** then choose the **Binance** tab on CoinLedger. Click on **Upload File** and drag each of your **CSV** files into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/503541953/eb244ab4c5ba3a2e9d45c7e2/Screen+Shot+2022-04-26+at+8.40.01+PM.png?expires=1776713400&signature=282496ffd35919b7a6ea91c22fa97a041b57b58dac790859a5610dee0b010850&req=cSAkE81%2FlIRcFb4f3HP0gKsOG1aO4u%2F700%2FTSxwoJZIn5SrNAn9oaneQ7NlO%0Ac9Qks1TknK08GgHQdQ%3D%3D%0A)

_Note: It's important not to open the file before you import it as Excel can cause formatting changes to the file that prevent it from importing._

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

## Binance Import Limitations

The Binance Trade History file import **only** pulls in spot trading activity from your Binance account. This file does not include crypto purchases made directly from a **debit card**, **credit card**, or **bank account (ACH)** or **distributions like staking or mining rewards.** If this limitation effects you, switch to [Binance API import](https://help.cryptotrader.tax/en/articles/2757038-binance-com-api-import-guide) or add these transactions manually.

Did this answer your question?

😞😐😃