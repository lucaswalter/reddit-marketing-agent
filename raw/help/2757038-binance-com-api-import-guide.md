[Skip to main content](https://help.coinledger.io/en/articles/2757038-binance-com-api-import-guide#main-content)

# Binance.com - API Import Guide

How to automatically import your trades using the Binance API

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 7 months ago

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/2757038-binance-com-api-import-guide#h_3b3a6e1104)

2. [Binance Import Limitations](https://help.coinledger.io/en/articles/2757038-binance-com-api-import-guide#h_3911b1b29b)


Binance API Import Walkthrough

Copy link

[Open video in Loom](https://www.loom.com/share/ef0883b5a9a94f319992d54e8f556378)

0

1.2×

1 min 14 sec⚡️1 min 32 sec1 min 14 sec1 min 1 sec49 sec43 sec37 sec29 sec

![](https://cdn.loom.com/sessions/thumbnails/ef0883b5a9a94f319992d54e8f556378-00001.jpg)

Copy link

[Open video in Loom](https://www.loom.com/share/ef0883b5a9a94f319992d54e8f556378)

0

1.2×

1 min 14 sec⚡️1 min 32 sec1 min 14 sec1 min 1 sec49 sec43 sec37 sec29 sec

# API Import Walkthrough

**Step 1:**

Navigate to your [account](https://www.binance.com/en/usercenter/dashboard/overview).

​

​ **Step 2:**

After sign in, select your profile icon in the top right corner, and navigate to the Account menu, then click to expand the dropdown menu. You will then find the **API management** option, click on it.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1750729656/4ed51e76f071613bf5dd233e197e/image.png?expires=1776713400&signature=e52a946cf1b67323a69d5759982f822266181fa9286feb3517d0b1a5838b69f8&req=dSciFs58lIdaX%2FMW1HO4zU%2Fpk%2FUB4pKnwIVlx57uQ9bbW5a3eB0bECODxEY9%0AXMTa5l1lLJ%2Fb%2Bd4jmYo%3D%0A)

**Step 3: Create API Key**

You will be prompted to create a new API Key. Enter a label for your key, and click **Create**. ( _This label can be anything._)

![](https://downloads.intercomcdn.com/i/o/262800410/b1e124eb03c3e874363dbeaa/Screen+Shot+2020-11-04+at+10.15.48+AM.png?expires=1776713400&signature=5ce710995ce8df3d88c571e0730adc4a8f6e113e933d373f88c21c87f5c4b8da&req=diYlHsl%2BmYBfFb4f3HP0gLoAvW2Gi2dCY99cnCSS4ZjFL%2F67ZdicfIaEcf%2FO%0AXth6FZB2Eg1rYOBPVg%3D%3D%0A)

**Step 4: Enter Verification Codes**

Next you will need to enter both an e-mail and 2FA verification code. Click **Send** and you will receive the e-mail code in your inbox. Retrieve the 2FA code from your authenticator app and after entering both codes click **Submit**.

![](https://downloads.intercomcdn.com/i/o/262809129/8399100a88da019c05da9c5b/Screen+Shot+2020-11-04+at+10.31.13+AM.png?expires=1776713400&signature=fe1c916413e81a84ecda7c2244c9469a90ce832df8aebdc7744df552918f27f1&req=diYlHsl3nINWFb4f3HP0gOhvyPCOY7Tc9%2BEWC%2BjqhZUQf1Ab3rAwOQdn4oVp%0A0ziBeEIZp8FrOYHL5Q%3D%3D%0A)

**Step 5: Edit Restrictions**

You will see a green banner notification that says **API key created** and then it will display your new **API Key** and **Secret Key**.

![](https://downloads.intercomcdn.com/i/o/262825772/129059e5a02574ebda781793/Binance.API.png?expires=1776713400&signature=270e072862d3850837019727df4608391fce7204b9615cba7f34042fda194687&req=diYlHst7moZdFb4f3HP0gLn%2FHDGncIz8mnz10%2BblJejju2KukXf8Tvlxy1KC%0AER1drFSwOExMEdXDvA%3D%3D%0A)

**Step 6: De-select Trading Access**

​

Click **Edit Restrictions** and then deselect **Enable Spot & Margin Trading**( _Remember, CoinLedger requires read only API access. You do not need to grant CoinLedger permission to enable trading.)_

Then make sure that **Can Read** is selected.

[Learn more about API key access here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts)

![](https://downloads.intercomcdn.com/i/o/262825620/7175eecaef8e91a46b242449/Api.Binance.2.png?expires=1776713400&signature=7a0f195d5638b611cbf45d045dc36c0c062cc656f3d0b7d1ed54544cf90dba0f&req=diYlHst7m4NfFb4f3HP0gF8OONRDBS2EAzpaOb1vdGEILGBGM8WBTxCzMM3%2F%0AIMFbGPSKXZ44Xvxi1Q%3D%3D%0A)

**Step 7: Save restriction settings**

​Click **Save** and you will be prompted to enter your 2FA code again.

![](https://downloads.intercomcdn.com/i/o/262851182/d0fbae748e1486d6df7d5566/Screen+Shot+2020-11-04+at+12.06.12+PM.png?expires=1776713400&signature=e78394da9f8f1f8c931609f3c56f239f42a62d14d175991768af597a1e075671&req=diYlHsx%2FnIldFb4f3HP0gI%2FCHoAeEVwnD7xqrxbO%2BBjcWWzhkaw0uXkUdft6%0AUrQ5ZTvct%2BEe6Ub%2Bsg%3D%3D%0A)

**Step 8: Enter Into CoinLedger**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Binance** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into CoinLedger. Click **Connect**.

![](https://downloads.intercomcdn.com/i/o/503335034/211922845c1d1f22462a328a/Screenshot+2022-04-26+at+18.55.00.png?expires=1776713400&signature=0ccb54d66994a173843dd2109dcdec60440794b45f6fa69c803f476f4407b70d&req=cSAkFcp7nYJbFb4f3HP0gDtya%2BlCXQk%2FVPYTxF4NLc%2ByC4Nb%2BayShL5P71eB%0AnLOYH6zPa3LVWD9I6Q%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Binance Import Limitations

Due to limitations with Binance API, import times may take up to 20 minutes to complete.

The following transaction types get pulled into your CoinLedger account when you link your Binance account via API:

- Spot market trades

- BNB conversions

- Liquid swaps

- Fiat trades

- P2P trades

- Crypto deposits and withdrawals

- Convert trades

- Commission Rebates

- Referral kickbacks

- Dividends





  - Flexible Savings

  - Launchpool

  - Savings Trail Fund

  - Fixed Savings

  - Activities

  - Locked Staking

  - DOT Slot Auction

  - DeFi Staking

  - Pool Savings

  - Dual Investment

  - Distributions

  - Stakings

  - Airdrops

  - Trading rewards

  - Lucky Draws

  - Mainnet Swaps

  - Black Friday Settlement

  - Refunds

  - Giveaways

  - Cashbacks

  - Buybacks

  - Trading Competitions

  - Learn & Earn programs

  - Monthly token unlock programs

  - Launchpads

  - Bounty Programs

  - Token Swaps


If you had any other type of transactions, those transactions will need to be entered separately following the [manual import guide](https://help.cryptotrader.tax/en/articles/6028758-universal-manual-import-template-guide).

Did this answer your question?

😞😐😃