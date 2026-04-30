[Skip to main content](https://help.coinledger.io/en/articles/5603669-kucoin-api-import-guide#main-content)

# KuCoin - API Import Guide

How to automatically import your KuCoin transactions into CoinLedger.

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/5603669-kucoin-api-import-guide#h_984bd54bfc)

2. [Main Accounts vs. Trading and Sub Accounts](https://help.coinledger.io/en/articles/5603669-kucoin-api-import-guide#h_f825aa5ac1)

3. [KuCoin API Limitations](https://help.coinledger.io/en/articles/5603669-kucoin-api-import-guide#h_505f628de4)


# Silent API Import Walkthrough Video

Watch video below and follow along with the written steps in this guide to see how to import your KuCoin transactions, step-by-step.

KuCoin API Import Steps: 2025

# API Import Walkthrough

**Step 1:**

Log in to your [KuCoin](https://www.kucoin.com/ucenter/signin) account.

![](https://downloads.intercomcdn.com/i/o/395095544/981666d4756a77392476b509/Screenshot_1.png?expires=1776713400&signature=0a87baf4a5ff7b8d1f7950324ce7acb8c9ac84d3aa56b745b56ad35bc7c2825e&req=dykiFsB7mIVbFb4f3HP0gHLAQTu3LFlzI%2BbpXWzG%2BC6blYAln2NIHuw6AMlk%0AQ6KcCCBAGBuLND5eMQ%3D%3D%0A)

**Step 2:**

Click on the profile in the upper right corner and select **API Management.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1332833539/fad00a8507f4f7b08d6bd81d16ee/Screenshot+2025-01-13+at+9_43_00%E2%80%AFAM.png?expires=1776713400&signature=1b2d0cd6a2cc82f2581c0b7c73ee4028e92653429888118b55eb96629b6a3152&req=dSMkFMF9noRcUPMW1HO4ze0GyLHZgG%2Bm73RvGF2GK%2BY3zukzHbdF7pRuZyYN%0AMUgv62eopN%2BF6TvkVP0%3D%0A)

**Step 3:**

Next, select **Create API.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1332834682/c666df16b886bf7734e95d855db9/Screenshot+2025-01-13+at+9_45_37%E2%80%AFAM.png?expires=1776713400&signature=f8a6f8b362fcdeba5b370457c8fe3b0bce5d35f2a291270001b250a0074aa029&req=dSMkFMF9mYdXW%2FMW1HO4zQL8tCCkxjekxS%2BDf7qAOSN%2FCFDZeZz0ztn2iZwU%0AFsOh3l2HMouv4aPiE94%3D%0A)

**Step 4:**

On the next page, select **API-Based Trading**. Ensure that **ONLY** the **General** box is selected under API Restrictions. Do not select any other restrictions under this field.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1332843579/1ca2d418f256dba78e9ff071148a/Screenshot+2025-01-13+at+9_48_34%E2%80%AFAM.png?expires=1776713400&signature=d4e73c96fbe393232547b65d955c75f94def64573f819060e7005b8a45116dc5&req=dSMkFMF6noRYUPMW1HO4zahvhwvcAWIfgCWCIUHJFri50JuWukCr4Ps4eU80%0AM91DTVLw2FQP2uM3L1s%3D%0A)

**Step 5:**

Next, create an **API Name** and an **API Passphrase**. The API Name and Passphrase can be anything you want. Just make sure to record the passphrase somewhere as it cannot be found later.

As noted above, set **API Restrictions** to **General** to restrict your **API Key** to read-only access. Also, click **No** on IP Restriction to ensure your import does not fail. Then, hit **Next**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1332879973/ff820926dff07e57228b5652c66c/image.png?expires=1776713400&signature=c7d7c1c7738ba71444e694470442a6caf5a4474b4c3d7798a2326c6e954aa154&req=dSMkFMF5lIhYWvMW1HO4zUu9INKMhdCmdHIVQlQNWgVH1XsR1xe1G57yrxXf%0ApkZGptazMIQdznTOLpo%3D%0A)

**Step 6:**

To authorize the creation of your new API keys, enter the **Trading Password**, **Email Verification Code** and **2-FA Code** on the next page, and once completed select **Confirm**.

![](https://downloads.intercomcdn.com/i/o/395124436/375d42ecc4b1005730280661/Screenshot_5.png?expires=1776713400&signature=0c1e2ec4fed85fc3e5c7f18c2e89e2f97639ddb75f2745992984d435b869f15d&req=dykiF8t6mYJZFb4f3HP0gLqlcH%2FSL1FKWbjcdpVYXlCsserRSkHvqPhCiBTq%0AR2cwUcSuKt2uLC2%2FHg%3D%3D%0A)

**Step 7:**

This window is displayed after successful security verification. From this screen you can easily copy your API Key and API Secret.

It is important to save the **API Secret** and **API Passphrase** somewhere because they are visible only while creating the **API Key**.

![](https://downloads.intercomcdn.com/i/o/488261589/33322bcecad5ee151fd5b2e8/Screen+Shot+2022-03-29+at+12.17.43+PM.png?expires=1776713400&signature=53d39fcde7d6f01554193c46aa8243b50f62be6764f8bd451eaca9bc1d54d994&req=cCgvFM9%2FmIlWFb4f3HP0gNlTs6sWxaX6FqMJ3MW9ue8%2BR6YM%2BCsY7OliohDL%0AqvA0ySew2iaPOwOIIA%3D%3D%0A)

**Step 8:**

Navigate to **Step 1. Import**. Select **Add Account** then select **KuCoin** to open up an import tab.

Select **Auto-Import** then enter your **API Key**, **API Secret** and **API Passphrase** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/503365643/54984a07b91cb2ab9378ad52/Screenshot+2022-04-26+at+19.42.49.png?expires=1776713400&signature=b3330d284f7ea9ad77600d0deab374db42bc5f8d56cb5cbc2ca6a76d91f6f366&req=cSAkFc97m4VcFb4f3HP0gLwB3wOw0QWMhBl0neslJOEI4HJrUirU8qyzww5J%0AkQ9z9EOB1hRAkvYNwQ%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

# **Main Accounts, Trading Accounts and Sub-Accounts: Which do I import from?**

The Main Account is primarily intended for sending funds in and out of the KuCoin exchange, while the Trading Account is used for spot trades. More information about these account types can be found [here](https://support.kucoin.plus/hc/en-us/articles/900002690766-Main-Trading-Margin-Futures-Pool-X-Account) and [here](https://www.reddit.com/r/kucoin/comments/nmju9m/can_you_trade_on_the_market_from_a_subaccount/), on KuCoin's main website.

It's important to review each account type to make sure you completely import from all KuCoin accounts. If you used multiple trading accounts and sub-accounts, you will need to create separate API keys for each account.

## General Overview of Each Account Type

- **Main Account:** This account is used to deposit and withdraw funds on KuCoin. In order to make spot trades on KuCoin you first need to transfer funds from your Main Account to a Trading Account. Main Accounts can also be used for P2P trades and lending. _Note that API Keys are not available for Main Accounts. If you had P2P trades on KuCoin you can enter those manually following [this guide.](https://help.cryptotrader.tax/en/articles/6028758-universal-manual-import-template-guide)_









![](https://downloads.intercomcdn.com/i/o/488220645/5043dd3e5af81760fdb4d12b/Screen+Shot+2022-03-29+at+11.10.14+AM.png?expires=1776713400&signature=9bdbdca30b02df4b7e71256307cabb057a94936210f546a347e15aec0be235b2&req=cCgvFMt%2Bm4VaFb4f3HP0gKcsmX4dtVDJTsp2EWgjrvCUagLyfAWBSs4hAI2Z%0AFYc%3D%0A)

- **Trading Account**: After transferring assets from the Main Account, the Trading Account is used for spot trades and KCS Pay fees. _API Keys are available for trading accounts._

​



![](https://downloads.intercomcdn.com/i/o/488219720/cffbd4efe3789f9f1f7f6357/Screen+Shot+2022-03-29+at+11.09.16+AM.png?expires=1776713400&signature=e4142bdcecffcca992275fb30ede3c615103b28ef42ef8f0651ce0b1f2767c84&req=cCgvFMh3moNfFb4f3HP0gJcZ89fvcfDKq6QBQY98lUgSMRKuuV9dbM5zit%2Fe%0A8hA%3D%0A)

- **Sub-Account:** Sub-accounts are customizable and can be used according to the discretion of each KuCoin user. They're often used with trading bots or margin trading. _API Keys are available for sub accounts._


# KuCoin API Limitations

**_U.S. users may not have access to API Keys on KuCoin._** New U.S. customers are not able to complete KYC on KuCoin. According to recent [KuCoin policy changes](https://www.kucoin.com/support/360015102254), this means U.S. users may not have the ability to create API keys on KuCoin. For this reason, we recommend all U.S. users [switch to using a CSV File Import](https://help.coinledger.io/en/articles/8196376-kucoin-file-import-guide) instead.

**_Due to technical limitations on KuCoin's end, their API is now limited to only retrieving data from the past year_** (going back 365 days from the date of the API sync). Transactions before that 365 day period may not be imported into CoinLedger. We recommend KuCoin users affected by this change [switch to using a CSV File Import](https://help.coinledger.io/en/articles/8196376-kucoin-file-import-guide) when importing their data instead.

**_Due to a limitation in KuCoin's API, transactions before 2/18/2019 may not be imported._**

If you traded on KuCoin before then you will need to make sure the **API pulled in all of your transactions.** If it fails to do so, you can get trade history files that covers all years. Follow [this](https://help.coinledger.io/en/articles/2624452-kucoin-alternate-file-import-guide) guide to request your KuCoin files prior to 2/18/2019 and [this](https://help.coinledger.io/en/articles/8196376-kucoin-file-import-guide) guide to export your files after 2/18/2019 directly from KuCoin.

Did this answer your question?

😞😐😃