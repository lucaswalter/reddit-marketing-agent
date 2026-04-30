[Skip to main content](https://help.coinledger.io/en/articles/9505113-how-can-i-import-my-margin-transactions-into-coinledger#main-content)

# How can I import my margin transactions into CoinLedger?

Import your margin transactions into CoinLedger in a few simple steps

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 9 months ago

CoinLedger supports tax calculations for margin trades and allows you to import some margin transactions automatically. If we don't yet support automatic imports of margin transactions from the exchange you're using, you can import your gains and losses from margin trades using the CoinLedger app. Read below for more information on how to import your margin transactions.

## Which exchanges can I import my margin transactions from?

You can import your margin transactions from any exchange using one of two import methods. Currently, CoinLedger supports **_automatic imports of margin transactions_** from Kraken, with support for margin trades on additional exchanges going live in the future. In the meantime, you can import your gains and losses from margin trades from any exchange into CoinLedger manually using the **Add Transaction** button on the Transactions page. Find step-by-step instructions for this process [here.](https://help.coinledger.io/en/articles/9505113-how-can-i-import-my-margin-transactions-into-coinledger#h_f5df514af0)

To import your margin transactions from Kraken, [please see the import instructions in this guide.](https://help.coinledger.io/en/articles/5338231-kraken-ledgers-file-import-guide) Please note that we currently only support importing margin transactions from Kraken through [Kraken's API import method](https://help.coinledger.io/en/articles/5509209-kraken-api-import-guide). Importing margin transactions through Kraken's CSV files into CoinLedger is not possible at this time.

## What is margin trading?

#### Margin Trading explained

When you trade cryptocurrency on margin, you borrow money from exchanges or other brokers to carry out trades. To better understand the concept of margin trading, imagine that you have 1 ETH worth $3,000. If you are using an exchange that offers 3x leverage, you can use your ETH as collateral to borrow up to $9,000. However, if you lose money on a trade and you no longer meet the platform’s minimum margin trading requirements, your collateral could be liquidated.

## How are margin transactions taxed?

#### Details

Although the IRS has not yet provided explicit guidance on how margin trades for crypto should be taxed, we can infer the proper tax treatment from similar asset classes like equities. Generally, profits and losses generated from margin trading are reportable as capital gains and losses, similar to other cryptocurrency disposals. You only have a taxable event when you "realize" a gain or loss from your crypto margin trading.

If you fall under an exchange’s minimum requirements for margin trading, it’s possible that your collateral will be liquidated to cover the exchange’s costs. Margin trading liquidations are considered a taxable event subject to capital gains tax. CoinLedger makes the complicated process of calculating your gains and losses from margin trades simple. To learn more about the taxation of margin transactions, [please see this guide.](https://coinledger.io/blog/crypto-margin-trades-taxes)

## How can I manually import my margin transactions into CoinLedger?

If CoinLedger does not yet support automatic imports of margin transactions from an exchange you use, you can import those manually into the CoinLedger app using the Margin Gain transaction type.

A margin gain transaction is any gain or loss obtained when closing (or while holding) a margin position. We recommend entering a standalone Margin Gain transaction to represent your gains or losses from margin trades. You should only enter a Margin Gain - you do not need to enter a transaction showing you opening or closing a position.

To proceed, follow the step-by-step instructions below.

#### Adding a Margin Gain Transaction

**Step 1**

Navigate to the [Transactions page](https://app.coinledger.io/individual/transactions) and click **Add Transaction**. The Add Transaction menu will now pop up on your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1643861050/0f7d39bf9da5ee63fdf2862ad6e8/Screenshot%2B2025-05-27%2Bat%2B11_24_11-E2-80-AFAM.png?expires=1776713400&signature=42f5e6ab5266c7fbf19d16fe8ee42598b3e4bb622e5fc3dccb56e0885b83e866&req=dSYjFcF4nIFaWfMW1HO4zTUNcluhaG2MVuDsk07jsy1d3hGSi1UOaerFdQTv%0A0Gvb%0A)

**Step 2**

First, under Classification, select **Margin Gain**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1643861592/db96690ee219c58d23d5c995a559/image.png?expires=1776713400&signature=352d78f4311fa699573d9a73f19079585d1a7da479104c68e474b976152cd2be&req=dSYjFcF4nIRWW%2FMW1HO4zTtT1ZV5DzzXmn5DT6JmfZHE1FAwTZ8n5AJw0R1T%0ADdwB%0A)

**Step 3**

Next, you'll need to enter the Timestamp for the transaction (in [UTC time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger)) as well as the Source Account (or wallet) where the transaction occurred.

**Step 4**

Now, it's time to manually enter your Margin Gain or Loss. For this step, you will need to navigate to the exchange or platform where your margin trades occurred.

For example, if you traded on margin on KuCoin, you would first navigate to your KuCoin account and look at the profits and losses for each of your margin transactions. The next step you take here will depend on whether your incurred a gain or loss on the margin trade you are trying to enter.

If you took a loss on a given trade, you would manually add a **Margin Gain** transaction to your account via the steps in Step 2.

Then, you would enter the amount you lost under the **Margin Loss** field, as shown below. In this case, I lost 200 XLM on this margin trade.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1643860105/c6e5a620bbcd1d31fa8d307bcd64/image.png?expires=1776713400&signature=a4b0515d3277f8c1f3a8c69f233acf796afac2945bdc4eff3e6f8ffcec475691&req=dSYjFcF4nYBfXPMW1HO4zU174mOckwUr5OjGA%2F93Ih0Fv92VMSwuAoMSO6fc%0A8AP5%0A)

Now you will see a new Margin Gain transaction on your account showing a capital loss, representing how much you lost on a particular margin trade.

If instead you profited on a margin trade, you would repeat the steps shown in Step 2, but would enter the amount you gained under the **Margin Gain** field instead.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1643860104/1ba4dd02f0b70567bd0008a13170/image.png?expires=1776713400&signature=fb99838540c22098c59ec921e03b5797f31db67328178463065b0d5607da0aea&req=dSYjFcF4nYBfXfMW1HO4zSMzrm9wPEFR3tDi2L%2FEYzG3FFxevMaeLgijaGTj%0Aryml%0A)

Now you will see a new Margin Gain transaction on your account showing a capital gain, representing how much you profited on a particular margin trade.

Once you are done filling out the details of your margin transaction, press **Save**.

While CoinLedger provides you with all the tools you'll need to manually input such transactions into our software on a DIY basis, we ultimately recommend consulting with a tax professional before doing so.

Have any further questions about importing margin transactions into CoinLedger? Reach out to our [Support Team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) anytime!

Did this answer your question?

😞😐😃