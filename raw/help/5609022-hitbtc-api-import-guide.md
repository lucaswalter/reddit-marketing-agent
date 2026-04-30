[Skip to main content](https://help.coinledger.io/en/articles/5609022-hitbtc-api-import-guide#main-content)

# HitBTC - API Import Guide

How to automatically import your HitBTC trades into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

​

​ **Step 1:**

Login to your [HitBTC](https://hitbtc.com/signinapp) account.

![](https://downloads.intercomcdn.com/i/o/396112395/45a58f5d36f005edb727843a/image.png?expires=1776713400&signature=b9fb9ac401f005c288a80c19d5cb242cded30b30618ded8df4b139cabb2338df&req=dykhF8h8nohaFb4f3HP0gFiuHqGmNyDEM95ZIfJ5FcmMOagrvsFqIgwMQoWD%0AqM0K1n6Mh%2BUowbYD%2Fw%3D%3D%0A)

**Step 2:**

Click the setting icon in the top right corner of the page.

​

![](https://downloads.intercomcdn.com/i/o/396133563/f9892eb847196212284a4381/image.png?expires=1776713400&signature=22f78a4def35030ce74f73f20edbb822b31d18719f7ead0f34b0729cd3febb95&req=dykhF8p9mIdcFb4f3HP0gPia7xoGiHQauVfCt%2F2hSELn%2Flc9vJhBiRuivZqp%0AB6c0XyPIukoNTp%2BBog%3D%3D%0A)

**Step 3:**

To enable Two-Factor Authentification (2FA), click on **Security** tab and under **Two-Factor Authentification (2FA)** section select **Add GAuth** method.

![](https://downloads.intercomcdn.com/i/o/396134412/b5b0114f018d401ae719a9f1/image.png?expires=1776713400&signature=9d006c1ae0211262474cb20cb901887bef1fbe5bdfa3767a2cd6b5f9df49bdc3&req=dykhF8p6mYBdFb4f3HP0gC%2Fdn11y55zXKZZrfgvO5Nj%2BXRgOj7uF4xdFsi4I%0ANXCKxiGkbbR5QGBGJQ%3D%3D%0A)

Write down your backup code, click the checkbox and then click **Confirm.**

![](https://downloads.intercomcdn.com/i/o/396141430/27a4c7c52d0edf3f75c71870/image.png?expires=1776713400&signature=157bed0af1efbcfba56d324b5dc0e9e3fae0bc0d007bbd3cad9a0619f3738ec3&req=dykhF81%2FmYJfFb4f3HP0gNGFZxhmIr48w%2FTzd3Zhb0zRbWPvXMCqFiFvg6Rr%0AmcSn6WNWqw3ylwtIJg%3D%3D%0A)

After that, open **Google Authenticator** on your mobile phoneand scan code that you see on your screen, and click **Next**.

​

![](https://downloads.intercomcdn.com/i/o/396145592/7684653de9a8e58a6e9abd81/image.png?expires=1776713400&signature=1b0faace895b3fabd8b2336995081ff3140976d78d021ff477caada275ba82af&req=dykhF817mIhdFb4f3HP0gNWXoLpUwGKvieKrydt93R%2BCwdypVD8VHbPyOPs7%0AbGW1tXeG5qCfraimDQ%3D%3D%0A)

Then enter the six-digit code from your device.

​

![](https://downloads.intercomcdn.com/i/o/396146440/240ac2a4760aebac7c1894dd/image.png?expires=1776713400&signature=379cb5ea73d401f3eb8f6655b4fdf77397cbbfe7df14dfc993309b03be03657a&req=dykhF814mYVfFb4f3HP0gOdhot2E9T5%2BwQu1Gc6c%2FKtvZ%2FRpS90ZeOmsW80w%0A%2Faw3QUaCj5f0wOOyHQ%3D%3D%0A)

To finish the 2FA setup, open a confirmation email and verify it.

​

![](https://downloads.intercomcdn.com/i/o/396147002/af5d236c1fde450225720b22/image.png?expires=1776713400&signature=1d7257d3c621c3a51097208cccac470cc3c8b4f5a4202b0108cb588e05dc0236&req=dykhF815nYFdFb4f3HP0gHGcJGnA588SA6c8IDgetsO3SZ488sb8bG2NoaMc%0AF2yD%2F7713W9s%2FbWZXA%3D%3D%0A)

**Step 4:**

Click on the **API Keys** tab and click the **New API key** button.

​ **_Note:_** _If you have **subaccounts**, you will need to create a separate API key for every one of them by selecting them in the **Select Account** menu. Later simply import every subaccount in a separate HitBTC tab inside CoinLedger._

![](https://downloads.intercomcdn.com/i/o/413418033/1c617254093a02d0d38497cc/image.png?expires=1776713400&signature=703910f93a9ac58fc21154f057cddb04b5700d2dd367d3c05d2fe1f6fa0d8fa4&req=cCEkEsh2nYJcFb4f3HP0gPZ%2FDnkCQ4CEWM%2FMMKHjv0RKoqN2Z2za8PC34U%2BC%0A7X%2BrabkbFN5ei9JB0Q%3D%3D%0A)

This window is displayed after API key is successfully created. It is important to save your **API Secret** and **API secret** somewhere because they are visible only while creating the **API Key**.

​

​

![](https://downloads.intercomcdn.com/i/o/396148974/078f28ba10016aa06a314f52/image.png?expires=1776713400&signature=4f0006d4d3ab3a3921a16e196962179fdf676a79b155a89e075c6a7a80b3a391&req=dykhF812lIZbFb4f3HP0gCYUPobTs4w5IScHzLtWmvgEq%2BXOMyKG3Mj%2FPmzV%0ANKtzKYdqoatfHIjRoQ%3D%3D%0A)

After that, click on the **Order book, History, Spot balance** and **Payment information** checkboxes, and enter 2FA.

​

​ **Important note: Make sure you clicked on both checkboxes.**

![](https://downloads.intercomcdn.com/i/o/447005733/dc0d2c0f6aec5c7a848f1057/image+%288%29.png?expires=1776713400&signature=04ea13c288bf8fe44b1002c37386393ce6edbbf05878e41adbe70d062b83c593&req=cCQgFsl7moJcFb4f3HP0gOKhEWeZWdoyci1%2BtkKbkxyHDYS7u%2F73krUsfVGW%0AqxV6Ndjga8wwbTQooQ%3D%3D%0A)

**Step 5:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **HitBTC** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/503364748/1dd77d18d14db9ad7a0d519c/Screenshot+2022-04-26+at+19.41.00.png?expires=1776713400&signature=7cb89b70efdb37a0cb3ef1fe677121c5b245e5904bad19cc3da30ab35b4a0498&req=cSAkFc96moVXFb4f3HP0gAtU7Ho28bK%2BImI%2FCdP8bbVLjPp9KqLy5wwjxxx9%0ATgvQoOEJ%2F77MmTzEwg%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

Did this answer your question?

😞😐😃