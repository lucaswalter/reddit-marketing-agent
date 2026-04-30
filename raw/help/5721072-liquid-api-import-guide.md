[Skip to main content](https://help.coinledger.io/en/articles/5721072-liquid-api-import-guide#main-content)

# Liquid - API Import Guide

How to automatically import your trades by connecting your Liquid account

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/5721072-liquid-api-import-guide#h_396b09817a)

2. [Liquid API Limitations](https://help.coinledger.io/en/articles/5721072-liquid-api-import-guide#h_2d1e86b4ff)


# Legacy Import Instructions

Liquid API Import Walkthrough

Copy link

[Open video in Loom](https://www.loom.com/share/6beac0e8aa5f424382afb1774aa8a648)

0

1×

1 min 2 sec⚡️1 min 17 sec1 min 2 sec51 sec41 sec36 sec31 sec24 sec

![](https://cdn.loom.com/sessions/thumbnails/6beac0e8aa5f424382afb1774aa8a648-00001.jpg)

Copy link

[Open video in Loom](https://www.loom.com/share/6beac0e8aa5f424382afb1774aa8a648)

0

1×

1 min 2 sec⚡️1 min 17 sec1 min 2 sec51 sec41 sec36 sec31 sec24 sec

## API Import Walkthrough

**Step 1:**

Log in to your [Liquid](https://app.liquid.com/sign-in) account.

![](https://downloads.intercomcdn.com/i/o/416921895/3b719a251b90e7ca410d2008/Screenshot_0.png?expires=1776713400&signature=16d0bbd80e09c826892663149f87beb088da4c0f3d89220d5dae9e0b8d75804c&req=cCEhH8t%2FlYhaFb4f3HP0gJ4F20xWAdfNi8d899o%2F8oxl%2FLQH0XF9TtRCDZ%2Bk%0A0zOkijRuTsznE21QXg%3D%3D%0A)

**Step 2:**

Select your profile in the upper right corner and then click **API Token** from the dropdown list.

![](https://downloads.intercomcdn.com/i/o/416922936/55f24f4860a82f23a87abb1d/Screenshot_1.png?expires=1776713400&signature=280ce4437d1eb1965cb342ac42c52f9f348f99602ee1c737b0da4a5f4f17a7d5&req=cCEhH8t8lIJZFb4f3HP0gFOE16T1ZJVYqP8gSy6hNmY4cw4DJl3TNmfkPinl%0Ap8ep0O0pzeJlCE6sIQ%3D%3D%0A)

**Step 3:**

Click on **Create API Token**.

![](https://downloads.intercomcdn.com/i/o/416923657/5d38488a69fa172c025839be/Screenshot_2.png?expires=1776713400&signature=1a00228ccba0a3875134bdaa745448a9ba096b73b48543deae591a66495912e8&req=cCEhH8t9m4RYFb4f3HP0gAqfWv2taKbU%2BH4yRLWWiAMSFpohuLtIhBIsOurq%0Aqfgu7dXRE9wNBUqLsg%3D%3D%0A)

**Step 4:**

Select **Read** for every permission. Be sure NOT to add any IP address to the IP whitelist.

Then, Input your **2FA Code** and select **Create Token**.

![](https://downloads.intercomcdn.com/i/o/416923974/53a276b321e21cee8f5930bd/Screenshot_3.png?expires=1776713400&signature=61f405a5bf22e1ccb366513d8ca6a2f153f4a8b662c31b92b74878982447ca2d&req=cCEhH8t9lIZbFb4f3HP0gNjWX5E1TSfyV5xvEi47zUD3nd1ZaSi1jrNf7BjE%0AYRRd%2FI3BNJIweaZkzw%3D%3D%0A)

**Step 5:**

Store your **Token ID** and **Token Secret** in a safe place, as this data is not accessible once you close this window.

![](https://downloads.intercomcdn.com/i/o/416928469/ea833c6ae93089944d1a1b3c/Screenshot_4.png?expires=1776713400&signature=ae39904d8765af5461adf5db5324bf39b55ffa58becdfd7e3ba21702717501ed&req=cCEhH8t2mYdWFb4f3HP0gNjN4aGWuK3hYLQvF9lbBMORucknAAb1uy5BATlN%0ApTESC4We9Gyx0i%2BNsw%3D%3D%0A)

**Step 6:**

Back in the CoinLedger, enter your **Token Id** and **Token Secret** from earlier steps into their matching fields on the **Liquid** tab, and press **Sync Transactions.**

![](https://downloads.intercomcdn.com/i/o/503339196/7c528d8263d470260eac6fbc/Screenshot+2022-04-26+at+19.01.08.png?expires=1776713400&signature=c054274234e1d87f2c8505b4dfd2a030f94a790d7e530ac230b461101c391237&req=cSAkFcp3nIhZFb4f3HP0gJrIfow2K7uOQ9fC4b%2Fipm9x1fbF8zJPRJdY8I0D%0A382JeHpkyPngdGwQXw%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## Liquid API Limitations

Liquid has recently paused withdrawals and deposits in accordance with bankruptcy proceedings and may not be available in your market. If this is the case, _please reach out to their Customer Support directly._ Alternatively, you can import your transactions from these exchanges into CoinLedger using our [Universal Manual Import](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide) template.

​

Did this answer your question?

😞😐😃