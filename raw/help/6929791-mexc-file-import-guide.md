[Skip to main content](https://help.coinledger.io/en/articles/6929791-mexc-file-import-guide#main-content)

# MEXC - File Import Guide

How to import your MEXC transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

**Important Note:** MEXC does not export a complete transaction history file that includes all transaction types. Instead, MEXC exports a few different file types: **Withdrawals**, **Deposits**, and **Trades**. Each of these files contains completely separate transactions.

For this reason, it is very important to carefully review all transaction types that you had on MEXC and then export each file that contains these transaction types. This guide includes descriptions of the data included in each file as well as step-by-step instructions for importing each file into CoinLedger.

**Step 1:**

Log in to your [MEXC](https://www.mexc.com/login) account.

![](https://downloads.intercomcdn.com/i/o/659100247/050a411f707d61ff28429b60/image.png?expires=1776713400&signature=ef59883b0e46ac20ed51aff2b61902b6300a368bfae40af1fc97bf82caa7b90e&req=ciUuF8l%2Bn4VYFb4f3HP0gHHCAAA6n8Fdpr5ZVbCV5OL42FLNGcLkjPhWhcVG%0A53%2Bl81E32bv5j342Aw%3D%3D%0A)

**Step 2:**

Navigate to **Spot Orders** from the dropdown menu.

![](https://downloads.intercomcdn.com/i/o/969951433/727d47f423902a00c904d59a/Screenshot+2024-02-21+at+11_30_21%E2%80%AFAM.png?expires=1776713400&signature=37fc6ee1e601e0d9e7a275ed2bda7a1d70d5a8ca0d723427f11fcb1e80a75b2a&req=fSYuH8x%2FmYJcFb4f3HP0gL3QNZAoYX1nm0XpxJWiFXxEhET89gB60qaqtqaV%0AglRwBkLHrJFkj74Eww%3D%3D%0A)

**Step 3:**

Select the **Trade History** tab and click on **Export Trade History.**

![](https://downloads.intercomcdn.com/i/o/969951722/21d82a62b092e75fc937aa5c/Screenshot+2024-02-21+at+11_31_09%E2%80%AFAM.png?expires=1776713400&signature=16340b96eaa9fa20fac90ac62242972f057b976f3acfa635f1da912a468e6e38&req=fSYuH8x%2FmoNdFb4f3HP0gJjZJicaWmBrtKaCPJzmLxMENVVQ13SfM3QfTC0U%0AMv9SJQ%2BF5O7JlFjsVQ%3D%3D%0A)

**Step 4:**

Leave **Trading Pair** and **Side** set to **All** and select a time frame that contains all of your trades. Then, select **Excel** on **Format** check-box and click on Generate.

(Note: MEXC limits users to only generating files in one-year increments, meaning **you can only select up to 365 days at a time on the menu shown below**. Make sure you generate a file for each year of your trading history on MEXC). Once the file is generated, select **Download.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1365045888/2a43c00a6910d16035b55286811a/image-20250203-180709.png?expires=1776713400&signature=d701c0c2f2082ea0b99a955969a62a6251eabe6e469fa78522c42cbd789f2201&req=dSMhE8l6mIlXUfMW1HO4zanCkB6CH%2Bss%2F35LTPrVwOkRyKBwSS%2BM9e2%2FMOO%2F%0AKhxXayx9or90bm%2B24OQ%3D%0A)

**Step 5:**

In the **Wallets** dropdown menu, select **Funding History.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1365048201/d64e716c1ae77b0083dfca824fdb/image-20250203-180933.png?expires=1776713400&signature=63684d35453c16fed330493df060c7160abe4eba43109423b4e6b6e83b5409e3&req=dSMhE8l6lYNfWPMW1HO4zWCEgQlXEK8xWkGR47Yn%2FUTWG6CDmh5sI6wyDHhO%0AICfVCNSrjoHlZtl3AoQ%3D%0A)

**Step 6:**

Click on **Export** next to the Refresh button.

![](https://downloads.intercomcdn.com/i/o/969953502/3728f0824d0f7de39902fea5/Screenshot+2024-02-21+at+11_33_43%E2%80%AFAM.png?expires=1776713400&signature=594ad11de973882a6e603749ef9c1979cefe95e49a562ccd11bd6d4b61885ae3&req=fSYuH8x9mIFdFb4f3HP0gMcD68aB1aaN6DsgpG2n%2FRYKQl2BA%2BfbMlGGpU7B%0A5u9nEvQXLOo6k%2FTJOw%3D%3D%0A)

**Step 7:**

With **Type** being set to **Deposit**, select a time frame containing all of your transactions and click on **Generate**. Repeat the same process, with the **Type** being **Withdraw** this time. **Download and export** both files.

![](https://downloads.intercomcdn.com/i/o/659110597/0a12ff8558c8772bb33ea72d/image.png?expires=1776713400&signature=4d33033ac2d4c7d022962cdfdee26261375014c39abbefa394910d26301d9867&req=ciUuF8h%2BmIhYFb4f3HP0gBm81hHBh19wF6lLWtKS%2FSRZi%2B0XPUnWfEL%2BYa9B%0AFG5huH%2BoL16KVDaIuQ%3D%3D%0A)

**NOTE:** Please make sure you **DO NOT select** _Encrypt the file_ at this stage. If you encrypt the file with password protection, it WILL fail to import into CoinLedger. Please make sure you **deselect/uncheck "Encrypt the file"** for both the Deposit and Withdrawal files that you generate, as shown below.

![](https://downloads.intercomcdn.com/i/o/969967261/13839b512589bf1453a2f6d0/Screenshot+2024-02-21+at+12_30_23%E2%80%AFPM.png?expires=1776713400&signature=ae33a05189dfed0de65754fc00ada621204cfb3dcb31e4bc5e28da02b5d94489&req=fSYuH895n4deFb4f3HP0gPlxzDmdcGc7L2gsHct5MFbfH5nAWw1YHV4Uwkr3%0ASChHtjks0JP1985U9w%3D%3D%0A)

​ **Step 8:**

Open the **CoinLedger** app and navigate to **Step 1. Import**. Select _Add Account_ then choose the **MEXC** tab. Click on _Upload File_ and drag your Trade, Deposit & Withdrawal History **XLS** files into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/674314587/fac2870979669c1732e95d4e/image.png?expires=1776713400&signature=f5cf0022c7b7a2cb5c0a53c7787e7c7c3142f8f89c56da622c5bc977189fdb2a&req=cicjFch6mIlYFb4f3HP0gMVwUF4HCbw4NWQa8IgkJiU%2FvQ93jAkeC5ET%2BDsq%0AOQsrgGh1kN%2FT4TWXfQ%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

​

Did this answer your question?

😞😐😃