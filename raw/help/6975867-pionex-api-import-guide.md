[Skip to main content](https://help.coinledger.io/en/articles/6975867-pionex-api-import-guide#main-content)

# Pionex - API Import Guide

How to automatically import your Pionex trades into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/6975867-pionex-api-import-guide#h_9a977ca9e4)

2. [Pionex Import Limitations](https://help.coinledger.io/en/articles/6975867-pionex-api-import-guide#h_d87780f082)


## API Import Walkthrough

**Step 1:**

Log into your [Pionex](https://www.pionex.com/en/sign) account.

![](https://downloads.intercomcdn.com/i/o/669015753/7ea45ddf7b4987a0b1d7be82/image.png?expires=1776713400&signature=efb35201a1f4a2c090c945d4e1bb0bd2d4a3cad652d3f380b3b37d7214e6281d&req=ciYuFsh7moRcFb4f3HP0gJdoPdUuicVBmgTsYMN6SXFmU%2F1V68E11cxBDPX4%0A%2BQZ%2FPnholpPt%2BY1QOQ%3D%3D%0A)

**Step 2:**

Navigate to **Account Settings** by clicking your avatar icon, and then select API Management.

![](https://downloads.intercomcdn.com/i/o/1009776770/5abad67e7db2d4004ef68ee4/image+%282%29.png?expires=1776713400&signature=26d99b4e88700cc7f9158685c105e59328eaa67fa53f178a4e3d1e381f3c7718&req=dSAnH855m4ZYWfMW1HO4zXYv6OXtiT300%2BAL4UDu3FU3cGwRiZDXDlAqoSB9%0A6wLbwR36T5faxeEqT8o%3D%0A)

**Step 3:**

Click on **Create API.** Enter an API Label (this can be any value you'd like) and click on **Submit.**

When prompted, enter the code sent to your email and your 2FA code.

![](https://downloads.intercomcdn.com/i/o/669027743/70288c61b1db2e1ada65dc92/image.png?expires=1776713400&signature=3a5e5a7a6211dc059a3d54316d0b59f12f2e852605bf86dc63b7a2c0d3768173&req=ciYuFst5moVcFb4f3HP0gB53KWPHSxJSbzJkycO81h%2FDNscbC%2ByY6YFdp93u%0AFCBYr83yQ%2BIdxtoG%2BQ%3D%3D%0A)

**Step 4:**

Upon successful API key generation, make sure to copy and store your secret key somewhere safe, as you will not be able to recover it later.

![](https://downloads.intercomcdn.com/i/o/669028444/f2a71d7141372f047a4528da/image.png?expires=1776713400&signature=1874d7419337f054fa16de53334453bf7287149e57118acc12530b7d04d15802&req=ciYuFst2mYVbFb4f3HP0gIs7Dr%2FfKlFLqxKOdqp9s9bwdnk0jrL70nGeVes8%0AmFoiuO7G8DwRCTIOGg%3D%3D%0A)

**Step 5:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Pionex** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/669963942/ce7ef4fbfbdba544be7950a2/image.png?expires=1776713400&signature=174f81566d21fadf9f436c5d27b03f83e88ff609f44ed8dea032923f1788a577&req=ciYuH899lIVdFb4f3HP0gPplGnTTuc9HGq719TOouxMHdRPXszRmZKsUFjWm%0AR%2BEGr4emJ4UOZ8rOaQ%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Pionex Import Limitations

Pionex's API has built-in limitations which may prevent you from acquiring any transaction history older than **3 months.** For this reason, you may consider switching to the _[File Import](https://help.coinledger.io/en/articles/7175790-pionex-file-import-guide)_ methodfor Pionex instead _._

Did this answer your question?

😞😐😃