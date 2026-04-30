[Skip to main content](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#main-content)

# How can I import bridge transactions?

Learn how to create a bridge transaction in your CoinLedger account

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 9 months ago

## Jump Ahead

- [What is Bridging?](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_5ca7339058)

- [When to enter a Bridge trade transaction into CoinLedger](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_e03eb4e9b8)

- [How to enter a Bridge transaction into CoinLedger](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_725621e1fc)





  - [Merging a Deposit and Withdrawal into a Bridge](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_be6be1bafa)

  - [Manually Creating a Bridge Transaction](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_d1fe7fc4ed)


- [Can I make bridge transactions non-taxable in my CoinLedger account?](https://help.coinledger.io/en/articles/8345587-how-can-i-import-bridge-transactions#h_dd53479e34)


## What is Bridging?

In the context of cryptocurrency and blockchain technology, "bridging" refers to the process of transferring assets between different blockchain networks. Multi-chain bridges are designed to help investors move their assets from one blockchain to another. For example, an investor who holds ERC-20 tokens who wishes to move their assets to the Avalanche blockchain can use the Avalanche Bridge.

## When to enter a Bridge trade transaction into CoinLedger

CoinLedger will automatically detect most bridges without any manual classification being required, but some bridge transactions may not automatically get recognized by our software. In these cases you may need to merge two transactions together to create a "Bridge" transaction, or create a Bridge manually. This will apply the correct cost basis to this asset and prevent a missing cost basis warning from appearing on your account.

#### Example

- Let's say someone bought ETH on Coinbase, and then sent it to their Arbitrum address on 1Inch.

- There, they subsequently wrapped their ETH, where it became Arbitrum ETH (a wrapped version of Ethereum).

- Now, CoinLedger is showing a Missing Cost Basis Warning for their Arbitrum ETH. This isn't due to an issue with CoinLedger, but its due to flaws with the way exchanges and protocols send transaction data to apps like CoinLedger.


**In the situation above, there were three transactions that occurred**:

1. A purchase of ETH on Coinbase

2. A withdrawal of that ETH from Coinbase and a subsequent deposit of that ETH into their 1Inch account (these two transactions occurred at the same time)

3. Finally, the customer wrapping their ETH and it becoming Arbitrum ETH


Without telling CoinLedger that this was a bridge transaction, our app would not know that these transactions were related-and thus, a Missing Cost Basis Warning would appear in this customer's account. You can resolve this by following the steps below.

## How to enter a Bridge transaction into CoinLedger

You can enter a bridge transaction into CoinLedger by merging a deposit and withdrawal pair into a Bridge, or by manually creating a Bridge from the Transactions page.

### Merging a Deposit and Withdrawal into a Bridge

Follow the step-by-step instructions below to merge a deposit and withdrawal into a Bridge.

#### Check the Potential Bridges, Trades and Transfers tab

CoinLedger will identify any potential bridge, transfer or trade transactions that were not automatically mapped upon import on the **[Transactions page](https://app.coinledger.io/individual/transactions)**. Using the **Potential Bridges, Trades and Transfers** tab, you can review each of the transactions CoinLedger has flagged and easily merge them together to resolve any Missing Cost Basis warnings on your account.

CoinLedger will flag each potential bridge transaction in pairs.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609739260/78fef7d340483e5390a67022b97c/image.png?expires=1776713400&signature=e96ebc595ce3ef8c411cb02df3cf1a5dcef5643b35037870385c6640f88d6ef5&req=dSYnH859lINZWfMW1HO4zYHUQAnOPuf6NgBDySXM0hs9%2FF2sGvKjCTxuBN%2FR%0ATbyW%0A)

To merge these transactions together into a Bridge, check the box next to each potential transaction match and then select **Confirm All** from the pop-up menu at the bottom of your screen. This will merge each Bridge together under the transaction type CoinLedger suggested.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609743114/bc7578af88047246d988cf13ba63/Screenshot+2025-07-08+at+12_12_18%E2%80%AFPM.png?expires=1776713400&signature=19e330f4189107c7783f26bc3b370dd6ad419e1c15e319cdcaa80331b0526562&req=dSYnH856noBeXfMW1HO4zW1X58X1WkmQ87yyZKWQb2CM9PLPNqgv3vl6hfzm%0AMCkl%0A)

Finally, to confirm these changes, press **Save All**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609744093/9e00193c7109ae4d9efbbbfbe4dd/image.png?expires=1776713400&signature=c9bd12462df181474664be705ce998149f30836e5bab19d146846e3ff57d8a70&req=dSYnH856mYFWWvMW1HO4zSqNAdwfXInqnF8c9%2FDQWnnJKSg7Zk54rx2ouxpE%0Ag6uX%0A)

Repeat this process for all of the potential bridges CoinLedger has flagged on your account.

If you were expecting to see a Bridge that was not suggested here, don't worry - you can still manually mark the transaction as a Bridge. Move onto the next step for more information on this process.

#### Step-by-Step Walkthrough

**Step 1**

Head to the CoinLedger app, and navigate to the **Transactions** page.

**Step 2**

Filter for the assets and/or platforms in question. Using the above example, the customer would filter their account for the assets ETH and Arbitrum ETH, as well as the platforms Coinbase and 1Inch.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609643603/9ebe5841bcc9f0089eceba468aea/Screenshot%2B2024-10-10%2Bat%2B11_35_06-E2-80-AFAM.png?expires=1776713400&signature=bc8041f6accf1cbfec886f784b5fbd55953aafb03f8003b621e993eb9d4c4cf1&req=dSYnH896nodfWvMW1HO4zcItLb4ZLxYNkeaCNyXWwPfSd1pgWGHqN3veluar%0AVs%2Bn%0A)

Then, identify each Withdrawal and Deposit transaction that show how you bridged the asset - that is, withdrawing the original asset and depositing the new version of the asset on the new chain. The amount and timestamp for this withdrawal and deposit should be similar, if not equivalent.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609643606/32fd5abf081bb6c8fa0c32b0b272/Screenshot%2B2023-09-07%2Bat%2B4_28_42%2BPM.png?expires=1776713400&signature=2efa5ad26a3918b9af40f5cb7e64c3c02f942eb526747d628224fb6d9f26e9b6&req=dSYnH896nodfX%2FMW1HO4zaC5DBE4PWFPYZWv06OqwyqFOm7FqnCkCDBBpcqM%0AmuL4%0A)

Once you've located each transaction, select them as shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609643607/91a02074799634ebfcf951be7fae/image.png?expires=1776713400&signature=0c7aa45e06ead132d5f97a8b20addbd33c5ea78c5c1573b64d13f6694b574aa7&req=dSYnH896nodfXvMW1HO4zY7DUQMiSL47FNnXmsNnXZBeZatVTEl%2BUw%2BIo41V%0AUsw0%0A)

Finally, at the bottom of your screen select **Merge** and then **Bridge**. This will create a bridge transaction between the two assets. In the example from earlier, this action would create a bridge trade of ETH for Arbitrum ETH, and would resolve the Missing Cost Basis Warning on that customer's account.

#### Transactions that cannot be merged into a Bridge

Some transaction types can't be marked as a bridge. These include:

- **Transactions between assets on the same blockchain.** Trying to merge transactions whose assets belong to the same blockchain will result in an error. Instead, you can mark these as a trade.

- **Token updates.** Token updates are not bridges and can't be marked as a bridge within CoinLedger.


### Manually Creating a Bridge Transaction

You can manually create a Bridge transaction from the [Transactions page](https://app.coinledger.io/individual/transactions).

#### Step-by-Step Walkthrough

**Step 1**

Navigate to the [Transactions page](https://app.coinledger.io/individual/transactions) and click **Add Transaction**. The Add Transaction menu will now pop up on your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609685360/6bfb626326a89f4d047bd505aa6f/Screenshot%2B2025-05-27%2Bat%2B11_24_11-E2-80-AFAM.png?expires=1776713400&signature=10e888bdad687e91b7052cae947ec444ba4eaf9f316bbfa15e622e3741f13488&req=dSYnH892mIJZWfMW1HO4zeLWNE854Iyz%2FyA7Zpcw4WV9beUIMRcyaEN5OcyT%0AoZ%2Fn%0A)

**Step 2**

First, select Bridge as your transaction type under Classification. Once you've done this, select **Next**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609695205/b56315fba23bb4326cb440d23a79/image.png?expires=1776713400&signature=e423a61cc21fce82f0d049f10b9b4366f73127cab16194326e90f9457e9be9c7&req=dSYnH893mINfXPMW1HO4zTh6qWDrJ92kd%2F3snvTL%2BPC7Amy5FbCO%2FwCAFYbB%0ABA54%0A)

**Step 3**

After this, you'll need to enter the Timestamp for the transaction (in [UTC time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger)) as well as the Source and Destination Accounts (or wallets) where the bridge occurred.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609697416/b4958e4ded794662484be32f665d/image.png?expires=1776713400&signature=1ab09ce470df39fd3c8ec124a2c6dfbd3253213a3d8ad9af552c28fe65203ff0&req=dSYnH893moVeX%2FMW1HO4zREuqgQI20fUeCQf%2FvkyW194fgstQ9NTI09khVYd%0A0Kgz%0A)

For example, if I sent my ETH from Coinbase to my Arbitrum wallet in MetaMask, (bridging my ETH to Arbitrum ETH), I would select Coinbase as the **Source** and MetaMask - Arbitrum as the **Destination**.

You can select the date and time manually by scrolling to your desired month, day and year or by typing it in directly on the timestamp field. Once you have completed these steps, click **Next**.

💡 TIP: Be sure to use the [UTC date and time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger) for your transaction.

**Step 4**

Now you will need to enter the asset (or coin) that was bridged in this transaction. In the example above, it was ETH - so I entered Arbitrum ETH as the Asset Received and ETH as the Asset Sent.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609711408/b0acd0269a6e7d57840091eedd58/image.png?expires=1776713400&signature=5152d77e74ceece5a3108f0119ee0a560441a7007820868523f90bda4e472c71&req=dSYnH85%2FnIVfUfMW1HO4zWlf72NRCntAS1euabZv8HjCaXEcDAr1NeIFCsBl%0AN9ct%0A)

💡 TIP: You **do not need** to manually set a price for your assets as CoinLedger will automatically set the correct price for you.

Once you have entered the asset(s) and amount(s) in the required fields, continue on to the final step by hitting **Next**.

​

**Step 5**

Finally, you have the option to add any Fees you paid in this transaction. Once you have entered all of the necessary information for this transaction, press **Save**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1609714802/8b1ce4bceaae654fd1c8875758c5/image.png?expires=1776713400&signature=e876955c10edb068d3197eba6f4df695f20f71b02f1c4b7589c95c54907145de&req=dSYnH85%2FmYlfW%2FMW1HO4zdIWvRQnf5k7EYRiDe210yy2teMJs0V6uF38qxqy%0AYEXw%0A)

## Can I make bridge transactions non-taxable in my CoinLedger account?

CoinLedger takes the conservative approach and treats bridging as a taxable token swap, making the fair market value of those bridged/wrapped assets at the time you received them your new cost basis moving forward. If you're interested in learning more about how bridges are taxed, [check out this walkthrough](https://coinledger.io/blog/wrapped-crypto-taxes).

If you choose not to treat bridging as taxable and would like to treat bridging transactions as equivalent to holding the same asset (which would not trigger a taxable event), you can toggle **Treat bridging as taxable** to OFF in the [Advanced Settings](https://app.coinledger.io/individual/settings/tax]) of your CoinLedger account.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1211668084/c3178e1fbae8cf36d46e928bfc44/Screenshot+2024-10-10+at+11_37_36%E2%80%AFAM.png?expires=1776713400&signature=5adceb4685a55fa6b3f56eac7b1dd12e3929256693214ae5140a7fefb5791a03&req=dSImF894lYFXXfMW1HO4zVmS4avqHCKcCt84R%2FM4ZLfBMNnashiLc8Wb5Ixo%0AuQoAv%2FtHEM0FEOEaCwU%3D%0A)

We recommend consulting with a tax professional before making a final decision.

​

​

Did this answer your question?

😞😐😃