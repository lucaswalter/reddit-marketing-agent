[Skip to main content](https://help.coinledger.io/en/articles/6588913-bybit-api-import-guide#main-content)

# Bybit - API Import Guide

How to automatically import your Bybit transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs **Read-Only** or **View** access to import your trade history. This permission does not give access to your private keys nor the ability to move your funds. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/6588913-bybit-api-import-guide#h_90ccd41132)

2. [Bybit API Limitations](https://help.coinledger.io/en/articles/6588913-bybit-api-import-guide#h_c7fa283975)


## API Import Walkthrough

**Step 1:**

Log into your [Bybit](https://www.bybit.com/en-US/login) account.

![](https://downloads.intercomcdn.com/i/o/586594239/02610c9be2983c51049111e3/image.png?expires=1776713400&signature=5ea58e1ac837d3ba6ae322aac2b9f04237d2dd66a0a4106c93d1920473f07a4d&req=cSghE8B6n4JWFb4f3HP0gEzMVj1mC9lPI%2BcmASV20o5P%2F6%2BDVIlrSEPhTS1E%0AbvWTCbPbRlOQJrRNGQ%3D%3D%0A)

**Step 2:**

Click on your profile on the menu in the upper right corner and then on **API**.

![](https://downloads.intercomcdn.com/i/o/894218229/3bd50e5cfe683158fc4a2acc/1.access-api-key-management.png?expires=1776713400&signature=893d42ed157695e29bcc748f1e1eedc68c265be2e606e7c4e82f8d61253b3df2&req=fCkjFMh2n4NWFb4f3HP0gEBPty9Kwv7Mnd16CZHB0njuJLWG1lYlpA%2FRCn2C%0A8AfXWnGXyVqCgIj%2Btg%3D%3D%0A)

**Step 3:**

Under **API Management** click the **Create New Key** button. Be sure to also select the correct Key Type, which is **System-Generated** API Keys.

![](https://downloads.intercomcdn.com/i/o/894218776/780f0bbb1a1d671b3e1da8d4/2.start-new-key-flow.png?expires=1776713400&signature=f6f06318944eec80095574c2cbd3e7f0136a1787c640bbde32d64acfd4dc8fdb&req=fCkjFMh2moZZFb4f3HP0gMP0AHAn5e6djQETKDO41krCJQuuaXV56I2mlJKg%0AVsKaFQINklq2RNJ2sA%3D%3D%0A)

​

![](https://downloads.intercomcdn.com/i/o/895144426/74b6659eb156e17c96379849/3.select-key-type.png?expires=1776713400&signature=185c4531785749f570af8f74a447c455c77e5c7a6c3398fe1b82ffc6ada2ed2e&req=fCkiF816mYNZFb4f3HP0gIUq7qFWj0VtiriwWPmCneoOaDq54mIXNVRUdmr6%0A4cI7dSNSUiAu%2B1EJ5A%3D%3D%0A)

**Step 4:**

Keep the **API Transaction** option selected. Give your key some name, select **Read-Only** under **API Key Permissions** and then select **No IP restriction.**

**NOTE:** you should copy these permissions **exactly as shown in the screenshots below.** This ensures that read-only permissions are given to CoinLedger.

![](https://downloads.intercomcdn.com/i/o/894219132/507c03b883f66eb0fe133565/4.1.define-key-values.png?expires=1776713400&signature=a0373fb67faa8fe2d8abf1a8defc422e488a85fffe2d342e32ea7176be931cf4&req=fCkjFMh3nIJdFb4f3HP0gDxbhDE3011t2%2Fco16y88gEvFK0%2BHmR8%2FJHQaqqn%0AYIqDHTPrBkE5vQVdCQ%3D%3D%0A)

Next, under the Trade column, select **Unified Trading**, and in the NFT row select **NFT products and transaction history**. Finally, check the **Assets box**, and then hit **Submit**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1421479797/2740f3de308b71a34dae0a1abe53/bybit_update.png?expires=1776713400&signature=5d52db0b9b91dadfc1e8fb8a4ebf3136032dfe3117c1efd3befb951cada885b6&req=dSQlF815lIZWXvMW1HO4zcc94%2BZ09IhcqWwhdqNwn2fZLjLFheDuAARZomje%0A%2FlYqFo1m%2FfN622pO9bc%3D%0A)

**Step 5:**

After clicking the **Submit** button, you need to enter your 2FA code and click **Confirm** to create the keys. If everything is correct, the window shown below should pop up.

The **API Secret** is accessible only while this window is available. Please store your **API Secret** somewhere safe to have access to it.

Copy all of the following keys and continue on to CoinLedger.

![](https://downloads.intercomcdn.com/i/o/894226846/7a4603c48b8bd9d1ec166e37/5.export-key-and-secret.png?expires=1776713400&signature=0fe2a6eb28debe2ac15af321332a9ff668e39f37764a93aa6aabdbeb2e136454&req=fCkjFMt4lYVZFb4f3HP0gLTi7lOK5sFFAW74cKTbTNW%2FB%2BRbdnJcOLPEchvB%0Ab6DgR%2FMUWhLLBCxenQ%3D%3D%0A)

**Step 6:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Bybit** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/593860793/e4a6ffd9e7fb0d610b65d344/Screenshot+2022-10-07+at+12.05.51.png?expires=1776713400&signature=2959105e0a39e88505aa03b242c274a43d0ac304941b809faa968951a5af3084&req=cSkkHs9%2BmohcFb4f3HP0gA5e5kWMIKHHGcibOn%2F0BffontJlMwmMgRmsZD0e%0AmBjjVrQ6eMhRbE%2BP6w%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Bybit API Limitations

CoinLedger currently does not support derivatives trading. If you've participated in derivatives trades on Bybit, these types of transactions may fail to import.

Additionally, if you have subaccounts, create an API key for each of those accounts and import them into CoinLedger one by one. The API keys created will automatically expire after 3 months. You will need to create new API keys after this period to sync new transactions.

Did this answer your question?

😞😐😃