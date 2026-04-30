[Skip to main content](https://help.coinledger.io/en/articles/6563578-ndax-api-import-guide#main-content)

# NDAX - API Import Guide

How to automatically import your NDAX transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger _only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts)._

**Note:** NDAX API only returns up to 3 months worth of trades. If you traded on NDAX for longer than 3 months it's recommended to switch to [file import](https://help.coinledger.io/en/articles/6518867-ndax-file-import-guide) to capture the full range of your crypto transaction history.

How to Calculate Your NDAX Taxes (the EASY way) \| CoinLedger - YouTube

Tap to unmute

[How to Calculate Your NDAX Taxes (the EASY way) \| CoinLedger](https://www.youtube.com/watch?v=obywX6L1PhM) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

**Step 1:**

Log into your [NDAX](https://ndax.io/auth/login) account.

![](https://downloads.intercomcdn.com/i/o/581449437/fe555242bd337de0b531ada8/image.png?expires=1776713400&signature=dab26621d74e210b5c4f89112d3245c0095fe72d4a701a4fe4a46c0bb87f2fa7&req=cSgmEs13mYJYFb4f3HP0gB%2FQYEcQg2IzgyophP1kfceVinJn5aE%2Fi46yvv1a%0AT5hT50eP%2BkzvfxbLdQ%3D%3D%0A)

**Step 2:**

Scroll down on the side bar and navigate to **Settings.** Once there, click on **Generate New Key** in the **API Key** section.

![](https://downloads.intercomcdn.com/i/o/581452150/e319ce645fc26423879e0f7d/image.png?expires=1776713400&signature=a84086cb60178f05d68fcd024345d48ff09416871fdf70ed66fa8b76ecaaa328&req=cSgmEsx8nIRfFb4f3HP0gNoNlZk3Q0HcC9%2Bw8SsexbZ%2FUI%2BnEpnkAPiSKR%2B4%0A9h59hzE5eeBCIcONeQ%3D%3D%0A)

**Step 3:**

Select **Allow Read Only** and click on **Generate**.

![](https://downloads.intercomcdn.com/i/o/581452939/bd2133b286c7fcbfeb1889f9/image.png?expires=1776713400&signature=9fff74553a515f293cae74cd71fce8ad9c2d61523043f20317051668e9db12cb&req=cSgmEsx8lIJWFb4f3HP0gDeKew8id1GXFITwtvbWS8zPKE2iRB8dSBbUAmIp%0Acb261WZVFKsO%2Frl%2FLw%3D%3D%0A)

**Step 4:**

Upon successful API key generation, make sure to store your secret key somewhere safe, as you will not be able to recover it later.

![](https://downloads.intercomcdn.com/i/o/581454178/54281fe6e639c58cf73aabf5/image.png?expires=1776713400&signature=7e5bf8c4d765d649c63454b99b83e390eeb354d1487dd81ea9089ac8e9431f80&req=cSgmEsx6nIZXFb4f3HP0gE7eIEGCMxwqsFBvKhbeXZZb3TxVhH8riLZyf9i0%0As5dFZxsEptJXCAgNrA%3D%3D%0A)

**Step 5:**

Copy your **User ID** from the **Personal User Info** section, as you will need this in order to import your transactions as well.

![](https://downloads.intercomcdn.com/i/o/581457071/a6fe04649e0cb324cb736f48/image.png?expires=1776713400&signature=7b0241f8ce3046b51eb1397286bdc58997c80b61e9e2eb1f2f2874fcb9c3a38d&req=cSgmEsx5nYZeFb4f3HP0gK2OvUmkkyKeaqcUUd3Efys0CGR9okFQ01nK%2BIJl%0AQaFD%2BKzr0lZRspCMYw%3D%3D%0A)

**Step 6:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **NDAX** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key**, **API Secret** and **User ID** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/581631820/770828d47d24d3041b6c878b/Screenshot+2022-09-16+at+16.15.45.png?expires=1776713400&signature=009feb69e76bf709031d9ebf8ee041373e634dc11175a4676c510e779bed4881&req=cSgmEMp%2FlYNfFb4f3HP0gGm7z6ZH0dQ1%2Bnbu%2BkqBn6QoIa5R5nVJXfeWMvXn%0AJyQ9dwxKeROp2ahoQQ%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

Did this answer your question?

😞😐😃