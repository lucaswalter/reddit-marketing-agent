[Skip to main content](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#main-content)

# Universal Manual Import Template Guide

Use this template to enter all crypto transactions from unsupported exchanges and wallets into one CSV file

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 10 months ago

If you used an exchange or wallet that is not currently supported on CoinLedger, there are two options to import those transactions manually:

1. Enter individual transactions [in-app](https://help.cryptotrader.tax/en/articles/6125080-how-to-add-transactions-manually)

2. Create a custom CSV file for all of your manual transactions


This guide explains how to enter all of your manual transactions into one file, the **Universal Manual Import Template**.

## Jump Ahead

- [Import Instructions](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_4430586d04)

- [Spreadsheet Fields Explained](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_aaf6c7a4f3)

- [Troubleshooting: Map a Partially-Supported Exchange's Transactions to the Universal Template](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_c9a5862457)

- [Manual Import FAQ's](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_a0aff82621)


# **Import Instructions**

**Step 1:**

Make a copy of the [Universal Manual Import CSV Template](https://docs.google.com/spreadsheets/u/1/d/1qxX6_YJosFM6RieDCUxh3BSfxFfhnVFcipMVBOA8oCs/copy) in Google Sheets _(you only need to click [this link](https://docs.google.com/spreadsheets/u/1/d/1qxX6_YJosFM6RieDCUxh3BSfxFfhnVFcipMVBOA8oCs/copy) to copy)_.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1353406792/28cfc20788e8504ea978a87893f9/CleanShot+2025-01-27+at+09_20_24%402x.png?expires=1776713400&signature=0d2fac579833325292e0dd21dc5eb27819278da3ff8acff603442eaf4a12aea7&req=dSMiFc1%2Bm4ZWW%2FMW1HO4zdGpmqNPTYpZf%2BDGMECRGMUcyflgumVfKEtKFCVv%0ArrvVFCE5KIhLpO5qkT8%3D%0A)

**_Note_** \- In order to prevent formatting errors it is recommended to use Google Sheets to create this file, as other spreadsheet editors such as Excel and Numbers often apply formatting changes that cause the file to fail import.

​

However, if you do not have access to a Google account you can use this [link](https://docs.google.com/spreadsheets/u/1/d/1qxX6_YJosFM6RieDCUxh3BSfxFfhnVFcipMVBOA8oCs) to download a copy of the file. You will then need to create a new CSV file in your own spreadsheet editor. Be careful to keep the column headers exactly as you see them, without deleting any optional columns.

**Step 2:**

Delete the sample data - these are just examples of properly filled out transactions for you to use as a reference when entering your first few transactions.

![](https://downloads.intercomcdn.com/i/o/490912440/401bafaf4d4c3063922cb561/Screen+Shot+2022-04-03+at+10.31.11+AM.png?expires=1776713400&signature=2f83b78cbb4ce1be7a4215dc168c733ea6b72f70dd6d36ddd6b1744944279e55&req=cCknH8h8mYVfFb4f3HP0gM4KpgXhpWIfQkmuRlH9YIW0Oza%2BbdeaMRFZfimf%0A1LbygVXtNt2q7rp3JQ%3D%3D%0A)

Begin filling out this template for each of your transactions that need to be imported. Detailed instructions for what to enter for each transaction type are outlined in the following [Spreadsheet Fields Explained](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_aaf6c7a4f3) section. We recommend reading through this section while filling out the template.

**_Important Notes for entering your data into the template:_**

1. It is very important to follow the formatting of the sample data when entering your own data into the template. This includes matching the Date and timestamp format exactly.

2. Do not remove optional columns from your sheet entirely, just leave them blank. Deleting these will cause your import to fail.

3. Please ensure that all dates and timestamps are in UTC.

4. Please do not enter currency symbols such as ($ or €). These are not needed and will cause your import to fail.

5. Please refrain from entering special symbols/characters such as (+ or -). These are not needed and will cause your import to fail.

6. If you do not need to input data into a column for a certain transaction, it is best to leave it blank. Please do not enter a 0 or a character such as "N/A" or "---" as this will also cause your import to fail.





1. For [example](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide#h_833c37a045): when entering a Deposit, you only need to fill out the Asset Received and Amount Received columns. You can simply leave the Asset Sent and Amount Sent columns blank for this particular transaction.


**Step 3:**

Save the template as a CSV file to your computer. Select **File** -\> **Download** -\> **Comma Separated Values** (.csv)

![](https://downloads.intercomcdn.com/i/o/476856477/c72eba60bbb93bfdbcf71176/Screen+Shot+2022-03-08+at+9.37.29+AM.png?expires=1776713400&signature=4e0f28eca2f4d030269150ce47f648f0a5369cdc079c050c86dc77e08578bce2&req=cCchHsx4mYZYFb4f3HP0gHUE8U%2FhDud8A7ip9bajq7Va%2B2Jz%2BitIX5EF%2FkS6%0AMlF3SE8l0EOJOYupmA%3D%3D%0A)

**Step 4:**

Navigate back to the CoinLedger site and upload your CSV file under the **Other Account** tab.

![](https://downloads.intercomcdn.com/i/o/699815209/21929ff870390fb423087560/Screen+Shot+2023-03-27+at+10.36.52+AM.png?expires=1776713400&signature=0bc3b2224f73d89d3aff36bde348ac631c042c002abd9ae6178418289ef90d9e&req=cikuHsh7n4FWFb4f3HP0gOzhV2WI5ePLzt5E%2BjQXyOLpn1Vs%2FFeINdukhpRT%0AT0NUWrjtpL8yuFOwOw%3D%3D%0A)

**Step 5:**

To customize the name of your manual import, click on the import tab and select **Edit Name.**

![](https://downloads.intercomcdn.com/i/o/504730806/70b3f9f7b36358347accf619/Screen+Shot+2022-04-28+at+1.49.19+PM.png?expires=1776713400&signature=4fccf328b01be5e7e9c9991d9a03b410a5e7a78a552911f9545226c8762a78fe&req=cSAjEcp%2BlYFZFb4f3HP0gPrA%2ByDKFu9YF5rb2BmSP4TKUMi6d3w4MvHUfSak%0AaEhBpaM%2BjCDur81D8g%3D%3D%0A)

Enter the name of the platform or whichever name will best help you keep track of your imports.

![](https://downloads.intercomcdn.com/i/o/504730938/08edae8b859ef5af96f3274e/Screen+Shot+2022-04-28+at+1.49.38+PM.png?expires=1776713400&signature=cbb9351a13795a857b8596110411748447fa9cde4d301c68ab8234a3f54f423a&req=cSAjEcp%2BlIJXFb4f3HP0gJzeBzYIt3al8hcE53CIxpQoYXJ%2BLKDuCW4%2FAAMJ%0AF4bf2uJXzAtij371NA%3D%3D%0A)

# **Spreadsheet Fields Explained**

Different fields are required depending on the transaction type. The following sections explain in detail what you should enter into each field. Click on the drop-down menu in each category to review these instructions.

## Date (UTC)

The UTC timestamp of your transaction

- The timestamp must be in the format of **Month-Day-Year**





  - Example: **mm/dd/yyyy hh:mm:ss**

  - Note: Hours, minutes, seconds are optional and a dash separator ('-') can be used instead of a slash '/'


- ( **VERY IMPORTANT** to ensure your dates are in UTC!!)


## Platform

The name of the platform where you transacted. This is an optional field that makes it easier to review and sort transactions later on. You can add as many platforms as you need into the spreadsheet.

## Asset Sent and Amount Sent

The currency and the amount that is outgoing in the transaction.

- A withdrawal of 50 XRP will have XRP set as the **Asset Sent** and 50 as the **Amount Sent.**

- If you traded BTC for ETH, BTC would be the **Asset Sent.**


## Asset Received and Amount Received

The currency and the amount that is incoming in the transaction.

- An income deposit of 50 XRP will have XRP set as the **Asset Received** and 50 as the **Amount Received**.

- If you traded BTC for ETH, ETH will be the **Asset Received**.


## Fee Currency and Fee Amount

An optional field which specifies the currency in which the fee was applied in this

transaction. **_Skip this field if the trading fee has already been applied._**

## Type

Transaction types are classified as follows:

## **Trades**

All fields for **Asset Sen** t and **Asset Received** are filled out

- **Buys**

- **Sells**

- **Crypto-to-crypto trades**

​


## **Incoming deposits**

The fields **Asset Received** and **Amount Received** are filled out

- **Income**

- **Interest**

- **Mining**

- **Staking**

- **Hard Fork**

- **Airdrop**

- **Gift Received**

- **Deposit** \- this is treated as a non-taxable self-transfer


## **Outgoing withdrawals**

The fields **Asset Sent** and **Amount Sent** are filled out

- **Gift Sent**

- **Casualty Loss**

- **Theft Loss**

- **Investment Loss**

- **Interest Payment**

- **Merchant Payment**

- **Withdrawal -** this is treated as a non-taxable self-transfer


**_Important note:_** The **Type** field is a mandatory field for all deposit and withdrawal transactions, but not for trades. All buys, sells, and crypto-to-crypto exchanges can be labeled as **Trades** but you do not have to put anything under the Type field for these transactions. As long as both Asset Sentand Asset Received fields are filled out, our importer can read the rest.

If you need further info on which transaction types CoinLedger supports and how we define them, check out our [guide on transaction types](https://help.coinledger.io/en/articles/8546372-what-transaction-types-does-coinledger-support)!

## Description

An optional field - helpful for you to add notes about the transaction.

## TxHash

An optional field for entering the transaction ID

# **Troubleshooting: Map a Partially-Supported Exchange's Transactions to the Universal Template**

Below we demonstrate the step-by-step process for mapping your transactions from another exchange's spreadsheet into our Universal/Manual Import Template. Click on the drop-down menu below for a detailed video outlining each step.

### Mapping Partially-Supported Exchange Transactions to the Universal Template

CoinLedger - Import Trades From Partially-Supported Exchanges

**Step 1**

First, download the transaction history file from whichever crypto exchange, wallet, or platform you're looking to import. Usually you can find this directly within your exchange or request it from your exchange's customer support.

**Step 2**

Once you have all of your transactions from your exchange, make a copy of the Universal Manual Import [spreadsheet template](https://docs.google.com/spreadsheets/u/1/d/1qxX6_YJosFM6RieDCUxh3BSfxFfhnVFcipMVBOA8oCs/copy).

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559605234/9128bec5fc4029856a533cd41124/Screen%2BShot%2B2022-04-03%2Bat%2B10_31_11%2BAM.png?expires=1776713400&signature=74d953611aaa7cd4f9bbd5d2e3f59ee5213347a1bb07ab02db377709a051b25d&req=dSUiH89%2BmINcXfMW1HO4zflkMk4nh0UNFF5UXHr2vwkgS7jklZDgF1Ks6%2FV5%0AZFFS%0A)

**Step 3**

Now map your transactions from your exchange to match the supported generic/manual import template on our website, as shown in the video above.

For further guidance on troubleshooting spreadsheet formatting errors, check out [this guide.](https://help.coinledger.io/en/articles/4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting)

**Step 4**

Once complete, download your newly created spreadsheet as a **CSV file** and upload it into CoinLedger.

# **Frequently Asked Questions**

Click the drop-down menu below to read the most common questions we hear about the Universal Template.

### Universal Template FAQ's

1. **Do the transactions need to be entered in chronological order?**

No. You can enter your transactions in any order. CoinLedger will order your trades by timestamp upon import.

​

2. **Can I enter multiple platforms in the same file?**





Yes. This template was designed to make it as easy as possible to enter all your transactions in one place.

​

3. **Do I need to include fees?**

This depends on whether the exchange already applied the fee to the transaction or not. You should review your specific exchange data to verify whether you need to add the fees separately or whether they are already included.

​

4. **What happens if I don't enter the Type on a deposit/withdrawal transaction?**

The file will fail import and you will need to edit the file to specify the Type. Otherwise, our software will have no way of determining whether you received or sent the asset.

​

5. **Do I need to enter the hours, minutes, and seconds on the timestamp?**

You don't have to. The only required fields are the month, day, and year. However if you do have the info for hours, minutes, and seconds it is best to enter that as much data as possible. Crypto prices are volatile and can range wildly over one day, so to be most accurate you should enter the full timestamp.

​

6. **What is the difference between Theft, Casualty, and Investment Loss?**





Investment Loss is the only type that gets reported as a realized loss on the Form 8949. Theft and Casualty losses will remove the asset from the global balance, but you will not realize the loss for tax purposes. You should consult with a tax professional before reporting an Investment Loss. Read [this guide](https://cryptotrader.tax/blog/reporting-stolen-or-lost-cryptocurrency-for-tax-purposes) to learn more.

7. **How do I enter NFT transactions into the manual template?**





NFT transactions can be imported manually as a "Trade" in the Universal Template. However, before importing these transactions, you will first need to add a custom asset representing this NFT to your CoinLedger account (otherwise your import will fail to map the transaction to the correct NFT asset). See instructions for adding a custom NFT asset to your account [HERE](https://help.coinledger.io/en/articles/9787001-how-can-i-add-a-custom-asset-to-my-coinledger-account).


Did this answer your question?

😞😐😃