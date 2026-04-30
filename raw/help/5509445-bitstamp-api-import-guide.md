[Skip to main content](https://help.coinledger.io/en/articles/5509445-bitstamp-api-import-guide#main-content)

# Bitstamp - API Import Guide

How to automatically import your Bitstamp transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

_CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts)._

Review the following video for a step-by-step walkthrough on automatically importing your Bitstamp trades to our software, or view the individual steps below!

# Video Guide - Short Version

Bitstamp API Walkthrough

# Video Guide: Long Version

How to Calculate Your Bitstamp Taxes (The EASY Way) \| CoinLedger - YouTube

Tap to unmute

[How to Calculate Your Bitstamp Taxes (The EASY Way) \| CoinLedger](https://www.youtube.com/watch?v=_AyfM1MhJ68) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

# Step-by-Step Import Instructions

**Step 1:**

Login to your [Bitstamp](https://www.bitstamp.net/onboarding/login/) account.

![](https://downloads.intercomcdn.com/i/o/378196470/6b40ee0e25a66bf837a494d7/image.png?expires=1776713400&signature=c2a1c2865fa6311b671beebfff2b8b12e3d3077e8001497f78c3e1d3e3d4fc01&req=dycvF8B4mYZfFb4f3HP0gHBHaLqUNb85nCnPZk5DqMLFynhom9ZsB9i7V9dN%0AmSxXKswLkjW6ZO%2FGtw%3D%3D%0A)

**Step 2:**

Navigate to the **API Access** page: [https://www.bitstamp.net/settings/access-control/api/](https://www.bitstamp.net/settings/access-control/api/)

![](https://downloads.intercomcdn.com/i/o/378197374/a6fd66f1ca06d041ab04ad9e/image.png?expires=1776713400&signature=a4928ece3fcb98f37fd5a3451f58994cd9b5ce52f5ee656b78d3ab6a89ece4ab&req=dycvF8B5noZbFb4f3HP0gPYYFZ1RECWsMxQMZHMR0wDr0m7EX8mcwvK%2BsgQD%0A0QqqBL1wx5ZxJthwdw%3D%3D%0A)

**Step 3:**

Click the **New API Key** button on the **top-right** and turn on the following permissions:

- **Account balance**

- **User transactions**


_This will give CoinLedger **read-only** access to your account and will **not** give access to your funds)_

![](https://downloads.intercomcdn.com/i/o/378198581/97e8d75dbe5716f3775228eb/image.png?expires=1776713400&signature=63da8a04618b5da6185214f8149f976f3008faef8165fb5829d4b73dad275977&req=dycvF8B2mIleFb4f3HP0gDmqQf%2Bq%2FjNtnk7FYyJ1vvQWzWWT1Mix7MpoJdoM%0APeWCbKn5YRC6UqUH2w%3D%3D%0A)

![](https://downloads.intercomcdn.com/i/o/378200569/25cb126af4d35b8f544c4dda/image.png?expires=1776713400&signature=dd8029dbf3f37cf27aa4a600ba302c7dd56aed95a6d03bc91dd4c05054690432&req=dycvFMl%2BmIdWFb4f3HP0gIeH6QyYvBWdaeYK8gfYxFmzF5KDxVxUs3IOh%2B61%0AOPiJvLoamuITneaAlw%3D%3D%0A)

**Step 4:**

After submitting, be sure to copy your **API** and **API** secret as they will be needed to import. Please note that you will not be able to copy the keys again after pressing **Activate**. In the above video, we copy and pasted our API key and secret into the Bitstamp API tab on our website, and pressed **Sync Transactions** so the keys would be saved for later. (the sync will fail since you haven't activated the keys yet, but this is expected). Once both values have been copied, click on the **Activate** button.

After pressing **Activate**, Bitstamp will send you a confirmation email to complete the API key setup process.

![](https://downloads.intercomcdn.com/i/o/378200966/faf2379e5605644f25ce9e5a/image.png?expires=1776713400&signature=f7ab2b773df18954ca4b3235f664e77440c5b4630922b6bab315408fa9bcdddd&req=dycvFMl%2BlIdZFb4f3HP0gECozZR9GRyx6N%2BnBryqrU0oj6xWjIqp45xQWaG%2B%0AXjHdODK%2F5lrCTu%2FZKg%3D%3D%0A)

**Step 5:**

Navigate to **Step 1. Import**. Select **Add Account** then choose the **Bitstamp** tab on CoinLedger. Click on _Auto-Import_ then enter your **API Key** and **API Secret** into the correct fields. (If they were entered into our app before, they should automatically be suggested when you click on the API Key or Secret box.) Click **Sync Transactions,** and now your trade history should come through.

![](https://downloads.intercomcdn.com/i/o/503368374/a92495008c7a32fdc1a9a8a4/Screenshot+2022-04-26+at+19.47.20.png?expires=1776713400&signature=2cec0cb06eb46d67d8f3098b159879dd7a072135769eb55c29ee8ce7e5bfbb15&req=cSAkFc92noZbFb4f3HP0gBbNNhbBDcb7AVRr4M4uxzEw9Mfk35%2BR8MDqtjkC%0AAVFMElbebdcJSSBSvw%3D%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

​

Did this answer your question?

😞😐😃