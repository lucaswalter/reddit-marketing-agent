[Skip to main content](https://help.coinledger.io/en/articles/5091142-coinex-file-import-guide#main-content)

# CoinEx - File Import Guide

How to import your CoinEx trades in CoinLedger

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over a year ago

**Step 1:**

Log in to your [CoinEx account.](https://www.coinex.com/signin?redirect=%2F)

**Step 2:**

Navigate to the [Asset History](https://www.coinex.com/asset/history/spot) page under the Assets tab. Select for **All** and then **Export**.

![](https://downloads.intercomcdn.com/i/o/606126335/52a4a5b0e0d2e9b02c66c1f7/Capture.png?expires=1776713400&signature=b072a4c1ea4884708651dba5d35a8dc4aaff794a8a4462841004078c89a8593c&req=ciAhF8t4noJaFb4f3HP0gOQQwywoF7bFpbe1nDb%2FAEbmF0mCyp0zGuA7TsyT%0A23%2FNMF%2FxTEU9TXv1Zw%3D%3D%0A)

**Step 3:**

You will receive a balance history file in **.xlsx** format. Navigate to **Step 1. Import**. Select _Add Account_ then choose the **CoinEx** tab on CoinLedger Click on _Upload File_ and drag your **XLSX** file into the box to import your transactions.

_Note: Import the file without opening or editing it. Opening the file in Excel may apply formatting changes that will cause import failure._

![](https://downloads.intercomcdn.com/i/o/503419867/2987abb7d220e91089362f07/Screenshot+2022-04-26+at+21.14.12.png?expires=1776713400&signature=815cfa645ae15ae468acdce972e66be0a9dc45bf59a78eaf1ee9576c898fe42e&req=cSAkEsh3lYdYFb4f3HP0gPXXk%2FZbJjJVq9sj9QZFtj9fcbm2Ve8wE1o4kExp%0A99Kbt0CfVoApXsQlGg%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

**NOTE:** CoinEx does not export complete transaction data for fiat purchases made on exchange (buying crypto with fiat currency.) The CoinEx file export only includes the crypto amount received and does not include the fiat amount spent. As a result, CoinLedger imports these transactions as deposits (non-taxable self-transfers). Refer to [this guide](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-transaction-to-fix-incomplete-data-exported-by-a-crypto-exchange) for instructions for how to edit the Deposit transaction and change it to a Fiat Buy.

Did this answer your question?

😞😐😃