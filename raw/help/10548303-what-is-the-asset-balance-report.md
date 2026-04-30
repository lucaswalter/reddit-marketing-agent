[Skip to main content](https://help.coinledger.io/en/articles/10548303-what-is-the-asset-balance-report#main-content)

# What is the Asset Balance Report?

Use the Asset Balance Report to see how CoinLedger is calculating asset balances across your wallets

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over a month ago

CoinLedger’s Portfolio Tracker tracks the amount, price, market value, cost basis, percentage change, and unrealized return of the cryptocurrencies held across all of your imported wallets. One essential tool to troubleshooting your Portfolio Tracker balances is the Asset Balance Report. **[The Asset Balance Report](https://app.coinledger.io/individual/asset-balance-report)** allows you to view each of the transactions that CoinLedger uses to calculate your balances.

This guide will outline what the Asset Balance Report is and how you can utilize it when troubleshooting your account balances.

# Where is the Asset Balance Report?

To locate the Asset Balance Report, click on the [direct link](https://app.coinledger.io/individual/asset-balance-report) to it in the top right of your Portfolio Tracking page.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1377835822/a23af96630abcd9cf6bb03ad085c/Screenshot-2B2025-01-16-2Bat-2B12_23_23-E2-80-AFPM.png?expires=1776713400&signature=c787aaa411504cf0ada31e6653f98838c8b9c13622d3cf243e3652ac35155720&req=dSMgEcF9mIldW%2FMW1HO4zRbFhe%2BuCLa3nudmKGZHQPwfMLGVDgq0MCk0eBu9%0AlFxCjP9c%2Fu215CphJkU%3D%0A)

# What can I do with the Asset Balance Report?

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1377855423/1af46766708fdbfa16564697a6b6/image.png?expires=1776713400&signature=4b1d82063876b42786fd8e87a218f927f793537004a49005e2923405ebdae61c&req=dSMgEcF7mIVdWvMW1HO4zWo47qS4uCIE15xgJEYKcrQaNhAvaEJvTl8mbs4Y%0Al5FgOoXy5kV178X3Vv4%3D%0A)

### Using the Asset Balance Report, you can:

1. Drill down into your Portfolio Tracker balance for each asset





1. Ex: I want to see my total balance of Bitcoin across all of my imported accounts

2. Specifically, CoinLedger shows you the Calculated Asset Balance and Cost Basis Balance for each asset in your portfolio





      1. **[Calculated Asset Balance](https://help.coinledger.io/en/articles/9001195-what-s-the-difference-between-calculated-balance-cost-basis-balance?q=asser)** is the total amount of a crypto asset we detect in your account across all your wallets (based on your imported transaction data)

      2. **[Cost Basis Balance](https://help.coinledger.io/en/articles/9001195-what-s-the-difference-between-calculated-balance-cost-basis-balance?q=asser)** is the current balance of a crypto asset in your CoinLedger account with known cost basis information (based on your imported transaction data)


2. View how much of a specific asset is held in each account you have imported into CoinLedger





1. In this context, "account" refers to each of the blockchains, wallets and exchange accounts you have imported on the **Import** page

2. Ex: I want to see how much Bitcoin I hold _specifically_ in my Coinbase account


3. View your [Staked Balance](https://help.coinledger.io/en/articles/11145949-what-is-my-staked-balance) to see how much of a particular asset you have staked.

4. View the specific transactions that CoinLedger uses to calculate your asset balances

5. Troubleshoot issues with your data such as inaccurate balances or [negative balance warnings](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#:~:text=deposits%20and%20withdrawals.-,Why%20am%20I%20getting%20a%20Negative%20Balance%20Warning%3F,-If%20the%20debits)

6. Troubleshoot your cost basis for an asset





1. Ex: I'm trying to understand how CoinLedger calculates the cost basis per coin and coins with known cost basis values on the [Cost basis breakdown](https://help.coinledger.io/en/articles/10302709-how-are-cost-basis-numbers-in-the-portfolio-tracker-calculated)


# How can I use the Reported Balance card for troubleshooting purposes?

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1965960066/870be195a9e7bd7c4fad88b601f4/Screenshot+2026-01-20+142137.png?expires=1776713400&signature=e8046e5e468ede143b32c3acbc005672e8300430832d139a79c874ef1aab6945&req=dSkhE8B4nYFZX%2FMW1HO4zQKaVD6hiWtXX3vzuR%2BpVWUhSTVSecFZBhq5Z2FW%0ADsAxZRsPrp4R2NbwNwY%3D%0A)

Under the main Asset Balance Report page, you'll see the Reported Balance amount from your exchange in real time. This value is automatically fetched via API at regular intervals for certain supported exchanges. **_Over time, we aim to enable this feature for most exchanges and wallets that integrate with CoinLedger._**

This feature displays your holdings for the selected asset as reported directly by the exchange or wallet. You can compare this information with the Calculated Balance card to identify any discrepancies between what CoinLedger has calculated and what the exchange or wallet reports. If these numbers don't match, it's a strong indication that there are gaps in your transaction data that need to be addressed.

Here is an up-to-date list of the supported platforms(this will be updated regularly as we launch support for more exchanges and wallets):

* * *

### **Centralized Exchanges**

- Coinbase

- Gemini

- Robinhood

- Kraken

- Crypto.com

- Binance US

- KuCoin

- BitGet

- Bitrue

- BitMart

- NiceHash


* * *

### Decentralized Platforms/Wallets

- Ethereum wallets

- Solana wallets

- Bitcoin wallets (including extended public keys imports)


* * *

# **Troubleshooting Staking & Unstaking Transactions**

If you notice discrepancies in your asset balances, staking and unstaking activity may be the cause.

To help identify and resolve these issues, CoinLedger now surfaces **staking-related warnings directly within the Asset Balance Report**.

* * *

## **Unstake Exceeds Staked Balance**

In some cases, you may see a warning indicating:

**“Unstake Exceeds Staked Balance”**

This means that an unstake transaction in your wallet is **greater than the calculated staked balance at that point in time**.

This can result in:

- Negative staked balances

- Missing asset balances

- Incorrect capital gains calculations


* * *

## **Why This Happens**

This issue typically occurs for one of the following reasons:

- **Missing staking transactions**





Not all staking activity has been imported (for example, missing native stake transactions)

- **Rewards included in unstake**





Some unstake transactions include both:











  - original staked amount

  - staking rewards


In these cases, the reward portion may need to be **split and categorized separately as staking income.**

* * *

## **How the Staking Warning Works**

When this issue is detected:

- A **warning banner** will appear in the Asset Balance Report

- The system flags the **first occurrence** of an unstake transaction that exceeds the calculated staking balance

- Clicking **“View transaction”** will take you directly to the flagged transaction


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/2172465930/47ae8a56f6c7306a6185d75bb3d7/image.png?expires=1776713400&signature=7f1f0e867e7e8ee3e2d552ca0603d4c79f976c4350136808e503be2f618b54b5&req=diEgFM14mIhcWfMW1HO4zYuHweow1x75HUoXrU%2BRFnQfO%2F3sebl6yS3WG959%0Ay1b2bJaLTg7VaD%2BnPt0%3D%0A)

From there:

- Clicking the warning opens a detailed view showing:











  - The amount exceeding the staking balance

  - Additional guidance on how to resolve the issue









    ![](https://downloads.intercomcdn.com/i/o/q3bdiij1/2172479451/5113af795e19f61266981477c49d/image.png?expires=1776713400&signature=7d81677fef8d01e3f53822a13982a3a1f89af351b1c964eb456e2a7e07f21de4&req=diEgFM15lIVaWPMW1HO4zdsG%2BRydzYe0O8qhsV6Uiqy%2FOFUDexaJdFzkia6g%0AnS4l%0A)


* * *

## **How to Resolve This Issue**

To correct the discrepancy:

1. **Verify all staking transactions are imported**











   - Ensure deposits, delegations, and staking interactions are complete


2. **Review the unstake transaction**











   - Confirm whether it includes staking rewards


3. **Split the transaction if needed**











   - Separate the reward portion into a new transaction

   - Categorize it as **staking income**


* * *

## **When Should You Check This?**

You should review staking activity if:

- Your balance is lower or higher than expected

- You see a **negative staked balance**

- You have recently unstaked assets

- You are using staking, restaking, or DeFi protocols


* * *

## **Important Notes**

- The Asset Balance Report reflects your **calculated staking balance at the time of each transaction**, not just your current balance

- This feature helps identify issues that were previously difficult to detect during reconciliation

- In many cases, resolving staking discrepancies requires **manual review and adjustment**


* * *

# How can I troubleshoot an incorrect balance for an asset using the Asset Balance Report?

If you believe the calculated balance for an asset on the Portfolio Tracker is incorrect, there are a few different ways you can utilize the Asset Balance Report to investigate this.

First, pull up the [Asset Balance Report](https://app.coinledger.io/individual/asset-balance-report) and navigate to the asset you would like to troubleshoot.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1377876436/cc4c898f2a36dfa64198218246d2/Screenshot-2B2025-01-16-2Bat-2B12_23_23-E2-80-AFPM.png?expires=1776713400&signature=6479266c39f6df01ca5f3f940252dfc46e86aae5f442aa848fbfd56fc2a2bbbe&req=dSMgEcF5m4VcX%2FMW1HO4zSYFjB5zJTeL8NdQPa8S9NyzndYFXxN563gtL2gu%0AU6tw4YE%2FBmGWqBOvfjs%3D%0A)

Select the **asset** and **account** you would like to troubleshoot. If you want to troubleshoot your balance for an asset across your entire account, leave All Accounts selected. If you'd like to troubleshoot your balance for an asset in a specific account, use the drop-down menu below Select account.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1377878218/588bd9e57917b3b9ddebcef1ed46/image.png?expires=1776713400&signature=07ce89889c12b671002c1a75955b4db36fef3adb049ade993b7784612e68451b&req=dSMgEcF5lYNeUfMW1HO4zVh5SPoy1Gn4zYPhHZrir6pX0LuHsHUHMWRmZ61U%0AGvT2b5caMMENsugVBUI%3D%0A)

**Next, review the Asset Balance Report entry for this asset and look for any of the following issues which can cause incorrect asset balances:**

- **Missing or inaccurate transactions**





  - Missing transactions indicate that you need to update or refresh your imports on the Import page





    - Solutions:





      - Navigate to the Import stage and press the **🔁 Sync All** button

      - If this does not work, you likely need to import a missing data source into CoinLedger


  - Inaccurate transactions could indicate that you made a mistake when editing a transaction or when manually importing transactions





    - Solution:





      - Filter for **Edited** or **Manual** transactions on the [Transactions page](https://app.coinledger.io/individual/transactions) to see if these transactions are correct


- **Large gaps of time missing in your transaction history**





  - If you are missing months or years of transactions for a specific asset that you know you have traded during that time period, this is a sign that you are missing transaction history data and need to update your imports





    - Solutions:





      - Navigate to the Import stage and press the **🔁 Sync All** button

      - If this does not work, you likely need to import a missing data source into CoinLedger


- **Negative Balance Warnings**





  - Negative Balance Warnings are the result of inaccurate or incomplete imported transaction data. To fix them, you should review all of your imported transactions.

  - Using the Asset Balance Report you can pull up the first instance of a negative balance for an asset on your account, making it easy to pinpoint the reason for that negative calculated balance.





    - Negative Balance Warnings will be flagged under the Troubleshooting section of the Asset Balance Report if they are present (if they are not present, you won't see this warning)


- **Discrepancy in your Calculated Asset Balance and Cost Basis Balance**





  - When calculated balance and cost basis balance [do not match](https://help.coinledger.io/en/articles/9001195-what-s-the-difference-between-calculated-balance-cost-basis-balance), this is a signal that you may be missing transaction history data

  - Missing inflows and outflows such as deposits and withdrawals are the most common culprit

  - Learn more about this [here](https://help.coinledger.io/en/articles/9001195-what-s-the-difference-between-calculated-balance-cost-basis-balance)


# Conclusion

Remember that CoinLedger's Portfolio Tracker calculates it's asset balances based on the transaction data that _you have imported_. Your tracked balances may not look correct if your transaction history is not up to date. We recommend taking advantage of the [Asset Balance Report](https://help.coinledger.io/en/articles/8681820-how-does-the-portfolio-tracker-work#:~:text=Why%20are%20my%20asset%20balances%20incorrect%3F) to make sure that all of your calculated balances are correct.

_Still need further assistance?_ Reach out to our Support Team at anytime at [help@coinledger.io](mailto:help@coinledger.io)!!

​

Did this answer your question?

😞😐😃