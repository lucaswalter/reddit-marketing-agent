[Skip to main content](https://help.coinledger.io/en/articles/5338231-kraken-ledgers-file-import-guide#main-content)

# Kraken - Ledgers File Import Guide

How to import your Kraken ledgers history into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

You can import your transactions from Kraken into CoinLedger by following the process below. Read on for more instructions on importing your Kraken transactions using their Ledgers CSV.

**_Please note:_** CoinLedger currently only supports importing margin transactions from Kraken through [Kraken's API import method](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide). Importing margin transactions through Kraken's CSV files into CoinLedger is not possible at this time.

Kraken File Import Walkthrough

**Step 1:**

​ [Login To Your Kraken Account](https://pro.kraken.com/app/history/export). Please ensure you are using the _Kraken Pro_ layout (you can select the grid icon as shown below and then select Kraken Pro).

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463335430/aa007870c69355188d967bbd03bd/Screenshot+2025-04-07+at+1_08_09%E2%80%AFPM.png?expires=1776713400&signature=26aa6a04d465853074761f526e03951e65c5ec434a573e8db3b8c4ff3cbe996f&req=dSQhFcp9mIVcWfMW1HO4zYWFV4Cwd33AIvrpl81QO0P0e3gwOiunxvKdbm1I%0AHcmYi1Is1cn5lXUNaT8%3D%0A)

**Step 2:**

Then, select the profile icon in the top right corner of the screen and select **Settings**. You can access this page directly using this link: [Kraken Settings](https://pro.kraken.com/app/settings/account).

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463338704/0e254280f8b1505b4cc5b13a37bb/Screenshot+2025-04-07+at+1_09_40%E2%80%AFPM.png?expires=1776713400&signature=a17e6839c2322333b49f16aa3fed00403db740fe89ea4c85a61e2a69e92e4c6a&req=dSQhFcp9lYZfXfMW1HO4zUl%2Fu5vJ2yN3jxLK7k5V2D36sgOmP4aqCLW7kyzA%0AnWbzmOlZj4owYY6%2FZLc%3D%0A)

**Step 3:**

Next, click on the **Documents tab** at the top of the page. Then, press **Create export.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463341940/ffb3debdf01bfad3ac8651ff22a6/Screenshot+2025-04-07+at+1_11_44%E2%80%AFPM.png?expires=1776713400&signature=730204ebd3105959694f7564b7f2c7a3bf8be146c60207727f20158d0d4a73c8&req=dSQhFcp6nIhbWfMW1HO4zSvThnkND8gqcQ%2BTO8eXGyd0dInOwnp%2Fij0%2BDg71%0Ahy%2BLXe6St7%2BReucniqU%3D%0A)

Finally, on the Create export menu select **LEDGER**. Please do not select any of the other export options.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463343635/bade3403b352b7ea10ca468b9221/image.png?expires=1776713400&signature=645b12956532b8bdf304c0aba1cccab5b9cd425f20b8a0ae68b0d1d57be6e2aa&req=dSQhFcp6nodcXPMW1HO4zavNNoS9fXS1nBmrqWOMoOkTGQgrCZcyiERvwXKh%0AhcfNIJh%2FrMEI4V9w7BU%3D%0A)

**Step 4:**

On the next menu you will be prompted to select the type of file you'd like to export. Under **Start and end date**, set your **date range** to as _wide of a date range as possible_ to ensure CoinLedger has your full transaction history.

Next, under Transaction types please select ALL other transaction types **_EXCEPT for_**:

- Margin trade

- Margin rollover

- Margin settle

- Margin conversion

- Margin interest


You can do this by selecting All, and then deselecting these margin-related transaction types.

Selecting these margin transaction types may cause your import to fail. If you'd like to import your margin transactions into CoinLedger, we recommend switching to [Kraken's API import method](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide) instead.

Under **Assets** and **Fields**, leave **All** selected. Finally, under **Format** select **CSV**. Then, press **Generate**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463357397/ea25498e746dbf7840158daec9b4/image.png?expires=1776713400&signature=37840001f7574c072ad79b63b41e083b7e36683df597e29cf17cb6d93686849d&req=dSQhFcp7moJWXvMW1HO4zV5XO7JGSMET8WU%2BVASDY0U5KLurhXgtIvWZH5Tx%0AesDwWBUM23Rx%2BEC17og%3D%0A)

​​ **Step 5:**

Download the zip file Kraken provides you. Finally, unzip that file so you have the **ledgers.csv** that is inside.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1463362405/999f1dfd0ad2fffa0d11225ce1ed/Screenshot+2025-04-07+at+1_23_39%E2%80%AFPM.png?expires=1776713400&signature=e354b128277df4dc47c475d4a35e75063ed5e4b81d78f630dc81794360e887df&req=dSQhFcp4n4VfXPMW1HO4zbUTPoYj4SQti%2FG1R35eEfFqLdSAMB3n6NO2jzOw%0A%2Bw%2BF%2B6TyVUOw1atZb50%3D%0A)

​ **Step 6:**

You will have a file in **.csv** format after extracting the .zip file. Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Kraken** tab on CoinLedger. Click on _Upload File_ and drag your **CSV** file into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/916591615/954dbbaaf985347374401ab2/image.png?expires=1776713400&signature=4deb7fc8d38d058d64b28b2d67a2974500e4724aae3dd53cf3d70cd358bfe0e1&req=fSEhE8B%2Fm4BaFb4f3HP0gBe3of9WyLHyXquOAN0ZSGcVHbzq4wM0Lj2LSjLl%0ATC7LmrprA49CJTQfxg%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

​

Did this answer your question?

😞😐😃