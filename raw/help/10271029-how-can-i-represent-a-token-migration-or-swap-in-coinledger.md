[Skip to main content](https://help.coinledger.io/en/articles/10271029-how-can-i-represent-a-token-migration-or-swap-in-coinledger#main-content)

# How can I represent a token migration or swap in CoinLedger?

Learn how to represent your crypto tokens undergoing migrations or upgrades in CoinLedger

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 9 months ago

In crypto, it's common for tokens to undergo migrations or upgrades. These could include:

- A project migrates from blockchain to another and users may need to swap their tokens on the original chain for those on the new chain (often referred to as a token migration)

- A project upgrades its smart contract and users may need to swap their old tokens for upgraded versions of the same token (often referred to as a token swap)


## How can I represent a token migration or swap in CoinLedger?

If you engaged in a token migration or token swap, these transactions will typically be imported automatically into CoinLedger, and no manual reclassification should be required. However, if you are importing transactions from a blockchain or protocol which CoinLedger does not have full classifications for yet, your token migration/swap may need to manually imported into CoinLedger.

This is an easy fix! Here's how you can represent a token migration or swap in CoinLedger:

**Step 1**

From within your CoinLedger account, navigate to the Transactions page and select **Add Transaction**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1293788553/f494d3442dd6a9e4b1043baca86a/Screenshot+2024-12-11+at+6_22_24%E2%80%AFPM.png?expires=1776713400&signature=8c2d6d837040cf4dc80090ba1aa24e3fef697073d4ca0d8d1a67ed8c0947ffba&req=dSIuFc52lYRaWvMW1HO4zc47UbBPsckKZcrJJIbwyvBiRMq3fZkvVL%2Bk%2BIda%0Aa3R6SoE0AMWc4KfzdwI%3D%0A)

**Step 2**

Now we'll enter the details of the token swap/migration.

First, select the **Trade** transaction type under **Classification**. Then, click **Next**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1615300624/52c4c2ef9f448de61325678b1337/Screenshot+2025-07-11+at+11_23_18%E2%80%AFAM.png?expires=1776713400&signature=1e1c22c39b9b9c4e9d94300c6da7f05dacfb5a0d7ae290bd0a6a492fe1d5f69a&req=dSYmE8p%2BnYddXfMW1HO4zYUq9gK3lKhXlzF4jpNj53R20mi8ldtg9Rnl4fna%0Aah1emqLBFLYdcaC%2FHQ4%3D%0A)

**Step 3**

Now you'll need to enter the Timestamp of the transaction (in [UTC time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger)) as well as the Source Account (or wallet) where it occurred.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1615299364/c26bb0e5b92e54ee41331d2fa37a/image.png?expires=1776713400&signature=861242df6162f44a7d56beea38691581b6ab19d11895692d19a7faf366e2b866&req=dSYmE8t3lIJZXfMW1HO4zQZ6EmIn4DFHeyZFgcLC1PR1szYuu0eILUHGjTe5%0ApxutpM5Aq7fYvL4wDCw%3D%0A)

You can select the date and time manually by scrolling to your desired month, day and year or by typing it in directly on the timestamp field. Once you have entered a timestamp and picked the source account for your transaction, click **Next**.

💡 TIP: Be sure to use the [UTC date and time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger) for your transaction.

**Step 4**

Now you will need to enter (or coins) you are sending and/or receiving in this transaction. You'll want to enter the old version of the token that is being upgraded/swapped as the asset sent and the new version of the token as the asset received.

For example: if you held the old version of VGX before their token upgrade occurred, you would use VGX (Old) as the Asset Sent and VGX (the new token) as the Asset Received. Make sure you enter the same quantity under **Amount** for each asset if they were swapped on a 1:1 basis.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1615307186/affeba11ceaf2e9ee98c25c29135/image.png?expires=1776713400&signature=477eea928ec88349d6c6ef0f4044d3c3f1bc89a49a49170ae511326e356a5a76&req=dSYmE8p%2BmoBXX%2FMW1HO4zY5F5FggrmTvJItLu0ekoC7poZsPtkd926rMX9hO%0Ad46ffS6an00NwAihxPk%3D%0A)

Once you've added all the necessary information for this transaction, press **Save**.

**Step 5**

Finally, double check that the transaction is marked as Not-taxable.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1615309204/caef70b8cdfbce87ecee394630d9/Screenshot+2025-07-11+at+11_30_57%E2%80%AFAM.png?expires=1776713400&signature=171a2a515afd2835fccabf6a580fce7447ba2675db61b97367b3651da14122ec&req=dSYmE8p%2BlINfXfMW1HO4zXWcysHQq8Fq2vrspv%2B%2BnYwnajjFYnfFGpmNH71J%0AmNH9HGRDIHjb5D0ksBY%3D%0A)

If it is still marked as a taxable trade, you can change this by selecting the three dots next to the transaction and hitting **Mark as non-taxable**. This ensures that the original acquisition date of the asset (pre-migration) is carried over properly after the token migration/swap.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1421464228/7ae01c3750f1f04e11b59bb26cb3/Screenshot+2025-03-13+at+3_43_55%E2%80%AFPM.png?expires=1776713400&signature=c37d738be0dc2639cd1217513dab4966e5e137480930e10af800f98bf7d1df35&req=dSQlF814mYNdUfMW1HO4zUGb%2BVQYaIE6yLGSO2nAcB71VOjtHFg3ckC1N13F%0Ap6FVyyyAMSRxqjZCg8c%3D%0A)

## How are token migrations and swaps taxed?

All token swaps and upgrades are treated as regular crypto-to-crypto trades from a taxable perspective, as you are trading one cryptocurrency for another.

In the case of a token swap or migration, if you swapped an old version of a token for the new version of the token on a 1:1 ratio, then you won't have any gains or losses. You may see a marginal gain or loss depending on the fees disposed of in this transaction.

To learn more about how token swaps or migrations are taxed, please see [this guide](https://coinledger.io/guides/crypto-tax).

Did this answer your question?

😞😐😃