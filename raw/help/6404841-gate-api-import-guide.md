[Skip to main content](https://help.coinledger.io/en/articles/6404841-gate-api-import-guide#main-content)

# Gate - API Import Guide

How to automatically import your Gate transactions into CoinLedger

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 6 months ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/6404841-gate-api-import-guide#h_a935b42955)

2. [Gate Import Limitations](https://help.coinledger.io/en/articles/6404841-gate-api-import-guide#h_29935c3b1c)


# Video Import Guide

How to Calculate Your Taxes From Gate.io (The FAST Way!) \| CoinLedger - YouTube

Tap to unmute

[How to Calculate Your Taxes From Gate.io (The FAST Way!) \| CoinLedger](https://www.youtube.com/watch?v=4Pt6NJcUPdE) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

## Step-by-Step Import Instructions

**Step 1:**

Log in to your [Gate](https://www.gate.com/) account

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802789084/4b788eebb74feb6c3e9bdd084276/0d922336-f431-4194-9b87-2d5f5e4f5c0a.png?expires=1776713400&signature=a06217e09e09ddfeef75aff59d521eeecd7b392cf5b92d02776e6a31e353f125&req=dSgnFM52lIFXXfMW1HO4zYbdk2xvbgPsJtXuamgyKutWxwSjhfdfYfW6qrC3%0AlAvoYX4fKr4r30WymM4%3D%0A)

**Step 2:**

- Navigate to the **[API](https://www.gate.io/myaccount/apiv4keys)** section

- Click on the **User** icon in the top right corner and select **API Key Management**


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802794090/3280d4f58a2c96458e3e2fe8e821/d117d981-fe39-4869-b56a-1a8123c4a7cb.png?expires=1776713400&signature=2214b2cce9ed71e63211080c549217ab8dc51bd9049ccf782f4f903503db6a24&req=dSgnFM53mYFWWfMW1HO4zXyjXkG3I593O2t%2FClN4HengFm0%2B8buQryYW%2BJtm%0A%2BK3m805xZHzayfqHcsc%3D%0A)

**Step 3**:

Click on Create API Key button on the right.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802796628/3ec4d208546f7185b3fe88aac003/1e9ea0f9-60bf-4fdd-84b0-dc7f5d2a9a2a.png?expires=1776713400&signature=7f1d6fda1adc9052b42d2ac1b7b412fb5280e41b1f2f8fcb0a3dd2f256daac43&req=dSgnFM53m4ddUfMW1HO4zf7TdbjH1Rg%2BM5tD3aqadj%2FfUB00mp30LIPqFiMY%0A%2FoyVx6ljf%2FVY3DCHuh0%3D%0A)

**Step 4:**

Select **Trading Account** as Account Type.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802798477/8cfb93a0e0de518523af9e6ee690/ccd6bfda-4ff5-4cb3-8aec-016f6431c33e.png?expires=1776713400&signature=f970c94c851b5b4fcbceff3b09510c7572675e2b06aaed7dceafec94c143fbad&req=dSgnFM53lYVYXvMW1HO4zdYtNeyvpbB5fAZoUt7G9DrstLeVA3R3j1hI3b64%0AlwKNX7qhRiQIu6GyuLQ%3D%0A)

**Step 5:**

Fill Create API Key requested info. Enter a remark (this can be anything you'd like) for the API key.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802801896/de2a1bc9eba004bedbd71669c64c/d6390f1f-2c3c-4b07-865f-d61a87ccbf8c.png?expires=1776713400&signature=5893f327cb0e75eba78e51ee98f1c7139f30107f0c7341cbd8508a2b38aa89d4&req=dSgnFMF%2BnIlWX%2FMW1HO4zfWdiS%2Byu3J9hiJivYg0WnJLSrq7UZkvDvEypg2s%0AVXyAErLS2ZssFZQk6%2FM%3D%0A)

**Note: If you are in US, select “Later” for Binding IP option.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802804856/a1bdc9bdfd9cadc6f086f8f301c1/45f1cf0f-65ab-47d2-af94-69748cf30538.png?expires=1776713400&signature=5496bdfea86a1eab3b7782029fc00667e6a1f22ab009bbbdd2aa7c4e8d61584e&req=dSgnFMF%2BmYlaX%2FMW1HO4zcnt%2BI94XrmeJGXa3aE0fI17se8SFznv8F5l7PNl%0A3rSvjz3nBLHYBobI2jk%3D%0A)

Make sure **Read Only** permissions are given to **Spot Trade and Wallet**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802806822/398da1622c48f6ba5cb20d0383aa/f9789d4c-92c1-46ec-8394-f948dc52ed09.png?expires=1776713400&signature=3f0cce181b8bc98037a98316f1ac0526b17fb0174caef4408a60664d4828cfe2&req=dSgnFMF%2Bm4ldW%2FMW1HO4zQKQkNDZWfKsZHb8zPXSYWzu8NYxssQS0VKibpiJ%0A8ZL%2Bccy59Jk64kjThFE%3D%0A)

**Step 6:**

Accept **Risk Reminder** check boxes.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802809450/d957bb195f6cccd19e068239479c/4352cf36-aab0-4a3f-b786-02af67d6e083.png?expires=1776713400&signature=f35234d92440267beb9c10da26975dc70b48c41b186236b885ed22e2f259a084&req=dSgnFMF%2BlIVaWfMW1HO4zXsViCFJ33ACDmygNw7sidqRMuFeHsScjW9bjJUx%0ATYDfos%2FfQONk2wTCRjI%3D%0A)

Step 7:

Fill security verification info.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802816464/2cd69538db9ae2aae23c32cdaf64/ac076f00-e505-440f-99de-4a07944665c0.png?expires=1776713400&signature=8ff3c4b2284301971b00cd194eeb2453a190bd30bac683e51d2bba895038cf1e&req=dSgnFMF%2Fm4VZXfMW1HO4zf7eAvobXU%2FVQ2ZH3DBdvWYZN0wpkHG21%2BGc7FFd%0AzL1RkXS1ZqnA30iVvX8%3D%0A)

Step 8:

Copy the Key and Secret into a safe place.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1802817719/7c72430535bebce1753677fac55b/2da32300-6129-43b6-82e9-3a92a7e43c01.png?expires=1776713400&signature=9242623339dee27112d43d16a4baaa2d396f7cc382381966685bc920604d57c5&req=dSgnFMF%2FmoZeUPMW1HO4zf6ZaEh%2BeCBSgphzx5uo1RPuKy%2FDj57O%2BJQOm%2FuM%0Ad6LhJ5vwA582k6zaWAA%3D%0A)

**Step 9:**

Navigate to Step 1. Import. Select Add Account then choose the Gate tab on CoinLedger. Click on Auto-Import then enter your API Key and API Secret into the correct fields. Click Sync Transactions.

![](https://downloads.intercomcdn.com/i/o/561323352/45a20b4f5ca900a7aab6e63c/Screenshot+2022-08-11+at+08.16.05.png?expires=1776713400&signature=bccbaf9e035a184b161d94e93636e8b8539749920564a7f18131d867184178a4&req=cSYmFct9noRdFb4f3HP0gA1P9HQp9oBClh3Ou0VTevAUkG1hkJET8r%2Bp%2FnKI%0AMygPsp68RYDrKFUJDg%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Gate Import Limitations

Fiat purchases made with debit/credit or bank transfer are exported by Gate as one-sided deposits. Fiat purchases made from your fiat wallet balance do get exported correctly (both sides of the transaction are included so CoinLedger is able to parse these correctly as a Fiat Buy transaction)

If you purchased crypto on Gate using debit/credit or bank transfer, you will need to import those purchases separately. There are three ways that you can import these fiat purchases into CoinLedger.

- Add them in-app as [single transactions](https://help.coinledger.io/en/articles/6125080-how-to-add-single-transactions-in-app) under your Gate tab in **Step 1. Import**

- Create a [CSV template](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide) and enter your fiat purchases as Trades

- Download the Deposits file from Gate. When you import this file into CoinLedger your fiat purchases will show up as one-sided deposits. Navigate to **Step 3. Review** and edit the transaction to change the transaction type to Fiat Buy, and then add in the fiat amount.

​


​

Did this answer your question?

😞😐😃