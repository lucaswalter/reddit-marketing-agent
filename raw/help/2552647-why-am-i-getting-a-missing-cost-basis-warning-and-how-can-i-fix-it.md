[Skip to main content](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#main-content)

# Why am I getting a Missing Cost Basis Warning, and how can I fix it?

Learn why Missing Cost Basis Warnings occur and how to resolve them

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 6 months ago

Missing Cost Basis Warnings happen when you haven't shown CoinLedger how you originally purchased or otherwise acquired a certain cryptocurrency.

When this is the case, there is no way for CoinLedger to know what your cost basis in that cryptocurrency is.

These warnings are _almost always_ caused by missing data. It's likely that you haven't imported all of your necessary transaction history needed for calculating your taxes. Learn more below about why Missing Cost Basis warnings occur and how to resolve them using CoinLedger.

## JUMP AHEAD:

- [What is Cost Basis?](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_1a92fe8268)

- [Why Do Missing Cost Basis Warnings Happen?](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_50575d0273)

- [How Do I Fix My Missing Cost Basis Warnings?](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_c2268b3c9b)

- [What if I am still unable to resolve my MCB Warning after following these steps?](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_fddb5799b8)

- [Frequently Asked Questions](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_876025470e)


# What is Cost Basis?

Cost basis represents the original value of an asset for tax purposes. It is used to determine your capital gains/losses incurred whenever you dispose of your crypto (trade or sell).

Put another way, cost basis typically represents how much money you put into purchasing your crypto (i.e. how much it _cost you_).

If you bought 1 Litecoin for $250, your cost basis is $250 per Litecoin.

If you later trade this Litecoin when it is worth $300, you subtract your cost basis from the $300 to arrive at your $50 capital gain from the trade. This is how crypto tax calculations are done at a high level. [More info here](https://cryptotrader.tax/blog/the-traders-guide-to-cryptocurrency-taxes).

# Why Do Missing Cost Basis Warnings Happen?

CoinLedger works by importing all of your buys, sells, trades, and crypto related transactions across _all_ of your cryptocurrency platforms. The application normalizes all of this data and sorts it chronologically.

When CoinLedger detects that you are selling or trading a cryptocurrency that it does not have any record of you ever acquiring, it flags the transaction as a Missing Cost Basis (as you are missing your cost basis for this sale/trade of the particular cryptocurrency).

## Why doesn’t your software automatically know my cost basis?

Most of the time it will - _if you have imported all of your transaction history data into CoinLedger_. Our system can only calculate profits and losses based on the information that you have imported. Like any software, we’re not able to generate fully accurate calculations based on inaccurate or incomplete data. If you leave out information, our software will not be able to calculate the gain or loss on your trades. This is why it’s critically important to import ALL of your crypto transactions for ALL years you have traded.

### Click here to learn why CoinLedger needs your entire transaction history.

Consider the following example:

- 1/1/2020 - User purchases 0.5 BTC on Coinbase for $10,000


- 3/1/2020 - User transfers his 0.5 BTC to Gemini where he sells it for $20,000


Let's take the transaction history of the user above as an example. Pretend that this user only imported his Gemini trading history into CoinLedger and ignored his other data. In this case, CoinLedger will only have data on a 0.5 BTC deposit into the Gemini account along with a sell transaction of BTC for USD at $20,000.

This would trigger a Missing Cost Basis Warning as the user has not shown our platform how he originally acquired that 0.5 BTC.

To CoinLedger, it looks like this 0.5 BTC just magically appeared in the users' Gemini wallet. Without the original purchase transaction data from Coinbase, the user's true $10,000 cost basis in his 0.5 BTC will be missing.

## What’s the fix for this? Importing the user’s missing transaction history data.

If the user imports all of his data from both Coinbase and Gemini, CoinLedger will be able to see that the user originally purchased this 0.5 BTC for $10,000 prior to selling it on Gemini.​

When the user then sells this BTC on Gemini, CoinLedger will be able to accurately calculate his correct capital gain using the cost basis applied from the original Coinbase purchase: $20,000 - $10,000 = $10,000.

# How Do I Fix My Missing Cost Basis Warnings?

- Step 1:Import your missing transaction history data - be sure to import all the exchanges, blockchains and wallets you have used to buy, sell and swap crypto over the years

- Step 2:Follow along with the step-by-step instructions on the [MCB Troubleshooting Tab](https://app.coinledger.io/individual/missing-basis-troubleshooting)


As mentioned above, your Missing Cost Basis Warning is likely resulting from missing data. To fix your warning, _you simply need to import or classify whatever data is missing._ Importing your missing transaction history data can include uploading a transaction history CSV file from an exchange you have not imported yet, importing a missing wallet address, or connecting one of your exchange accounts to CoinLedger via API. For any exchanges that we do not offer CSV file or API support for, you can import these transactions into CoinLedger [manually](https://help.coinledger.io/en/articles/2584884-how-can-i-manually-import-transactions-into-coinledger).

## Step 2: The MCB Troubleshooting Tab

If you have verified that all of your imports are current and up-to-date, the next step is following along with the step-by-step instructions on the [MCB Troubleshooting Tab](https://app.coinledger.io/individual/missing-basis-troubleshooting).

Here, you can view each asset on your account that has a missing basis along with step-by-step instructions on how to fix it.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1586486760/c712943032632bf95fa6834beb34/image.png?expires=1776713400&signature=22d312d24ab2ccfe64166e0e03b34190b824734dea7229f357a1518ecd69d859&req=dSUvEM12m4ZZWfMW1HO4zV5eBeYLifXVMTX2ci%2B8hQ%2BXQ1gQLB%2BC5oO6C%2B8%2B%0AmLJ6lH9xcH0wZfbtAYM%3D%0A)

To begin, first select which asset you would like to troubleshoot using the **Select asset** drop-down.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1587732719/2b2952630412a7742432bc49772c/image.png?expires=1776713400&signature=260da80353127f8dcc9414e6a34729cbd0f5d4064c4b4c5972ae94744ae5166d&req=dSUvEc59n4ZeUPMW1HO4zVz7V98NWC%2FMd1%2F5IgxFJPNupTYZ73LmFrQgUZ8d%0ACv5X5M92TgjsJjzwh5U%3D%0A)

Then, follow the step-by-step troubleshooting flow on your screen. You can click on each step to expand the instructions.

​

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1586489979/6858eac1888a3520dbc7fb6d4fa9/image.png?expires=1776713400&signature=dc40ab90af666cafeba07d56cd44456cf04aa7f8071a8d0c76a5c2f6a61e56ad&req=dSUvEM12lIhYUPMW1HO4zfbsbVT4e4U6bYm3LrS8ZJiOAP9Liqmf7KYffVJN%0A5IB55BXBnBCbwEMUujc%3D%0A)

💡 TIP: Make sure to complete this step-by-step troubleshooting flow for **_each asset with a missing basis_** **_on your account_**.

​

### Step 1: Verify Portfolio Balance

On this step, CoinLedger will highlight any issues with your imported data that are contributing to your missing cost basis.

We will also prompt you to review your Calculated Balance for this asset (shown at the top of your screen) to ensure that it matches what you see in your exchanges and wallets. Double check that your Calculated Balance shown here matches the balance shown in your wallets - if it does not, this likely means that you are missing data and forgot to import a wallet or exchange into CoinLedger.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1600213616/d9a92f1226da7b8b7e03b1a4be57/image.png?expires=1776713400&signature=b444187cd2bc4f760d0009fe3dfff7646327e3cbd17deb2f0dd39f1f958ba11f&req=dSYnFst%2FnodeX%2FMW1HO4zToSqqqSjMEqV2fjVTKsDZE7s3Jxps5YReyl5Zgs%0AWldm%0A)

Additionally, if CoinLedger has highlighted any issues with your imported data you will see a prominent Warning banner appear on Step 1, as shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1600222737/a3d83cc3d263fadc76372c1ff2b8/image.png?expires=1776713400&signature=237f208666fad9d777c570a58f55c95c519e49a4fda1c0f2259767228a251391&req=dSYnFst8n4ZcXvMW1HO4zbSmt3eLREDZAf%2Ft7N4jRalYBtOD8E2U04lqUHCK%0AMZ%2Fh%0A)

Click on Step 1 to expand this banner and review the issues CoinLedger identified with your imports. We recommend addressing these issues before continuing on to the next step. These issues may include an account that you have not [imported any data](https://help.coinledger.io/en/collections/1998022-import-stage) for yet, [duplicate imports](https://help.coinledger.io/en/articles/10416095-what-should-i-do-if-i-have-duplicate-transactions-on-my-account), and more.

For example, on my account CoinLedger flagged that I have not imported my Optimism data yet. To resolve this, I would click **Go to Account** and then import my Optimism address.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1586522730/d6852db75eeee3591c2ccf302495/image.png?expires=1776713400&signature=7fab2d3e373fda0aba28cf54917d0805fdac4890e6520f9388b3c65f4a9a65e1&req=dSUvEMx8n4ZcWfMW1HO4zZ3AWj3xbsWZn0myQyypSXSQuCZFwBxSHogRiN5k%0A8DQD%0A)

Once you have completed all of the recommendations shown on Step 1, you can move on to Step 2.

### Step 2: Review Potential Trades / Bridges / Transfers

On this step, CoinLedger will flag any potential bridge, transfer or trade transactions that were not automatically mapped upon import. Merging these transactions together ensures that your cost basis is represented correctly in CoinLedger.

To merge these transactions together, navigate to the Transactions page and click on the **Potential Trades / Bridges / Transfers** tab. Then, follow [these steps](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab).

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1586506058/69017ce0d17738b49e46b660d9c5/image.png?expires=1776713400&signature=191fba1ec4cfa7c15a5bab3abf9793243b5ad43515e334707e8783afa9d19b5a&req=dSUvEMx%2Bm4FaUfMW1HO4zQ1iG9r9%2B8R9yeCqfCY2f8FMWfIbnbfBWUVnRRl3%0ABmNJ%0A)

CoinLedger will let you know on this step _if there are no unmatched_ trades, bridges or transfers on your account for your selected asset. If that is the case, you can move on to the next step - though we still recommend reviewing your deposits and withdrawals manually to ensure that no bridges or trades were missed.

​

### Step 3: Classify Deposit, Withdrawal and Uncategorized Transactions

On this step, CoinLedger will prompt you to classify your deposits and withdrawals as well as your uncategorized transactions. If you have any uncategorized transactions or deposits and withdrawals to review on your account, they will be highlighted here. Follow along with the steps on your screen to address these issues.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1586529199/ce31fd8c8dd20e593d777ce52882/image.png?expires=1776713400&signature=ba04dc4ffef1997dbf1775fafcf02e86ed26d0a35017c6a59bd40bf37cac247d&req=dSUvEMx8lIBWUPMW1HO4zWXgZrsnTcQYjYjliXNrzfCMsGYc5nrEtaYgkC9k%0Azj7C%0A)

Here are some of the issues you may see highlighted in this step:

- **Uncategorized Transactions:** If your wallet transacted with a smart contract or decentralized app that we don’t have a native integration with yet, the transaction will be classified as **Uncategorized** in CoinLedger. Uncategorized transactions may also appear when you import a transaction type that CoinLedger doesn't automatically recognize. Learn how to classify these transactions in [this guide.](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions)

- **First Inflow Missing Basis**: These warnings occur when CoinLedger detects that you have deposited or transferred crypto into your wallet, but you haven't shown us how you originally purchased or acquired it. When the original acquisition for the asset has not been imported, there is no way for CoinLedger to calculate what your cost basis is for that asset. Therefore, it is flagged with an Inflow Missing Basis warning. Learn how to resolve these [here](https://help.coinledger.io/en/articles/6811823-how-to-fix-first-inflow-missing-basis-warnings#h_cc63713424).

- **Review Deposits:** Transactions like trades or income events (such as income from mining or staking your crypto) may sometimes be imported into CoinLedger as simple deposits and withdrawals. In Step 3, CoinLedger will flag any deposits and withdrawals in your account that should be reviewed. Scroll down below Step 3 to find these, as shown below. Learn what to look for when reviewing these deposits and withdrawals [here](https://help.coinledger.io/en/articles/5915504-when-do-i-need-to-manually-classify-or-fix-my-crypto-transactions).


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1588388470/850e4b99c5625f2c7cef901c7a30/Screenshot+2025-06-25+at+3_22_23%E2%80%AFPM.png?expires=1776713400&signature=b9da7a5291b4afc6b45c93861cf85d1bc7ea5dca72b9a0ebd9725c1993e5fcce&req=dSUvHsp2lYVYWfMW1HO4zeCVQzu3JuZPLKzPYApEQ9aVqyrwgPanJb9dufsb%0A6sdY%0A)

​

# What if I am still unable to resolve my MCB Warning after following these steps?

If you have followed all of these steps but are still unable to resolve your missing cost basis, CoinLedger does allow you to manually enter your cost basis by creating a Manual Position. You can enter a **Manual Position** for any asset that is missing its cost basis on the Transactions page.

You can also ignore a Missing Cost Basis Warning. When you ignore a missing cost basis, you'll no longer see warnings for that specific asset on the Transactions page. This is [allowed by the IRS](https://help.coinledger.io/en/articles/2865416-can-i-file-my-taxes-with-an-unresolved-missing-cost-basis), but it may result in higher capital gains on your tax report.

Click on the drop-down menus below to learn more about these features:

### Entering a Manual Cost Basis Position

**Step 1**

Head to the Transactions page of your CoinLedger account. Next, select the **Add Transaction** button. Then, on the pop-up menu select the **Position** tab. This is where you will create your Manual Position transaction.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1555549311/dc5c95f34255bc3421ac25a02cc5/Screenshot%2B2025-06-04%2Bat%2B9_22_06-E2-80-AFAM.png?expires=1776713400&signature=2aad7d8630147ef1a1e4ca3214bceec2d79b0f3f3a8dbd330ca79a53cc257ce7&req=dSUiE8x6lIJeWPMW1HO4zcgLN0%2FzSd%2FLtGtvVMxuBvsjg1kLbD3NewSIKZ9s%0AEbh1%0A)

**Step 2**

First, you'll need to enter the Timestamp of the position (in [UTC time](https://help.coinledger.io/en/articles/10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger)) as well as the Source Account (or wallet) where the position was created.

You can select the date and time manually by scrolling to your desired month, day and year or by typing it in directly on the timestamp field. Once you have entered a timestamp and picked the source account for your transaction, click **Next**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1555549305/be23a21866443e216aae045d0ec9/image.png?expires=1776713400&signature=8e942ffd34c94c7dc9ab4f7c402f772d1894639ab12cfa4dc086b08e58031208&req=dSUiE8x6lIJfXPMW1HO4zYbxT4%2BEEEAsBEXmIas%2FQ1x7uupPy7MGREMGNgOK%0AckoY%0A)

**Step 3**

Next, you'll enter the details of the position you are creating. Make sure to fill out each of these fields:

- **Fiat Currency:** The fiat currency which you exchanged for crypto.

- **Cost Basis:** The price that you paid in the above fiat currency for this crypto.





  - Ex: If you bought 1 ETH for $1,000, your cost basis is $1,000 per ETH.


- **Asset:** The crypto asset which you purchased/are entering a Manual Position for.





  - Ex: If I bought 1 ETH for $1,000, I would enter ETH as the asset.


- **Amount:** The amount of crypto which you purchased/are entering a Manual Position for.





  - Ex: If I bought 1 ETH for $1,000, I would enter 1 as the amount.


![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1555549307/e39192be11be4b2be13425434272/image.png?expires=1776713400&signature=e33c686474e32a85f3a7bb396676c4b15fee20a804ded7dee8dc63ded2e3d606&req=dSUiE8x6lIJfXvMW1HO4zb8rCqX07cXJq55PuCRTuda7oZQmtU4B6gfhCbDM%0ASWZU%0A)

**Step 4**

Once you have entered each of the necessary fields for your Manual Position transaction, select **Save**. Your Manual Position will now been created for the asset you selected. You can locate this transaction by filtering for your Manual Positions on the right-hand side of the screen under Transaction Type, as shown below:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1555549315/290645d409975ccb1802a1633e05/Screenshot-2B2024-11-03-2Bat-2B1_27_02-E2-80-AFPM.png?expires=1776713400&signature=66f7803aeba9c7dac5ec5a7e42292c3d66aac969222162d8073e35f887e7ce37&req=dSUiE8x6lIJeXPMW1HO4zULklbh4VDLZaFaZXHkJkPB%2BdtbiDBp%2FEzUYTx2t%0AOXg9%0A)

You can edit or delete this Manual Position at any time by selecting the three dots next to the transaction and selecting **Edit transaction** or **Delete**.

### Ignoring a Missing Cost Basis Warning

You can ignore a Missing Cost Basis Warning by following the steps below. When you ignore a warning, CoinLedger will no longer show you missing cost basis warnings for disposals of that asset. You may see warnings pop up for disposals of that asset in later tax years, however.

For example: if I ignore a MCB warning for ADA in 2023, I will no longer see any missing basis warnings for ADA on my 2023 tax report. But If I import new data in 2026 that contains disposals of ADA, I may see a missing cost basis warning pop up then.

Ignoring a missing cost basis is allowed by the IRS, but it may result in higher capital gains since our system will assign a cost basis of zero dollars to these assets. If you are willing to accept these potentially higher gains and move on from this missing basis, you can ignore it via the steps below:

**Step 1**

First, identify the warning you'd like to ignore. You can do this from the [MCB Troubleshooting Tab](https://app.coinledger.io/individual/missing-basis-troubleshooting) by clicking **View** and jumping to the first disposal of that asset with a missing cost basis.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1784119853/fdc7c33b93895a95c59653aef03f/Screenshot+2025-10-17+at+3_06_18%E2%80%AFPM.png?expires=1776713400&signature=0a210be004fd78a023e5313453ae1761626f979c512043f53ca57b923bb59ea5&req=dScvEsh%2FlIlaWvMW1HO4zfZeC8XZsr9gL4uSsh05p1zSmzou09B8TPU68WAN%0Ajjgb%0A)

You can also do this by clicking on a specific warning from the **To Review** tab (located on the Transactions page).

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1784122118/5eaf17bd6b48bdac9107c5347b8f/Screenshot+2025-10-17+at+3_07_32%E2%80%AFPM.png?expires=1776713400&signature=ead9498616cf20248fc89a080949aa7f3a286f050a4b2f9c12974b2fa688d891&req=dScvEsh8n4BeUfMW1HO4zV2q5aEtwAVRCh7KnmDb6ZV7934inz%2FHEDMCPewY%0ALZW2%0A)

**Step 2**

Once you've identified the missing cost basis you'd like to ignore, click **Ignore this warning.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1784123972/2dbfcbcc03701677ee9835da4d8c/Screenshot+2025-10-17+at+3_09_13%E2%80%AFPM.png?expires=1776713400&signature=aa72033a6eca8560a8ac2ac58e589aa2b286691e895a2d995cd2e74348e8f7f6&req=dScvEsh8nohYW%2FMW1HO4zeQ49yxF%2FHAa6ualpdtKtaDXCw3K0b%2FoKIJCFovd%0A8QdB%0A)

**Step 3**

Next, you'll be asked to confirm that you want to ignore this warning. Once you click **Confirm**, missing cost basis warnings for disposals of this asset will no longer appear for the tax year in which the transaction took place.

For example: by ignoring this missing cost basis warning for SOL, I will no longer see any warnings for disposals of SOL on my 2021 tax report. I may see warnings pop up for disposals of SOL in later tax years, however.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1784127085/37fafa0ad713760651de3300edd1/image.png?expires=1776713400&signature=f1503a2e5a4c5f38961d69f1e93f2a3462f7adb1e936fcc218dc3e3a1d5dc699&req=dScvEsh8moFXXPMW1HO4zdtsMLdSrBi07kudQOaSnG42bqTA7Mqk2BfvtE3z%0A0Thp%0A)

You can undo these changes by visiting the [Advanced Settings page](https://app.coinledger.io/individual/settings/advanced) and navigating to the **Hidden Missing Basis Warnings** section. To unignore a Missing Cost Basis Warning, simply click the three dots next to the warning and press **Restore**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1784142358/0720a873e4dd27d0dd41fe42f6f9/Screenshot+2025-10-17+at+3_19_40%E2%80%AFPM.png?expires=1776713400&signature=aa95a8865871d9d8d83eb38e1a29a0fe3442fb5322b2c724a1ba163a9281566a&req=dScvEsh6n4JaUfMW1HO4zfqOix1CNAJggQPyi9YT%2B3EzEHL8XkY%2FJBDCicky%0AMmh6%0A)

# Frequently Asked Questions

### FAQ's about Missing Cost Basis Warnings

**Can I Run My Tax Report With a Missing Cost Basis?**

Yes. CoinLedger will still run your tax report in spite of Missing Cost Basis Warnings. In many circumstances, Missing Cost Basis Warnings _will not_ have any significant effect on your gains and losses. Our platform treats this missing data with a zero cost basis—the most conservative approach.

Learn how your Missing Cost Basis Warnings will affect your tax report in [this article here](https://help.cryptotrader.tax/en/articles/2865416-what-happens-if-i-run-my-report-with-a-negative-balance-warning).

**I’ve uploaded all of my information, why do I still have a missing cost basis warning?**

If you’ve uploaded all your information for all years of trading, but still have a missing cost basis, it is possible you have duplicate transactions imported from one of your crypto exchanges. It is also possible that your crypto exchange does not import all of their complete transaction data, and you’ll need to get in touch with our Support Team to identify and get around these limitations. Also, remember to check the total impact of each warning on the [Missing Cost Basis Troubleshooting page](https://app.coinledger.io/individual/missing-basis-troubleshooting). Here you can see the potential report impact of each of your warnings. If your warning has an insignificant (or even $0) impact on your potential gains and losses, it can safely be ignored. The IRS allows this.

**I have data for the missing cost basis, how do I add it?**

The easiest way to import this data is to upload a transaction history CSV file or connect an API key from an exchange we support. If you have a cost basis for one of your flagged transactions that you would like to add manually, you can add this to our software using our [Universal Manual Import Template.](https://help.cryptotrader.tax/en/articles/6028758-universal-manual-import-template-guide) Be sure to include the date, timestamp, price, and the assets you traded/received in this transaction.

Alternatively, you can manually add a cost basis for an asset by entering a Manual Position into CoinLedger on the Transactions page. You can find details on this process [HERE](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it#h_2ff6517137).

**I have duplicate transactions, does this matter? How do I get rid of them?**

Yes! While CoinLedger automatically detects and filters out most duplicate transactions, some may slip through the cracks depending on the method you are using to import transactions. This can be problematic, since duplicate transactions may lead to missing cost basis warnings and other inaccuracies with your tax report and portfolio tracking calculations. Please see [this guide](https://help.coinledger.io/en/articles/10416095-what-should-i-do-if-i-have-duplicate-transactions-on-my-account) to learn why duplicate transactions occur and how you can remove them from your account.

**How can I edit the cost basis of a transaction?**

Currently, it is not possible to directly edit the cost basis of a transaction. Editing a transaction or changing its historical price (which is **_not related_** to cost basis) will not alter your cost basis and is not recommended.

Instead, to update your cost basis, we recommend either importing your entire crypto transaction history or manually entering your cost basis using CoinLedger’s [Manual Position](https://help.coinledger.io/en/articles/10080173-can-i-manually-enter-an-asset-s-cost-basis-aka-a-manual-position) feature.

Still stuck? Think there is a different problem? Reach out to our [Support Team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) at any time!

Did this answer your question?

😞😐😃