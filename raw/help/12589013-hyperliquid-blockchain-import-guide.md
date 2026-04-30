[Skip to main content](https://help.coinledger.io/en/articles/12589013-hyperliquid-blockchain-import-guide#main-content)

# Hyperliquid - Blockchain Import Guide

Import your Hyperliquid transactions with your wallet address and automatically calculate your taxes.

![](https://static.intercomassets.com/avatars/5073255/square_128/IMG_20210823_191315_%281%29-1646924862.jpg)

Written by Caio
Updated today

CoinLedger natively integrates with Hyperliquid to simplify your crypto taxes. By connecting your public wallet address, all of your supported transactions will be imported and classified.

# Jump Ahead

- [Importing Your Hyperliquid Transactions](https://help.coinledger.io/en/articles/12589013-hyperliquid-blockchain-import-guide#h_55201a3434)

- [What transaction types on Hyperliquid does CoinLedger support?](https://help.coinledger.io/en/articles/12589013-hyperliquid-blockchain-import-guide#h_00de2ff703)


# Importing Your Hyperliquid Transactions

To import your Hyperliquid transactions into CoinLedger, you’ll simply need to import the wallet address you use on the Hyperliquid platform.

**Step 1**

First, locate your public receive address in the wallet you used to trade on Hyperliquid. This is typically the address associated with your deposits and trading activity.

**Step 2**

Next, head to CoinLedger. From the **Imports** page, select **Add Account** and then search for **Hyperliquid**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1779878858/498f6cb476a96eb76e9d7b8329bc/image.png?expires=1776816000&signature=ecc48d4c9957e6849df804ba15cd759bd64633514d79c3ec4bc92c9d48701a8a&req=dScgH8F5lYlaUfMW3nq%2BgcTVm2NNf2pstqMCBkOtSEiF6jmjzTEm7np47O5e%0AQYYGSwPpjj9EHZntUqdhA3VxsTQ%3D%0A)

**Step 3**

Paste your Hyperliquid wallet address into the box shown below, and then press **Connect Wallet** to import all of your transactions.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1779883626/4f08cfd5c1ebd55a013ba9f880f5/image.png?expires=1776816000&signature=f189112dff0a86ff8fb401a13b7f19752a16707f6a720a4eddda39a6535e1160&req=dScgH8F2noddX%2FMW3nq%2BgeXn%2FuisIqd7rrvA0GzN9PMdjY0HqswUm13MuApL%0Awz%2F6HTp99vhp1BQoyzqDWntJNqw%3D%0A)

# **What transactions are supported?**

CoinLedger has expanded support for Hyperliquid imports to cover a broader range of on-chain and trading activity. When you connect your wallet, the following transaction types may be imported and classified automatically:

- **Bridge activity (Arbitrum ↔ Hyperliquid USDC)**

Deposits and withdrawals across the Hyperliquid bridge.

- **Vault activity**

Deposits, withdrawals, distributions, and leader commissions (including HLP and user vaults).

- **HYPE staking**

Staking deposits and withdrawals.

- **Liquidations**

Forced position closures, including details on affected positions.

- **Rewards claims**

Claimed incentives and protocol rewards.

- **Spot genesis token events**

Token distributions related to genesis or similar events.

- **Transfers and sends**

Transfers between your own Hyperliquid accounts, including movement between spot and perpetual accounts.


* * *

## **What transactions are not imported?**

Some internal account operations do not represent real asset movements on-chain. These are **intentionally skipped** during import rather than flagged as transactions.

This includes:

- Moving margin between your own spot and perpetual accounts

- Transfers between sub-accounts

- Small internal system or account activation fees


These actions don’t impact your balances from a tax perspective and are therefore excluded to keep your reports accurate and clean.

* * *

## **Notes**

Hyperliquid is a complex DeFi ecosystem that includes trading, staking, vaults, and bridging activity.

Because of this, transaction classification may continue to improve over time as support expands

​

### **Perpetual Transaction Types**

The following perpetual trades are fully supported and will be classified as a profit or loss transaction based on the position's net outcome.

|     |     |     |
| --- | --- | --- |
| **Transaction** **Type** | **Description** | **CoinLedger Classification** |
| OpenLong | Opening a long perpetual position. | Handled as part of the overall Margin Gain/Loss calculation upon close. |
| OpenShort | Opening a short perpetual position. | Handled as part of the overall Margin Gain/Loss calculation upon close. |
| CloseLong | Closing a long perpetual position. | Margin Gain or Margin Loss |
| CloseShort | Closing a short perpetual position. | Margin Gain or Margin Loss |
| LongToShort | Flipping a position from long to short. | Margin Gain or Margin Loss (Represents the combined close of the long and open of the short). |
| ShortToLong | Flipping a position from short to long. | Margin Gain or Margin Loss (Represents the combined close of the short and open of the long). |

**Note on Perpetual Classification**: For futures, derivatives, and perpetuals, CoinLedger records realized gains and losses when a position is closed or flipped. A Margin Gain transaction reflects either a profit or a loss from the position. If the amount is positive, it is added as a profit. If a loss was incurred, the amount will be displayed with a negative sign, as shown in the screenshot below. The system automatically calculates these net figures upon import.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1779899351/82183ad583005e1a89550cb649db/image.png?expires=1776816000&signature=ebfa61eb192b0566cf898ca6c40da422d2e775dc32a11f4093451dde9df03553&req=dScgH8F3lIJaWPMW3nq%2BgRPhBcoOv60lJNIMQsTJi89x1gjbI2VyI%2FQQ3SgL%0AkOCOYNEJ0g%2FBnTE7FGub%2Fc6ZgbM%3D%0A)

Did this answer your question?

😞😐😃