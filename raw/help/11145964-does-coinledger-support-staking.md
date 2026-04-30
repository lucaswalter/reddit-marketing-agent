[Skip to main content](https://help.coinledger.io/en/articles/11145964-does-coinledger-support-staking#main-content)

# Does CoinLedger support staking?

CoinLedger supports staking transactions as well as staking rewards

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 10 months ago

CoinLedger fully supports staking, but the way your transactions are imported will depend on your method of staking.

Our software supports **native and liquid staking** as well as **staking rewards**.

Native Staking refers to locking up your crypto with a validator. It is usually done within the blockchain or wallet where your assets are held (for example: staking SOL within your Phantom Wallet). These transactions will appear in CoinLedger as Native Stake (when your crypto is staked by withdrawing it from your wallet and locking it up with a validator) and Native Unstake (when your crypto is unstaked and returned to your wallet). Both actions are non-taxable, but any staking rewards earned while your crypto is staked are taxable and treated as crypto income.

In liquid staking, a user receives a token in return for staking their assets. For example, if I stake my ETH on Lido I will receive stETH in return. This token can then be exchanged to unstake my ETH and withdraw it from the staking protocol.

## What staking transactions does CoinLedger support?

Your native staking transactions will appear in CoinLedger as **Native Stake** and **Native Unstake.** Learn more about those transaction types below.

### Native Stake and Native Unstake Definitions

- A Native Stake transaction is any transaction where you staked your crypto by withdrawing it from your wallet and locking it up with a validator. Your staked asset cannot be transacted with until it is unstaked. Many applications or exchanges will pay out staking rewards to your wallet while your crypto is staked. This is a non taxable transaction. However, receiving staking rewards is taxable. Staking rewards are treated as crypto income.

- A Native Unstake transaction is any transaction where you unstaked your crypto and received it back into your wallet. This is a non taxable transaction. However, receiving staking rewards is taxable. Staking rewards are treated as crypto income.


Example: In the image below, you can see that I staked a total of 0.0301 SOL. These were imported as **Native Stake** transactions into my CoinLedger account. Then, a few days later I unstaked my SOL. This was imported into CoinLedger as a **Native Unstake** transaction.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1527567279/e7d9508c9d975e0f38331cb1c604/image.png?expires=1776713400&signature=15cd9d6d97f0745b254c9b6a07f6e125ef726b2433a88f72ddcd84166206abf1&req=dSUlEcx4moNYUPMW1HO4zXotDE0r7nrfwZBmmiR4xp9n2PJzkElwY2i4QR4k%0AwZBn%0A)

CoinLedger also supports Liquid Staking, but these transactions will show up in our software differently. When you stake your crypto with a service like Lido, Marinade or Binance, you will receive a staked token (sometimes called a placeholder token) in return. This transaction may be imported as a Trade or Add Liquidity transaction in CoinLedger. Then, when you unstake your crypto by swapping your placeholder token for the original asset you staked, this may be imported as a Trade or Remove Liquidity transaction.

The IRS has not released clear guidance on liquid staking. CoinLedger takes the conservative approach and treats transactions where you swap your crypto for a placeholder token as taxable. However, you can mark these transactions as non-taxable at your own discretion by following [these steps](https://help.coinledger.io/en/articles/9993812-how-can-i-mark-transactions-as-non-taxable#:~:text=Marking%20an%20Individual%20Trade%2C%20Multi%20Asset%20Swap%20or%20Bridge%20as%20Non%2DTaxable).

## How will my staking transactions show up on the Portfolio Tracker?

For every asset that you have natively staked, you'll be able to see your Staked Balance on the [Asset Balance Report](https://app.coinledger.io/individual/asset-balance-report). This tells you how much of a particular asset you have staked. You will see your Staked Balance next to your Calculated Balance and Cost Basis Balance, as shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1494331101/56fc76992892df197d35be94c295/AD_4nXfJMHhLzcGjwCsjkCzB3tULMx2L5nJL7Kq-ux6NDmfhfNKfY8tI2U_GWfaBeBJBL9l6M7KUKGkWvkCt087OC05mb7jgO9XgRc65UIxTk-gSjJ5FTxIVEmLC0-kPoBkgjlY4RJeknQ?expires=1776713400&signature=f2eb69f7a9103a0429ca1bd619c461b049366e749f5654773e6f189ca1ab689f&req=dSQuEsp9nIBfWPMW1HO4zaYxDgATGCdW0hXSMQoEBf44wpWres%2BLeBBHlvSX%0AQxvT%2B6%2F4lIf0N1h8fTw%3D%0A)

Your Global Calculated Balance for an asset will include the amount of crypto you have staked, but the individual wallet-specific balance for the asset that was staked will not. Learn more about how this works in the drop-down section below.

### How is my Staked Balance calculated?

Calculated Asset Balance is the total amount of a crypto asset we detect in your account across all your wallets (based on your imported transaction data). CoinLedger breaks down Calculated Asset Balance into two types: global and wallet-specific balances. Your Calculated Asset Balance (Global) is the amount of a crypto asset you hold across all wallets on your CoinLedger account, while your wallet-specific Asset Balance is the amount of an asset held in just that particular wallet.

Your global Calculated Balance for an asset (the amount of an asset you hold across all wallets) will include the amount of crypto you have staked. Native Stake and Unstake transactions will not affect this global balance.

However, Native Stake and Unstake transactions will affect your individual, wallet-specific balance for the wallet where these transactions occurred - and they will also affect your Cost Basis Balance.

Here's an example of what this looks like:

- Let's say I have 100 SOL in my Phantom wallet, and then I decide to stake 80 SOL. My Calculated Balance within my Phantom Wallet is 20 SOL, while my Staked Balance within my Phantom Wallet is 80 SOL. This is because this 80 SOL technically left my Phantom Wallet when it was staked.

- However, my overall Global Calculated Balance shown on the Asset Balance Report is still 100 SOL, because the 80 SOL that I staked is technically in my possession and could be unstaked at any time.

- My Cost Basis Balance for SOL will also be 20 SOL (100 SOL minus the 80 SOL that has been staked). This is because when an asset gets staked, it cannot be disposed of or traded away until it is unstaked.


Please note that only crypto which you have staked _natively_ (by sending it to a validator to be staked without receiving another token in return) will show in your Staked Balance. Crypto which has been staked through liquid staking (when you receive a token in return for staking your assets) will not be reflected in your Staked Balance, since you are technically receiving a different asset back in exchange for staking. However, any staking rewards you receive while your crypto is staked will be imported into CoinLedger as Staking Income.

### Example of Liquid Staking in the Portfolio Tracker

For example, if you stake your ETH via Lido and receive stETH in return, your staked ETH will _not_ be reflected in your Staked Balance on the Asset Balance Report for ETH. This is because you received a different asset back (stETH) in exchange for staking your ETH.

To import your staking transactions, you'll first want to start by [importing your blockchain wallet address.](https://help.coinledger.io/en/articles/8404015-how-can-i-import-my-wallet-transactions)

Still have questions about staking? Feel free to [reach out to our Support Team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) anytime!

Did this answer your question?

😞😐😃