[Skip to main content](https://help.coinledger.io/en/articles/3620033-bitrue-file-import-guide#main-content)

# Bitrue - File Import Guide

How to import your Bitrue transaction history into CoinLedger

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over a year ago

Learn how to import your Bitrue transactions using their transaction history file by following the steps below! To automatically import your Bitrue transactions using their API, please [check out this guide](https://help.coinledger.io/en/articles/9519226-bitrue-api-import-guide).

# Step-by-Step Import Instructions

**Step 1:**

Login to your [Bitrue](https://www.bitrue.com/user/login?callBackPath=/) account.

**Step 2:**

Click **Assets** and then **Overview** from the top navigation bar.

![](https://downloads.intercomcdn.com/i/o/666740922/58698543d2d1782e93556ec2/Screenshot_10.png?expires=1776713400&signature=050973a64a864b450cefc19c71ecd7d0df055572fd46fd5aa6b2b363882f530b&req=ciYhEc1%2BlINdFb4f3HP0gDIyIkhK653xwoQ5K2QGUdkRvNNCFvvZYgKojk7n%0A9oW%2BjM4aPwGUW6MIiA%3D%3D%0A)

**Step 3:**

Click on the **Export Transaction History** button and use the following options.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1333534734/1c4df2998f89bc2014ddfb063a01/Screenshot+2025-01-13+at+6_10_10%E2%80%AFPM.png?expires=1776713400&signature=2d9c85ba68f9d83a2227d84d36e02a9d2d747ceae07dd8e602a4f432c2729b54&req=dSMkFcx9mYZcXfMW1HO4zbNK8t0PqH%2F4IzN4CyDBfof%2BvxnqaPYXyjjzLwXN%0A5O%2F00u3EYkwzZA1kLPo%3D%0A)

On the following pop-up menu, select a date range that covers as much of your transaction history as possible. You can do this by selecting customized and then specifying a custom date range for your file. Bitrue allows you to generate custom files in one year increments. Transactions from January 2022 and later can be downloaded via this method. You may need to export multiple files to ensure you capture your entire transaction history.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1333540433/065604e2c17eaedccd9fab8ffa08/image.png?expires=1776713400&signature=d7f8e9fe1eb3510edf40385d783abf4985227a88968cb8a62abbefbf4b30845a&req=dSMkFcx6nYVcWvMW1HO4zf665HnOa712YsYbB8mkaC8ykekh6vVavxoQMbAT%0Aj3kxyAxeDssYHKQufuc%3D%0A)

Under both **Account** and **Coin Type**, select **All**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1333537050/276da35e6e9f63853b1895906472/Screenshot+2025-01-13+at+6_12_58%E2%80%AFPM.png?expires=1776713400&signature=0feff5d6899cb1b9cb97637f3171c0878c0eaac90c7c266ae0b0c7878f4b2dab&req=dSMkFcx9moFaWfMW1HO4zR%2BXrKYoxdgsg27UdVKaOU7LOMoZYioJLPUF8hlP%0A0sWhWDvaliDHT7AMXao%3D%0A)

Finally, press **Generate**. You will receive an email notification once the files are ready to download.

**Step 4:**

You will receive files in CSVformat. Within CoinLedger navigate to **Import**. Select **Add Account** then choose the **Bitrue** tab on CoinLedger. Click on **Upload File** and drag each of your CSV files into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/503542504/a26bf56713198046a6d72d9e/Screen+Shot+2022-04-26+at+8.42.51+PM.png?expires=1776713400&signature=347b3279a01b77110a156b2a7dc614a7eb9ae912fb31d4c953280a626f6621bc&req=cSAkE818mIFbFb4f3HP0gNqHxlGf3EDZWF4mARdNnsXTRhT%2Ba5Gzeik9khQT%0A3hJpQvddEsnra2GK7g%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

**NOTE:** Bitrue does not export complete transaction data for fiat purchases made on exchange (buying crypto with fiat currency.) The Transaction History file only includes the crypto amount received and does not include the fiat amount spent. As a result, CoinLedger imports these transactions as deposits (non-taxable self-transfers). Refer to [this guide](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-transaction-to-fix-incomplete-data-exported-by-a-crypto-exchange) for instructions for how to edit the Deposit transaction and change it to a Fiat Buy.

Did this answer your question?

😞😐😃