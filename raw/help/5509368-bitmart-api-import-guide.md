[Skip to main content](https://help.coinledger.io/en/articles/5509368-bitmart-api-import-guide#main-content)

# BitMart - API Import Guide

How to automatically import your BitMart transactions into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

CoinLedger only needs "Read" or "View" access to import your trade history. This permission protects your accounts. Learn more about API access in this [article here](https://www.cryptotrader.tax/blog/the-ultimate-guide-to-api-access-for-your-crypto-exchange-accounts).

Jump ahead with this table of contents:

1. [API Import Walkthrough](https://help.coinledger.io/en/articles/5509368-bitmart-api-import-guide#h_ada60bcd07)

2. [BitMart API Limitations](https://help.coinledger.io/en/articles/5509368-bitmart-api-import-guide#h_46d3026815)


## API Import Walkthrough

**Step 1:**

Login to your [BitMart](https://www.bitmart.com/login/en) account.

![](https://downloads.intercomcdn.com/i/o/378180935/66b537f8eb160b016c546903/image.png?expires=1776713400&signature=dceb7cbce64e1cdedd9dfc1d77df73db8d5b8bbe47584fc3e90599a113eb6a8c&req=dycvF8F%2BlIJaFb4f3HP0gHdZ0AIE87YHRoJx64QXz%2FxkfvgmLnUZbGUASWeF%0Agi11rkXwLlyePJ5ICw%3D%3D%0A)

**Step 2:**

Select **Account** from the top-right dropdown.

_Direct Link:_ [https://www.bitmart.com/account/en](https://www.bitmart.com/account/en)

![](https://cryptotradertax.intercom-attachments-7.com/i/o/380245173/fe9b51f85772e7ae05fb2aa0/rhn-XA0hsS06W3_AqZ_Q1KGno0pSCGIzSfMtPKQaq1mSqPYiv-YI3Ra1MFTat4v9I2rebrCE_mu9VOaqWaZ1Wg-NUAbVRXHKYKEKLYnt1vPt2UVTzqfkxe3drNxRXzqL4tMypZBgWCztkUtOOQ%3Ds0?expires=1776713400&signature=e743f18b172f4d221c1a6ca627749ff71a7c77b35f115473cbe09eeab36af5d1&req=dygnFM17nIZcFb4f3HP0gOoSStNkoR5svsoYTu284LFnDJhceIKyxG7Cd5Es%0AMoTTts5zBtmfEqRwZQ%3D%3D%0A)

**Step 3:**

Next, navigate to the the **API Management** section.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1346717520/481edd0c4448d65595cabd631ef9/Screenshot+2025-01-22+at+10_30_10%E2%80%AFAM.png?expires=1776713400&signature=0b691c2f9715859d415772141be1cbf9ff722bdf676851546bb5b01525add34d&req=dSMjEM5%2FmoRdWfMW1HO4zXw7KWREYrcc%2BZeDf4GstVxi07CPEpzZJeyh8h14%0ABhczeO%2Fr9u6heMoK2bA%3D%0A)

_Direct Link:_ [https://www.bitmart.com/api-config/en-US](https://www.bitmart.com/api-config/en-US)

**Step 4:**

Fill out the form to create an API Key:

- **Memo**\- This can be any phrase you’d like, but make sure you write this memo down or save it to a safe place before proceeding to the next steps

- **Read-only -** this will be toggled on by default and it is the only Authority you should set for your API key. Trade and Withdraw _should not_ be toggled on


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1346726913/94bbb44b63fbb80a52a4cbd2bfd6/Screenshot+2025-01-22+at+10_35_01%E2%80%AFAM.png?expires=1776713400&signature=f005ffe7619d9c4b64b112247babb6ed03cd1c51ec559972a61840060de99e8c&req=dSMjEM58m4heWvMW1HO4zSEWJZM2vFJgyCm76xBqkTu5QSuN%2BhSxyxk7jXCR%0AjcwwklXv4QLh2oulB8Y%3D%0A)

Once you've completed the steps above, press **Submit**.

You'll be prompted to complete some necessary verification steps, including an email and 2FA authentication code.

**Step 5:**

Now, your API Access Key and Secret Key have been created. Copy both of these keys to safe place before clicking **Confirm**, as you will not be able to access the Secret Key again. Once you have done so, press **Confirm**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1346748692/7c7b4b15f908658dfe95d5338b08/blurred+keys+on+confirm+step.png?expires=1776713400&signature=941205022c4ccc96c10c720abf6e594e5a34584a09ae74ba4dc6653c4b7bc30a&req=dSMjEM56lYdWW%2FMW1HO4zSvpU6yQLNJiGIs6oMrX3utrMh0brmfP7q%2F3x9lt%0AJWpq5GnjLxMtEitz5uo%3D%0A)

**Step 6:**

In your CoinLedger account, navigate to **Step 1. Import**. Select _Add Account_ then choose the **BitMart** tab on CoinLedger. Click on _Auto-Import_.

Next, paste the Memo you created earlier into the **Memo** field. Then. paste the Access Key into the **Access Key** field, and paste the Secret Key into the **Secret Key** field.

After that, press **Sync Transactions**. Your data from BitMart will now be imported.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1423074223/7db08c99c16d265f127af65b71a5/image.png?expires=1776713400&signature=8326631489e3b017ab8516ea21c90a724406dd04843f34e3787a4b38fa71b006&req=dSQlFcl5mYNdWvMW1HO4zY89NnKam0l4nAaJo%2BBVGq6XiX9rdBpJMDx67ImF%0AsYg1TLXCbuhabSMglMY%3D%0A)

When importing your transaction history via API, you will have the option to specify a start date for your import. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1144576227/2a8ddecd53bf4147102675a6/Screenshot+2024-08-13+at+11_27_06%E2%80%AFAM.png?expires=1776713400&signature=78f5fd1a7da208e81d414c869527848577953835c7b8cfd84fcafba9a4890edb&req=dSEjEsx5m4NdXvMW1HO4zcBUukmAlF4%2BKOJfcMx7dzOdMxYwFwNgQCINWEw%2B%0A73zXIPC%2Fp0ZkpWc%2B3mY%3D%0A)

## BitMart API Limitations

These transaction types are not returned by BitMart's API:

- Staking rewards


These transaction types aren't currently supported by CoinLedger, and will cause your import to fail:

- Margin trades


Please note BitMart has a date range limit on their API calls **which means they only return data from the past 30 days.** As a workaround, we recommend importing via our [Universal CSV template](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide) instead.

Did this answer your question?

😞😐😃