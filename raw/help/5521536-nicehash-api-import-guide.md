[Skip to main content](https://help.coinledger.io/en/articles/5521536-nicehash-api-import-guide#main-content)

# NiceHash - API Import Guide

How to automatically import your Nice Hash transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

_CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts)._

NiceHash API Import Walkthrough

Copy link

[Open video in Loom](https://www.loom.com/share/d77e80f941ae4937948f805b241f1c25)

0

1×

1 min 59 sec⚡️2 min 28 sec1 min 59 sec1 min 39 sec1 min 19 sec1 min 10 sec59 sec47 sec

![](https://cdn.loom.com/sessions/thumbnails/d77e80f941ae4937948f805b241f1c25-00001.jpg)

Copy link

[Open video in Loom](https://www.loom.com/share/d77e80f941ae4937948f805b241f1c25)

0

1×

1 min 59 sec⚡️2 min 28 sec1 min 59 sec1 min 39 sec1 min 19 sec1 min 10 sec59 sec47 sec

**Step 1:**

Login to your [NiceHash](https://www.nicehash.com/my/login) account.

![](https://downloads.intercomcdn.com/i/o/456285778/1c898b4ef0874a18f1eb5444/image.png?expires=1776713400&signature=5242054dc3273b62430798d7155824693485a8366da3fc467f195f0295b078fe&req=cCUhFMF7moZXFb4f3HP0gJT8KvBhpdrFxFFjpULf%2BcBZk0Dr3NUf%2Boc039zM%0A1wcgziYXozd7jZXRhw%3D%3D%0A)

**Step 2:**

Navigate to the **API Keys** section under the **Settings Page.**

_Direct Link:_ [https://www.nicehash.com/my/settings/keys](https://www.nicehash.com/my/settings/keys)

![](https://downloads.intercomcdn.com/i/o/380246198/9e479ee5df5dc895e38fbff9/image.png?expires=1776713400&signature=4180463ff88a4ef9da212fbc64a58c3a499bf29c1b621512727e59ae9788c123&req=dygnFM14nIhXFb4f3HP0gJHnKZkwDdacfEmRDZh%2F%2BydFrgIvTlMafsYA67P5%0AUvp6PMQsWy2yqM%2FIqQ%3D%3D%0A)

**Step 3:**

Click **Create New API Key** and fill out the the form with the following settings:

- **Wallet Permissions - View balances, wallet activities and deposit addresses** \- Turn this option on

- **Exchange Permissions - View exchange order -** Turn this option on

- **All other options** \- Turn these off


![](https://downloads.intercomcdn.com/i/o/498546534/97ba55427e64ea9392fe7440/image.png?expires=1776713400&signature=2255b2bfef0c1fcf52c1abcb66f1bb230f731d76c4911beb7ff0abcaf53c2877&req=cCkvE814mIJbFb4f3HP0gC15xcI2r1AajavBUWKWDk%2BrtQ0HPLf2zqQJ%2F42f%0AqN1w6uEGYdFAlzwK7Q%3D%3D%0A)

**Step 4:**

Copy your **API** **Key** and **API Secret** as these values will be needed later.

![](https://downloads.intercomcdn.com/i/o/380246735/a332cea482654bd77aa03b19/image.png?expires=1776713400&signature=53f605dd0884c12a87da98cef13900e669f04d245c29489c14445ab7e6f9fbe7&req=dygnFM14moJaFb4f3HP0gGP04IoKPEp6%2FWf0pR3GlMGMOaZYQk%2F2I7c1Ua30%0A2HxPdl8cdvWOXXDgCA%3D%3D%0A)

**Step 5:**

Follow the on-screen steps to enter your verification code to fully activate the API key. Once activated, copy your **Organization Id**.

![](https://downloads.intercomcdn.com/i/o/380247055/2dc2abccea3f3cb1c932f7c4/image.png?expires=1776713400&signature=95ce6ed48f2d33a58e53229eea93bcfc0849fba0cfeeff2fc41360390f53b1e0&req=dygnFM15nYRaFb4f3HP0gFoxp7u3nTWgAv93%2FZUIlWjoeXzD0a17DhPG6vZ9%0AuL0Lni17wuCJq5xBMg%3D%3D%0A)

**Step 6:**

Navigate to **Step 1. Import**. Select _Add Account_ then choose the **Nice Hash** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key**, **API Secret** and **Organization ID** into the correct fields. Click **Sync Transactions**.

![](https://downloads.intercomcdn.com/i/o/503367679/c69005ba916b76b6fd8a24e0/Screenshot+2022-04-26+at+19.46.11.png?expires=1776713400&signature=83592c366b9d25cde2175ee77fe8c0eb1cd0fd4f3c76d200abb9d7922fa92a2f&req=cSAkFc95m4ZWFb4f3HP0gG3B8TM%2FJQKyHfT39vUkoweVhDZn44L%2B8AwJwUvw%0AvfrJKAOHAlIY02UzpQ%3D%3D%0A)

**Important note**

NiceHash does not export complete transaction data for fiat purchases or sells made on exchange. The API import only includes the crypto amount received or sent does not include the fiat amount. As a result, CoinLedger imports these transactions as Deposits or Withdrawals (non-taxable self-transfers).

Refer to [this guide](https://help.coinledger.io/en/articles/6708304-how-to-edit-a-transaction-to-fix-incomplete-data-exported-by-a-crypto-exchange) for instructions for how to edit the Deposit transaction and change it to a Buy (and with using the same approach you can edit a Withdrawal and change it to a Sell.)

Did this answer your question?

😞😐😃