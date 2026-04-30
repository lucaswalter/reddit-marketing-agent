[Skip to main content](https://help.coinledger.io/en/articles/5799736-bitfinex-api-import-guide#main-content)

# Bitfinex - API Import Guide

How to automatically import your Bitfinex transaction history.

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

**Step 1:**

Login to your [Bitfinex](https://www.bitfinex.com/login) account.

​

![](https://downloads.intercomcdn.com/i/o/431644866/76fda781b1f9208ee1d53b79/Bitfinex+login.png?expires=1776713400&signature=99ff8b16813c6b3913f68cc0480746476fc7c546822c34d7bfc4b5f3c3f3e3fb&req=cCMmEM16lYdZFb4f3HP0gP%2FM2sdq%2BOq1XIo84qBjdcg9G3CVbCOwNqP7pDwq%0ANEEI3%2B5iAtCMIsKriA%3D%3D%0A)

**Step 2:**

In the top right corner click on the **Manage Account** button (1 on the picture below), then hover over **API Keys** (2 on the picture below) and click on **Create New Key** (3 on the picture below)

​

![](https://downloads.intercomcdn.com/i/o/431703466/cbd9be97c4f234913e5e14a6/Bitfinex+main+page.png?expires=1776713400&signature=1bbb51382cc3389ceb0f9fe0ff0d0e633ea3a0b638b5f66f765a0fb84f4f617b&req=cCMmEcl9mYdZFb4f3HP0gJ9bGZjutyRw17SQvySWwbouovstBVlqd9umHCgL%0AU1wmHyJSIaLLoIhWPQ%3D%3D%0A)

**Step 3:**

On the **Create New Key** tab select the permissions that will be granted through your API key. We only need Account history switched On to successfully import your data (1 on the picture below). As mentioned in the beginning of this article, you can learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts). After selecting the permissions, click on the **Generate API key** button in the bottom right corner (2 on the picture below). Optionally, you can name your key as you want in the box next to the **Generate API key** button e.g. 'CoinLedger API key'

![](https://downloads.intercomcdn.com/i/o/431679062/3524366189facf3d60aebdd0/Bitfinex+Create+New+Key.png?expires=1776713400&signature=b624cc96d177c3a0eac5738cff71a8ed383cc59dbfefcf239839f510e78145ca&req=cCMmEM53nYddFb4f3HP0gM9HKxeI0EocEOOsbVT29Ih%2Fsdnvz5w4Gb5VfKSX%0AraVqkOQBQg6tjAx%2B%2Bw%3D%3D%0A)

**Step 4:**

Enter the 2FA token to authenticate request and then click on **Authenticate** button.

![](https://downloads.intercomcdn.com/i/o/431684731/bbc15677c3cdbe78bcee6d3a/Bitfinex+2fa+for+api.png?expires=1776713400&signature=fd30acd71ada23021664b00755d1abee3d59789bddd7d49f5a825e1b8edb8d87&req=cCMmEMF6moJeFb4f3HP0gKoxfXdk0TW%2BMFu3I5fYTry%2BqpBwHocqqfx4tAsy%0A%2BME0kh0udNpseoQr9A%3D%3D%0A)

**Step 5:**

After authenticating request, you will get an e-mail message similar to the one shown in the picture below. Open message and click on the **CREATE API KEY** button to finish creating API key.

​

![](https://downloads.intercomcdn.com/i/o/431687222/f82674c53abe6eb86337ded2/Bitfinex+api+mail.png?expires=1776713400&signature=80fd479563c24a336895bb90b3a5df7a9bac5294cb497fcaf3f9e56b01af9500&req=cCMmEMF5n4NdFb4f3HP0gLSYXH3eABRBAp2amL7ZkekKST4JmOIYn27IrHTy%0AQ5k%2FpDFnGq0SWQofBg%3D%3D%0A)

**Step 6:**

Once you clicked the button it will redirect you to page showing your **API key** and **API key secret**. Store them somewhere safe as it will not be shown again and you need to provide them so we can import your transactions.

![](https://downloads.intercomcdn.com/i/o/434105684/d6c73a99345d10041c51f041/Screenshot+2021-12-14+at+15.34.48.png?expires=1776713400&signature=cc45221249688a78e9adeb5dd4052c01fb3ac4e876eebaf1e3d5559bd09c5e86&req=cCMjF8l7m4lbFb4f3HP0gO1rjb1Qtkgi0TRhpzTb9laUK%2FpIudlvfOVp7g9t%0AvXZMNfE6w5x6bMlznA%3D%3D%0A)

**Step 7:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Bitfinex** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/503337042/67ddfc2d505f52f110515733/Screenshot+2022-04-26+at+18.57.53.png?expires=1776713400&signature=00996eabfff0c9606e4088f8665d9ec0919660e4c153e9d00bae9dee9e15d902&req=cSAkFcp5nYVdFb4f3HP0gLcmMg%2B5%2F8jdKQZzHMMPe8seCpWrRYTQN2CL9gr3%0A%2BXe%2Fa4kSVYGhap76UA%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

Did this answer your question?

😞😐😃