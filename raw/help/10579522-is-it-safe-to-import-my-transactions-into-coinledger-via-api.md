[Skip to main content](https://help.coinledger.io/en/articles/10579522-is-it-safe-to-import-my-transactions-into-coinledger-via-api#main-content)

# Is it safe to import my transactions into CoinLedger via API?

Learn why it is safe to import your transactions via API Keys or OAuth

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over a year ago

### Yes, it is safe to import your transactions into CoinLedger via API!

In order to calculate your capital gains and losses as well as your Portfolio Tracker balances, CoinLedger needs your transaction history data - you can import this data via CSV file, a blockchain wallet address, manually, or via a set of API Keys from a crypto exchange.

For some exchanges, CoinLedger offers a type of API integration called OAuth.

Importing your transactions into CoinLedger via API Keys or OAuth is safe, since CoinLedger only requires "read" or "view" only access to your transaction history data. CoinLedger **never** requires trade or withdrawal permissions for API Keys on your exchange accounts, and will never ask you to input these keys.

Read only API access allows the system that is connecting to an exchange's API to **ONLY** “read” or “view” the transaction history data for that account. This type of granted access is popular amongst portfolio trackers and crypto tax software systems like CoinLedger that need to know your transaction history in order to work properly.

These applications do not need to be able to make trades on your behalf, so they will only require this “ **read only**” access. CoinLedger is no different. CoinLedger never requires trade or withdrawal access from your exchange accounts, only "view" or "read" access.

This means that connecting your API Keys to CoinLedger is completely safe, since our application can never access your funds or other personal data and does not have the ability to.

Furthermore, your personal information is **never** saved into our database.

From within your CoinLedger account, you also have the ability to delete all transaction history data and exchange API connections at any time. Learn more about this process [here.](https://stripe.com/docs/security)

Ultimately, if you don't want to connect your API Keys to CoinLedger, you can switch to CSV import for that exchange instead.

## What is OAuth?

Another type of API import is a protocol called OAuth.

The API integration CoinLedger has with Gemini and Coinbase is built with the OAuth protocol. When you set up an API connection via OAuth, you are logging into your Gemini and/or Coinbase account **directly** **on their website** and then authorizing CoinLedger to view your transactions on a secure, **_read-only_** basis.

As part of an OAuth connection, after you login using your username or password, the exchange sends CoinLedger back a token (very similar to an API key) which is used to fetch transaction history **ONLY**. As a note, our system **never** receives your username or password on any service that is connected via OAuth.

Coinbase and Gemini have built their OAuth protocols with the utmost security and privacy in mind. The API "token" created during an OAuth connection can also be revoked by you at any time. Here's some more information on how OAuth works:

- Gemini OAuth Protocol information: [https://www.gemini.com/blog/geminis-oauth-2-0-support-opens-the-door-to-wider-crypto-usage](https://www.gemini.com/blog/geminis-oauth-2-0-support-opens-the-door-to-wider-crypto-usage)

- Coinbase OAuth Protocol information: [https://docs.cdp.coinbase.com/coinbase-app/docs/coinbase-app](https://docs.cdp.coinbase.com/coinbase-app/docs/coinbase-app)


Still have questions about CoinLedger's security and privacy practices? We recommend checking out this guide [here](https://help.coinledger.io/en/articles/6161888-security-and-privacy-your-questions-answered). You can read this article to learn more about CoinLedger's privacy and security philosophy, and why your data is safe and secure on our platform.

If you have any additional questions, we encourage you to reach out to our [Customer Support Team!](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support)

Did this answer your question?

😞😐😃