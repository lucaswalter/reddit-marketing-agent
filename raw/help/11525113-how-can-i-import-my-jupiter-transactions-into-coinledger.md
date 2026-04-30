[Skip to main content](https://help.coinledger.io/en/articles/11525113-how-can-i-import-my-jupiter-transactions-into-coinledger#main-content)

# How can I import my Jupiter transactions into CoinLedger?

Learn how to import your Jupiter transactions into CoinLedger

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 7 months ago

CoinLedger supports Jupiter. You can import your transactions by connecting the SOL address you use on Jupiter to your CoinLedger account. Below, you’ll find a detailed overview of this process and the transaction types on Jupiter we support.

### Jump Ahead

- [Importing Your Jupiter Transactions](https://help.coinledger.io/en/articles/11525113-how-can-i-import-my-jupiter-transactions-into-coinledger#h_48b2656f0a)

- [What transaction types on Jupiter does CoinLedger support?](https://help.coinledger.io/en/articles/11525113-how-can-i-import-my-jupiter-transactions-into-coinledger#h_6e465ae5e1)

- [Can I import my futures, derivatives, or perpetuals trades from Jupiter?](https://help.coinledger.io/en/articles/11525113-how-can-i-import-my-jupiter-transactions-into-coinledger#h_da128e2904)


## Importing Your Jupiter Transactions

To import your Jupiter transactions into CoinLedger, you’ll simply need to import the Solana wallet address you use on Jupiter.

**Step 1**

First, locate your public receive address in the wallet you used to swap crypto on Jupiter.

**Step 2**

Next, head to CoinLedger. From the Imports page, select **Add Account** and then search for Solana.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559199557/38cc7fbd4680fc3744837a76d6c1/AD_4nXeush1I9vpvj5lfZnvDi2McyKtFfhCn-GNu0kpkmNlqIFHCt3awivTHwIbQ8VaCp7LzcdhqDeEk-2z8HOj-9Vil54iKgE9-EFUxPig7WfKhebgTbxCP3St8ZVblOuVACYtfdPpGqQ?expires=1776713400&signature=e0f93d22b785bddf25358010b9ac795755a7b0e32feb3e4bb376a254c70a444b&req=dSUiH8h3lIRaXvMW1HO4zRHxS9MsFpJT%2Fl0nnEVodDonytGbMwUdO%2FXM3Vmg%0AZ9zBb1JwngO3hszRoTM%3D%0A)

**Step 3**

Paste your Solana wallet address into the box shown below, and then press **Connect Wallet** to import all of your transactions.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559199560/11307250b3d82b2ba4a00755bfe2/AD_4nXdnVA5VKckVMZEA0C821ljUiQalZutoouobxgUp-wrveIJ0KSuOCt6eHfOW8EZnX8_-iCCFmNyOgliLBjh2N1SCszSBP_uWz17PoBfhC9lUPR04DO77I1GQKKD6UvI3tghoY4Ky3g?expires=1776713400&signature=0128a4a4b8ff56b2801e18defe31cb17a923a493b335309953ac51bc1f91d234&req=dSUiH8h3lIRZWfMW1HO4zWvxUDfYPBM8u%2FZGABhMZZLX9zCWmfK%2FTIhBimkY%0A1Ti7olMEuikok8o%2BESg%3D%0A)

## What transaction types on Jupiter does CoinLedger support?

CoinLedger supports the following transaction types on Jupiter:

- Swaps

- DCA

- Limit orders


These transactions will be brought in when you import your SOL address into CoinLedger.

### Examples

Here are some examples of what these transactions will look like when imported into CoinLedger.

#### Swaps

Swaps on Jupiter will be imported as Trades in CoinLedger.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559277165/56da66c3e2f2de240b415fcaa597/image.png?expires=1776713400&signature=fd670c03e4ee381840737ff565f24ab28195e24530175182f80d388360347d60&req=dSUiH8t5moBZXPMW1HO4zS%2FHd2LIYvoSVgWRuYdlAr7a4njE%2BGtlMEaapZoD%0Azu7e%0A)

Most of the time, your trades will be classified correctly upon import. However, we recommend checking the [Potential Trades, Bridges and Transfers tab](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab) on your account to ensure that your Jupiter swaps were all classified correctly.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559259116/e24a261a23aff7db4a235bf7fc07/image.png?expires=1776713400&signature=f9176c8fc93970fea9e525c70e3cabc1c2c0f9a673298bd2634d7fb95f312018&req=dSUiH8t7lIBeX%2FMW1HO4zX5BjBaUZoU1ir014V%2Fdu54m6K21TQta%2FJp9ILGW%0AdBzd%0A)

You can accept CoinLedger’s suggestions for each of the potential trades shown on this page. To accept the suggestion and merge these transactions together, check the box next to each potential transaction match, and then select **Confirm All.**

#### DCA

Jupiter allows you to purchase crypto by Dollar-Cost Averaging (DCA). With DCA, you can buy crypto over time by dividing one large investment into smaller, scheduled trades. Jupiter lets you DCA every minute, hour, day, week and month.

For example: let's say I want to buy IBRL every minute on Jupiter. Here's how these transactions will look when imported into CoinLedger, starting with the first partial fill at 8:15 AM:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559286430/d014dea3751a20c9adddc4b88d19/image.png?expires=1776713400&signature=3faee2911a8b221abf5e7a123556a7af9a9c7ef634926ccd685d1eba2b5188c0&req=dSUiH8t2m4VcWfMW1HO4zc95qB5p4mJGQwDNIpVL5OpKMU51S%2BwUvLY2olA2%0APite%0A)

In CoinLedger, every fill of my DCA order is imported as a Trade. I can verify that these Trades are DCA transactions by clicking the arrow next to Transaction ID and opening the transaction on SolanaFM.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559291571/c10c4a23237542aa8adc9042ea7d/Screenshot+2025-06-06+at+11_46_43%E2%80%AFAM.png?expires=1776713400&signature=6ea85ef0503ce5337b484ce2cd0b39dd52271bd8a6ab3697121bae750e68c994&req=dSUiH8t3nIRYWPMW1HO4zcCypzzlzDVuQZnZ2KA0e0UuGCaU3wJECxI8p2g9%0A4dyi%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559292560/3c21a7a20d5dadb3d97949831f81/Screenshot+2025-06-06+at+11_48_07%E2%80%AFAM.png?expires=1776713400&signature=d4c18bdc3fcbf55e3dfb679f8eb24fc8c05e3466c96c79f1798a4d9acafcb41f&req=dSUiH8t3n4RZWfMW1HO4zX0SYHZpwl%2FbosF0xZz8629qzp37DCx2O6kUO6J9%0A88aM%0A)

Initiating a DCA order will be imported as a Fee, while cancelling/closing an order may be imported as a Fee or Deposit.

To learn more about DCA transactions on Jupiter, please see [this guide](https://support.jup.ag/hc/en-us/articles/18734553582620-How-to-set-up-your-first-Recurring-order-DCA-on-Jupiter).

#### Limit orders

Limit Orders on Jupiter allow you to buy or sell a token at a specific price. The platform will automatically execute this trade when the token reaches that price. If there's insufficient liquidity to fill your entire order at once, it may be filled in smaller portions until complete.

For example, let's say I wanted to trade for SOL when it reaches a particular price. Jupiter will automatically execute this trade when SOL reaches that price. This transaction will appear as a Trade in CoinLedger, as shown below:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559357374/5ea8fb5dceb97a30954abdce3a4e/image.png?expires=1776713400&signature=6e112df2f280667d54b175e47767da369c1b31bc31b00f4e13a7f130be969fd3&req=dSUiH8p7moJYXfMW1HO4zdzMiaEESRfhiGp2iWNU%2BBL6QyfRFvNmj6vSqsY2%0Ad6jX%0A)

I can verify that this trade is a limit order fill by clicking the arrow next to Transaction ID and opening the transaction on SolanaFM.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559359340/51cb18c4e473dfa6ed1669fd3d65/Screenshot+2025-06-06+at+12_35_09%E2%80%AFPM.png?expires=1776713400&signature=4d8ef2cb2194ab9d0fbac1f29d011a2824f5e2bdcfb6c876f204ae759794b8b6&req=dSUiH8p7lIJbWfMW1HO4zXU0BzET2MT%2FLFQyJcG9GD%2FUmKJxtMhfkV6Y9pr4%0A5UMs%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1559360574/329d51e17f5c2b35f8b1bf70fc07/Screenshot+2025-06-06+at+12_35_44%E2%80%AFPM.png?expires=1776713400&signature=82963b9e804e05236e9453bcae1c11248dd976a372d873ccb8faeaef2864bff9&req=dSUiH8p4nYRYXfMW1HO4zS4L2COty19%2B1%2BqJjYfzZCmQk%2BsoCnxETfnxye%2F3%0AvshR%0A)

A transaction opening a limit order will be imported as a Fee in CoinLedger, while a fill of a limit order will be imported as a Trade.

To learn more about Limit Orders on Jupiter, please see [this guide](https://betastation.jup.ag/guides/limit-order/how-lo-work).

## Can I import my futures, derivatives, or perpetuals trades from Jupiter?

CoinLedger does not currently support futures, derivatives or perpetuals trades, and these cannot be imported from Jupiter at this time. Support for these transaction types will be available in the near future.

In the meantime, you can manually enter your profits and losses from futures, derivatives, or perpetuals trades into CoinLedger. You can do this by utilizing our Margin Gain transaction type on the **Transactions** page. Learn more about this process below.

#### Manually entering your profits/losses as a margin gain transaction

CoinLedger allows you to enter Margin Gain transactions into CoinLedger. A margin gain transaction is any gain or loss obtained when closing (or while holding) a position. We recommend entering a standalone Margin Gain transaction to represent your gains or losses from margin, futures, derivatives or perpetuals trades. To learn more about this process and to see step-by-step instructions, [please visit this guide.](https://help.coinledger.io/en/articles/9505113-how-can-i-import-my-margin-transactions-into-coinledger#:~:text=How%20can%20I%20manually%20import%20my%20margin%20transactions%20into%20CoinLedger%3F)

**DISCLAIMER:** Before following these steps, we recommend consulting with a tax professional and ensuring that your transactions are represented accurately. CoinLedger is not liable for any mistakes made when entering these transactions, and cannot offer explicit tax advice.

​

Did this answer your question?

😞😐😃