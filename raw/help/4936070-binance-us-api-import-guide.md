[Skip to main content](https://help.coinledger.io/en/articles/4936070-binance-us-api-import-guide#main-content)

# Binance.US - API Import Guide

How to automatically import your Binance.US transaction history into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs **Read-Only** or **View** access to import your trade history. This permission does not give access to your private keys nor the ability to move your funds. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/4936070-binance-us-api-import-guide#h_cf947f14ae)

2. [Binance.US API Limitations](https://help.coinledger.io/en/articles/4936070-binance-us-api-import-guide#h_185f4818b3)


Binance.US API Import Walkthrough

Copy link

[Open video in Loom](https://www.loom.com/share/bbe7b63ccfc04737aa731d0f1a21a190)

0

1.2×

1 min 2 sec⚡️1 min 17 sec1 min 2 sec51 sec41 sec36 sec31 sec24 sec

![](https://cdn.loom.com/sessions/thumbnails/bbe7b63ccfc04737aa731d0f1a21a190-00001.jpg)

Copy link

[Open video in Loom](https://www.loom.com/share/bbe7b63ccfc04737aa731d0f1a21a190)

0

1.2×

1 min 2 sec⚡️1 min 17 sec1 min 2 sec51 sec41 sec36 sec31 sec24 sec

## API Import Walkthrough

**Step 1:**

​ [Login](https://www.binance.us/en/login) to your Binance.US account.

**Step 2:**

Select your profile icon in the top right corner, and select **API Management** from the dropdown menu.

![](https://downloads.intercomcdn.com/i/o/1115217608/5210b37c5c2c35018d35ca81/Screenshot+2024-07-16+at+9_53_23%E2%80%AFAM.png?expires=1776713400&signature=0a4b78b41cdb249d9b5a8d1f7f40c131350ec6e3608e211b249b24ed8d7877a4&req=dSEmE8t%2FmodfUfMW1HO4zUXYLMgPMf9dsS9L53JQW%2FKvW8MhjZx0EUqpDBvD%0AoKNAxx8VvvIP%2FweLAnw%3D%0A)

**Step 3:**

Enter a label for your key, and click **Create**. ( _The label can be anything you choose._)

![](https://downloads.intercomcdn.com/i/o/1115217934/de6c3b613db7d0f0fcffa444/Screenshot+2024-07-16+at+9_55_54%E2%80%AFAM.png?expires=1776713400&signature=7ecc6d556280192e10eec54511529eeaf48dcf69df8c60474593911dc4e89833&req=dSEmE8t%2FmohcXfMW1HO4zQ0zadQjhSl39p4z37OT0I9dbzEv0Ujn36PNcOZb%0AV6XcazTg5KJIWX7RI%2Bo%3D%0A)

**Step 4:**

Enter the security verification information sent to your 2FA device.

![](https://downloads.intercomcdn.com/i/o/1115218133/0fa1bfda2171fa1b045e273c/Screenshot+2024-07-16+at+9_56_12%E2%80%AFAM.png?expires=1776713400&signature=96f7753b53ee37dc5d25ab44ecaa8e42597424c3db8deb3fa5ca89dab5931fb7&req=dSEmE8t%2FlYBcWvMW1HO4zZ6kWR74JZfMZdr2auH8sRZwefnCi8c9EYOLbtR5%0A9WSTv5Kb6YGqC%2FnHzbM%3D%0A)

**Step 5:**

You will now have a new API Key and Secret created under the **Exchange API List** section. **Please do NOT select any API Keys from the Tax API section,** as these API credentials will not import into CoinLedger.

Copy the **API Key** and **API Secret** values as they will be needed for later.

**Step 6:**

Update your API permissions to ONLY check the **Enable Read** box:

![](https://downloads.intercomcdn.com/i/o/1115218759/82b4342d0fcb978838c673b3/Screenshot+2024-07-16+at+9_56_52%E2%80%AFAM.png?expires=1776713400&signature=f16e7eb54e075580e7b0235384acbebb61e3f837d54016fa0fd75573a727c846&req=dSEmE8t%2FlYZaUPMW1HO4zdzJdGLdXX8V0umoevvwbSTpAedSBDsP0PQrGdhC%0AroiP8leIaO7SmFO6Jsc%3D%0A)

**_Important Note: Leave the IP address restrictions field with the default value. The API Key will not work without this._**

Finally, **please do NOT select any API Keys from the Tax API section,** as these API credentials will not import into CoinLedger.

**Step 7:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Binance US** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/1115221344/a564b72a3b73a03e1003b97e/Screenshot+2024-07-16+at+9_59_15%E2%80%AFAM.png?expires=1776713400&signature=62c8e3fb6be3fba9bc03c71aeaa07378426c6cdcd5f8969c8c95ed483fe4ff7d&req=dSEmE8t8nIJbXfMW1HO4zbH%2FheB4DMmRdHR3K%2B1OTV7uwFvddvvkE%2FSgAjio%0AGLYPxLaJhsj8Erk3eGM%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Binance.US API Limitations

Binance.US has a limitation that do not allow the importing of crypto purchases made directly using a debit card, credit card, or bank account (ACH). As a result, these purchases are excluded entirely from the API import and will not appear in CoinLedger. If you've used Binance US to purchase crypto via the payments methods above, it is recommended you switch to the file import method. Please refer to the [Binance US File Import Guide](https://help.coinledger.io/en/articles/4935722-binance-us-file-import-guide) for further details.

Two alternative ways to add your Binance US fiat purchases are by using the Universal Import CSV (ideal for several transactions) or by adding individual transactions directly in CoinLedger (ideal for few transactions).

Fiat purchases using your USD account balance on Binance US do get exported correctly by Binance US. This limitation only applies to purchases made directly on Binance US with debit/credit/ACH.

Did this answer your question?

😞😐😃