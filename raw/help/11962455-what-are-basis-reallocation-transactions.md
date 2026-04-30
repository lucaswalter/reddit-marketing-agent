[Skip to main content](https://help.coinledger.io/en/articles/11962455-what-are-basis-reallocation-transactions#main-content)

# What are Basis Reallocation Transactions?

Learn how Basis Reallocation transactions help transition accounts to Per-Wallet basis tracking.

C

Written by Craig Brentz
Updated over 8 months ago

If you are a US user who has switched over to per-wallet cost basis tracking to comply with IRS revenue procedure 2024-28, you may have noticed new Basis Reallocation transactions in your transaction history.

These transactions are created automatically by CoinLedger when you switch your account settings and are essential for ensuring accurate 2025 tax reports.

### What is Cost Basis Reallocation?

Cost Basis Reallocation is an automated process that occurs when you switch your account from Universal to Per-Wallet basis tracking. CoinLedger will take all your existing tax lots at the end of 2024, and assign them to your platform accounts based on the calculated portfolio balance for each asset and account.

## What does a Basis Reallocation Transaction do?

A basis reallocation transaction shows how the reallocation process changed the cost basis balance for the assets in a given platform account.

Let's look at a simple example:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1659130071/25f57170504ed567512aafb06519/image%284%29.png?expires=1776713400&signature=836db2d171f7e0497bb013d801afbc51d83d34ef408a26621facecdeaa99b665&req=dSYiH8h9nYFYWPMW1HO4zU%2BoLhVhHKYflIsbFiqFCLjzCIaQGvUSSzXkREA1%0AvQI%2BoXegliVLmOjiROY%3D%0A)

This transaction tells us that after CoinLedger performed cost basis reallocation, the cost basis balance of Ethereum in this wallet increased by 1 ETH, bringing the total cost basis balance to 1 ETH.

Now let's walk through a scenario with two platform accounts to see how cost basis gets reallocated between them. Here is the 2024 transaction history:

- Buy 3 ETH on Coinbase

- Withdraw 1 ETH from Coinbase

- Deposit 1 ETH into an Ethereum wallet


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1659133005/e14e5f781d608c5610dbe8ff72b5/image%285%29.png?expires=1776713400&signature=b1983f4c6a85afd937db174205cea24b5039b524e442de56ce80fe4a1ab7c5e8&req=dSYiH8h9noFfXPMW1HO4zSrijLFCUkCwxZSoE2XsijvR39D038XO1kjskkXO%0Azs6%2FEmRKQw1YaNWSJ60%3D%0A)

At the end of 2024, CoinLedger knows a few things about this user’s transaction history.

- They have 3 total ETH of cost basis

- The cost basis balance of ETH on Coinbase is 3, because they bought all the ETH on Coinbase but did not specify the destination of the 1 ETH withdrawal.

- The cost basis balance of ETH on the Ethereum wallet is 0. We know they received a deposit of 1 ETH, but we do not know where it came from, so we cannot determine the cost basis.


Remember that CoinLedger considers Deposits and Withdrawals to be self-wallet transfers that do not affect cost basis balance.

When reallocation occurs, CoinLedger will take that 3 ETH of cost basis, and allocate it across both the Coinbase and Ethereum accounts based on the calculated asset balances that we can see on the Portfolio page.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1659135620/ba8d253d0c0c29e769d4954641bc/image%286%29.png?expires=1776713400&signature=549faa15816c217a2c903241325eac91c3509c0d5bdde95f08ee6056e120e547&req=dSYiH8h9mIddWfMW1HO4zZIoSu7FCxRpLv6glSa63ev4Xu%2B1%2FY7J4LIXKCJY%0AaBp9gPZ7ydyy%2FoIx8bo%3D%0A)

Coinbase has a calculated balance of 2 ETH because the transaction history shows a 3 ETH buy and a 1 ETH withdrawal. Ethereum has a calculated balance of 1 ETH, from a 1 ETH deposit. As a result, CoinLedger can fully allocate the tax lots across each of this user’s platform accounts. Post-reallocation, all balances will be accurate, and this user can proceed with reconciling their 2025 transactions using per-wallet cost basis tracking.

## FAQ

#### **What if my cost basis balance is too low?**

If the cost basis balance for a given asset and wallet is lower than the actual balance in that wallet as of January 1, 2025, you will see missing cost basis errors if you fully dispose of your holdings from that wallet. In order to fix this, make sure that all of your acquisitions are imported and that the balances of each asset on the Portfolio page are accurate.

#### **What if my cost basis balance is too high?**

If one of your platform accounts gets allocated more cost basis than exists in that wallet as of January 1, 2025, you may be missing some withdrawals or disposals that are causing the calculated balance of that platform account to be higher than reality. Ensure that all data, including deposits and withdrawals are imported so that CoinLedger has an accurate idea of the balances in each of your platform accounts.

#### **Can I still fix my older data?**

If anything in your transaction history changes prior to January 1, 2025, the reallocation will run again automatically and these transactions will update accordingly. Be aware that changing earlier data will likely alter previous tax reports, which would require amending earlier filings in order to fully comply with IRS regulations. However, this may be necessary to ensure your 2025 report is as accurate as possible.

If you have questions about your specific reallocation transactions or need help troubleshooting balance discrepancies, please contact our support team.

Did this answer your question?

😞😐😃