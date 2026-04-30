[Skip to main content](https://help.coinledger.io/en/articles/6201854-coinspot-api-import-guide#main-content)

# CoinSpot - API Import Guide

How to automatically import your CoinSpot transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/6201854-coinspot-api-import-guide#h_29185d3eef)

2. [CoinSpot API Limitations](https://help.coinledger.io/en/articles/6201854-coinspot-api-import-guide#h_038df6a1f2)


How to Calculate CoinSpot Taxes (FAST) \| CoinLedger - YouTube

Tap to unmute

[How to Calculate CoinSpot Taxes (FAST) \| CoinLedger](https://www.youtube.com/watch?v=B7PoWw0aNRA) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

## API Import Walkthrough

**Step 1:**

Log in to your [CoinSpot](https://www.coinspot.com.au/login) account

![](https://downloads.intercomcdn.com/i/o/509837397/c014bda14e0c54be1d34ffdc/image.png?expires=1776713400&signature=c71bf5a4d9c4e2023cbf863fe02e6c15eda8231df1a65f5dd7aff78f88466c7a&req=cSAuHsp5nohYFb4f3HP0gEDuJQza3ocO1rtwF6ScU0O2nLO%2FnZpZNsZ3tADA%0A2aEMDQj3JFBTIlFpkQ%3D%3D%0A)

**Step 2:**

- Navigate to the **[API](https://www.coinspot.com.au/my/api)** section

- Click on the **My Account** icon in the top right corner and select **API**


![](https://downloads.intercomcdn.com/i/o/900514450/90064751e742a54ff05d0980/Screenshot+2023-12-04+at+12.16.27%E2%80%AFPM.png?expires=1776713400&signature=60478f0bc7c2f9a4ee6dfe003e3b1f05737b059fc8ddb85a602ff278645a9ae7&req=fSAnE8h6mYRfFb4f3HP0gOpHSAA1crt5wo2cRnp2%2BISJQJ04DWbyOUXm%2FqHa%0A6y5VNOZjNt33NDItSA%3D%3D%0A)

**Step 3:**

Click on **Generate New API Key**

![](https://downloads.intercomcdn.com/i/o/509838175/cee69db6accb748a505956d7/image.png?expires=1776713400&signature=288d0e719386420d2d1c841ca87a068ca4602d40049b2f4571d4ccd77f7f295c&req=cSAuHsp2nIZaFb4f3HP0gLPaP3khUESg74czbFLC%2BklCFhF99LrqUk%2BeVV95%0AZFuLJA1Zt2tzUJabMg%3D%3D%0A)

- Select a name (this can be any name you'd like) for the API key, make sure **Read Only** is selected for API Key Type and enter your 2FA code

- Click **Create API Key**


**Step 4:**

Click on the confirmation link received by **e-mail.** You should receive an e-mail from CoinSpot asking to confirm the new API key creation, click on the received link to proceed.

**Step 5:**

Copy the secret into a safe place. Click **View Secret (One Time Only)** and copy the secret into a safe place, as you will not be able to recover it later.

![](https://downloads.intercomcdn.com/i/o/509840352/908a5098b13f04c1d84cf5ab/APIKeysCoinspot.png?expires=1776713400&signature=8b4e1f6be6b8f4343d5f5b84e3372db8b0c0f3e10d9cd166fa57e6f8c3e6c27a&req=cSAuHs1%2BnoRdFb4f3HP0gNcmpyy9ScfP6IqZRWiRsNYggu6qTzCvCpJNhGlx%0AmxySUBZ4lhM7zWPxXw%3D%3D%0A)

**Step 6:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **CoinSpot** tab on CoinLedger. Click on _Auto-Import_ then enter your API Key and API Secret into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/509841221/0283334f6b239cf148030268/Screenshot+2022-05-09+at+12.30.05.png?expires=1776713400&signature=fcfc81d436974fc924f4d8c658550d05553c1b7d7b8987b5879c2bf3dd0a7c51&req=cSAuHs1%2Fn4NeFb4f3HP0gO4BkgfaO%2Bk0WeG1eMzZb6CsKK7%2FB3w2PBTfvfbi%0AeGuBaCzrQUj5%2BsI%2Bkw%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## CoinSpot API Limitations:

These transaction types are not returned by CoinSpot's API:

- [Bundle trades](https://www.coinspot.com.au/bundles)

- NFT Transactions


Additionally, CoinSpot's API may not return timestamps for certain trades, which can cause the import to fail. This issue is actively being worked on by the exchange.

​

Did this answer your question?

😞😐😃