[Skip to main content](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide#main-content)

# Kraken - API Import Guide

Import your spot and margin transactions from Kraken into CoinLedger automatically using our API integration

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

Spot and margin transactions can be imported into CoinLedger from Kraken using their API import method. Read on for step-by-step instructions on this import process.

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide#h_a73ed9edb1)

2. [Kraken API Limitations](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide#h_9c2121d5fd)


# Video Guide

How to Do Your Kraken Margin Taxes (the EASY way) \| CoinLedger - YouTube

Tap to unmute

[How to Do Your Kraken Margin Taxes (the EASY way) \| CoinLedger](https://www.youtube.com/watch?v=7zXrMnPeLec) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

## API Import Walkthrough

**Step 1:**

​ [​Login](https://pro.kraken.com/app/trade/btc-usd) to your Kraken account. Linked here is the URL for Kraken Pro. The remaining steps shown below are using the "classic" layout on Kraken Pro, which you should be prompted to select when you first login.

![](https://downloads.intercomcdn.com/i/o/378140086/fa8a849d18886511d8851750/image.png?expires=1776713400&signature=af1a52c9bc18010a7d83746cb957bfd659b4746a03434790c17065751d5dced5&req=dycvF81%2BnYlZFb4f3HP0gP2sRc2Fgu%2F3b3Um1rTcBYAqyJRhAdQRrvJFybXB%0A1Z2Hlfcoj9aFooDrNQ%3D%3D%0A)

**Step 2:**

Select your profile from the top-right dropdown menu and navigate to **Settings.** Then, click **API** to view and create new API keys.

![](https://downloads.intercomcdn.com/i/o/916603523/cb5b09bc05911d8ca363ae88/Screenshot+2023-12-22+at+12.48.52%E2%80%AFPM.png?expires=1776713400&signature=1e3d211ea1dd41e469ded854981d41eb130e916d49b006b6799e9314f50fb596&req=fSEhEMl9mINcFb4f3HP0gHsNgUOZQvnqYHfNm5%2FLsf763Kg8ZNxTj9AnMvnE%0AcYL6%2B2jwEp9FEbSPYw%3D%3D%0A)

**_Direct Link:_** [https://pro.kraken.com/app/settings/api](https://pro.kraken.com/app/settings/api)

**Step 3:**

Next, click the **Create API Key** button and create a new API key with the settings below. After the settings are filled out, click the **Generate Key** button.

**Be sure the following checkboxes are enabled:**

- **Query Funds**

- **Query Open Orders & Trades**

- **Query Closed Orders & Trades**

- **Query Ledger Entries**


Then, at the bottom of the menu turn Custom Nonce Window **ON** and set the **Nonce Window** to 10,000.

![](https://downloads.intercomcdn.com/i/o/916605285/035a04d3f6c3698a2d7bead9/Screenshot+2023-12-22+at+12.52.14%E2%80%AFPM.png?expires=1776713400&signature=d27d69d5d33cb2db4a08db176c3ef2ffd9151692cac326c40cb5389890db9994&req=fSEhEMl7n4laFb4f3HP0gAjXiQudh%2BdwaFAWgk4ACG0vT2xq2hHgnP9OkX%2Bc%0AaIYf%2FGtZrbDMDcEh1Q%3D%3D%0A)

**Step 4:**

On the next screen, copy the **API Key** and **API Private Key** values from Kraken. These will be needed for later to import your transaction history, and you won't be able to see them again after closing this window.

Once copied, head over to the CoinLedger app.

**Step 5:**

Navigate to the **Import** stage **.** Select **Add Account** then choose the **Kraken** tab on CoinLedger. Click on **Auto-Import** then enter your API KEY into the API Key field. Finally, enter your API Private into the **API Secret** field. Then, click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/916607684/d65df5fe85e941e022e43c93/image.png?expires=1776713400&signature=b37d4c49d319ac0ef47928c85bef427611a28f9b6bbec5bb778359cbed808ce7&req=fSEhEMl5m4lbFb4f3HP0gHLPqfsqR7qGxWTc2PZT2%2B7u6YnHhekKx0mW4oWo%0AgAF0LdpCBl6tgsLYQA%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

## ​Kraken API Limitations

If you have a lot of trades, note that your import may take some time, typically around 5-10 minutes but occasionally longer. This is normal and completely expected!

​

Did this answer your question?

😞😐😃