[Skip to main content](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab#main-content)

# What is the Potential Bridges, Trades and Transfers tab?

CoinLedger will identify any potential bridge, transfer or trade transactions that were not automatically mapped upon import

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 3 months ago

In most cases, CoinLedger will automatically detect bridges, transfers and trades without any manual classification being required. However, some blockchains or exchanges send CoinLedger incomplete transaction history data, which will cause these transactions to get imported as two separate transactions (a deposit and withdrawal). While this is not the fault of CoinLedger, our software does offer a solution to these problems!

Potential Trades, Transfers and Bridges Walkthrough

CoinLedger will identify any potential bridge, transfer or trade transactions that were not automatically mapped upon import on the **[Transactions page](https://app.coinledger.io/individual/transactions)**. If our system flags any of these potential bridges, transfers or trades on your account, they will be shown here under the **Potential Bridges, Trades and Transfers** tab. Using this tab, you can review each of the transactions CoinLedger has flagged and easily merge them together to resolve any Missing Cost Basis warnings on your account.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1411652813/2f79cdb55e62b6b6fa6f6ac1ac97/image.png?expires=1776713400&signature=80d24c13709bcc7bedaeb0a0efbdeaab107986e56f7034ac5c45caf29fb8e23c&req=dSQmF897n4leWvMW1HO4zTNuj6ZyfsOblg3eamzGRwTqC8c%2BmCnJoy1S4RGq%0AInnp6ROkT41W5P3D%2BZY%3D%0A)

CoinLedger will flag each potential bridge, trade or transfer transaction in pairs, and will suggest the most likely classification that these two transactions should be merged into.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1411642652/5f136216e6a7ff38d5ae0b4ff0b5/AD_4nXcNEtz3j91-RYUV4hroUKl1qo3mH80OPy8nJY0PD0hWnlr44CQtdX7YyGYOCSQHOZ3zw5MxbCp_9xwaDH85q9HUKAAXYJMjxmCkhme9Z7EWjwKy3uh7q-MhK6m4uRrYW1bLFXDioQ?expires=1776713400&signature=19679997ea75f67ce107b7e190c8f914275b2c7f4de201055c0e7bc240208696&req=dSQmF896n4daW%2FMW1HO4zeqrYpFqoEwBGMdxDUSn%2FcyLbMxOYZYd46%2BFCkBC%0Aat%2Fmf4dHEETwu3%2FiJb4%3D%0A)

To accept all of these suggestions in bulk and merge each of these transactions together, check the box on the Potential Bridges, Trades and Transfers tab (as shown below) and then select **Save All** on the pop-up menu at the bottom of your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1613642622/99a537f086e8c686cf0b670b21ca/Screenshot+2025-07-10+at+1_22_14%E2%80%AFPM.png?expires=1776713400&signature=1328df23653e7989a49a8feb82e9431557b828461959965a03bfee3c334cd33e&req=dSYmFc96n4ddW%2FMW1HO4zY8swwpFPOpxT6nCWZvmTAZZH4RtsnMjmk8OMfcY%0AcqpmJzJ9Bl1rWA8CYbU%3D%0A)

Each of your selected transaction pairs will now be merged together using the transaction type CoinLedger suggested.

You can also merge individual suggestions together by checking the box next to each potential transaction match you want to accept, and selecting **Confirm All** from the pop-up menu at the bottom of your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1613641010/b9885d6d2f39fb89d03dacdd1cf2/Screenshot%2B2025-03-07%2Bat%2B11_06_28-E2-80-AFAM.png?expires=1776713400&signature=2d49b09359f273d31141b7e52ba73dc4ab81f94ce5be92ad77881d61aa820f46&req=dSYmFc96nIFeWfMW1HO4zTX0yGa2kr%2BDDwA6xOKSAqRdwCxpO1tB%2B752x11Q%0AX54aZVTyEpBRKDMed7Y%3D%0A)

To confirm these changes, press **Save All**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1613641009/90ae66598f6168842ec71186ec3c/image.png?expires=1776713400&signature=49675e9642ddda2ece33d37105870b9cc1aad0b238f5a462ab6bf092fdde7435&req=dSYmFc96nIFfUPMW1HO4zfin8voR7WfMcYZpnIrqiiT8ttqwO%2F2WlJW%2F0ybC%0A7MDdPU552qVw%2BnW3SiY%3D%0A)

**Alternative step - "Create Transfer" feature**

If you have a loose/naked withdrawal or deposit that you cannot match to its corresponding pair, CoinLedger allows you to quickly resolve this with an action button called "Create Transfer". See how this works below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1994841214/61bfaf491db5716160e7df54a2e5/image.png?expires=1776713400&signature=4993830bb5944fcea37672f4188e8a2bd7c1818ec891a35c8b28ee782e91e9e1&req=dSkuEsF6nINeXfMW1HO4zT1MRvgqHtboZtk%2FmlXU0NvS4al%2BPzMKFkbYzKAA%0Awyely1KjQl8KdysFoEs%3D%0A)

Next, simply select a source account, and CoinLedger will automatically convert this into a Transfer transaction while preserving the original transaction details (timestamp, amounts). In the example above, since the original transaction is a Deposit, CoinLedger will create the corresponding Withdrawal to complete the transfer. The same process works in reverse—if the original transaction is a Withdrawal, CoinLedger will generate the matching Deposit.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1994842868/9bd38d4fd031cbaa17ad4df52eed/image.png?expires=1776713400&signature=eae3697f51b7be5e0f4100cd5753cd3ee3c3b06e22bdc8d19de4af631ec7469a&req=dSkuEsF6n4lZUfMW1HO4zQeRSSKN08aZE%2FWlt1yPuH%2B08G%2BY8S76vnrKrdnL%0AFZvLFiV%2FJvygm3vY%2FLE%3D%0A)

Here's how the final transaction looks on CoinLedger's UI:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1994842864/710c7398938c989ced1d7ab72b30/image.png?expires=1776713400&signature=177bf2ca3dbeded5f9919098acc9551044aa8e6fc3725fd94085f9b9fe4ddf6d&req=dSkuEsF6n4lZXfMW1HO4zasBy5sL%2B6IYnrbtWBgU9hKLZuBGiTRfvMnecw2C%0AObj3FFNlUmQ4ITA56%2Bg%3D%0A)

This option is particularly useful when you're missing one side of a transaction and need a quick solution instead of importing complete data. It's most helpful when you're only missing a few transactions. For larger gaps, consider importing a CSV file or using an API when available.

# Frequently Asked Questions

Please review each of the drop-down sections below for the common questions we see about this feature.

## What if I want to change the transaction type before merging the transactions together?

If you don’t accept CoinLedger’s suggestion for a specific transaction and would like to change the transaction type before merging the transactions together, you can do so by checking the box next to it, and clicking **Reclassify** on the pop-up menu at the bottom of your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531389723/e7e02e87791e18c36655ea61a697/image.png?expires=1776713400&signature=f6cad61a071552f428dbc3295e54f16ff4acb90b4112b97d9ca5c4bfd43379d9&req=dSUkF8p2lIZdWvMW1HO4zeOjjymxU0f%2F2pq5r9%2FTDR7Mi0vWhdUPK1GFUfue%0ADYWE%0A)

For example: CoinLedger may suggest a potential bridge to be merged together on your account, but you may want to merge that transaction into a trade instead. You can do this by hitting **Reclassify** and then selecting Trade.

## How can I ignore a suggestion on the Potential Bridges, Trades and Transfers tab?

You can ignore a suggestion by clicking the three dots next to the potential match and selecting **Ignore**. This will remove the suggestion from the Transactions page. However, the two transactions from this potential match will still be present in your account.

​

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531388920/17444c4950807d86e97fe3a3dc7c/image.png?expires=1776713400&signature=49fdb1db5b87bcb7708b56da869d3438d8da516e8139bba4229253fa0d2ed91a&req=dSUkF8p2lYhdWfMW1HO4zdU4kYNaTkG2INqEosdyApcRCx4d8ZCa8Wy5900D%0Awirm%0A)

## Why is my merge failing?

If your attempted merge fails, CoinLedger will show an error message explaining why the merge failed and how to fix it. In the example below, you can see that two of my potential transfers failed to be merged together. A pop-up menu then showed up on my screen explaining why this occurred.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531382430/8cd219935f1e4a3399bfcd9b663a/image.png?expires=1776713400&signature=b99a4ad2688a34732b6b21789805816379990c9e3c43595fc75043185a3a3c66&req=dSUkF8p2n4VcWfMW1HO4zZWJSkEkMN1NHgm3HMO8uem2XMRdJmHBwh0rgWPT%0ANJj5%0A)

In both of the Transfers shown above, my transactions failed to be merged together because the withdrawal and deposit transactions contain two different assets. In order for a transaction to be a transfer, _the same asset_ has to be sent from one wallet to another, so the transfer classification is not appropriate here. For these transactions, I could merge them into a [different transaction type](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab#h_25b12680c5) like Trade or Bridge instead.

CoinLedger may also prompt you to edit one or both of the transactions before merging them together. Usually, this is because the amounts sent and received in each transaction do not match. This is necessary for a merge of two transactions to be successfully completed.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1613759149/afa3bd1430479b25fa9fe48cc6ff/image.png?expires=1776713400&signature=66f0404b3c88ac5ebbda7223a00b321ab1880839c39bfb24ce51afeb36249e40&req=dSYmFc57lIBbUPMW1HO4zWlTaJKj1dCwuPatramz7zp28Y8OMdklNPIIk6uc%0ASTRj%0A)

You can fix this by selecting the 3 dots next to the transaction, hitting **Edit transaction**, and changing the Amount Sent or Received to match the amount shown in the other transaction.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531382423/de3821b8b7aba86d421564dc0a22/Screenshot%2B2025-05-01%2Bat%2B7_04_53-E2-80-AFPM.png?expires=1776713400&signature=f6f73239a675c73150755b73e3185c8f6a4bda3b5713ce741f5d7b4f9e6a8622&req=dSUkF8p2n4VdWvMW1HO4zUa9v6S%2FOALTzAG9m1EZQ6n5AJWb46wvtfwQ%2FZUy%0AIRG4%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531382420/3d4421d854d4e3905c24bfb511ca/Screenshot%2B2025-05-01%2Bat%2B7_01_46-E2-80-AFPM.png?expires=1776713400&signature=d3032903fb4de5e9a87dcff2f86484a922b5868f7d8ba7bd551d8595a8cce431&req=dSUkF8p2n4VdWfMW1HO4zVzGzjX4%2FNQC7ekY%2F4OZiz9xJUeIoZTewNUlw3Wu%0AfLev%0A)

Once you have finished editing the transaction, press **Save** to ensure your changes go into effect. Then, you can retry the process of merging the two transactions together.

## I'm not seeing a trade, transfer or bridge suggested on this tab that I think should be here. What can I do?

If a potential bridge, transfer or trade is not being suggested on this tab but you think it should be, we first recommend searching for this transaction on your account using the [filters](https://help.coinledger.io/en/articles/5964817-how-can-i-filter-my-transactions-by-asset-date-or-transaction-type) on the Transactions page. Most transactions will be correctly classified by CoinLedger during your first import, which means it is likely that this transaction already exists in your account.

If you have verified that this transaction has not been imported, though, you can manually merge a deposit and withdrawal together into a bridge, transfer or trade. Here's how:

**Step 1**

First, head to the **Transactions** step of the CoinLedger app. Then, locate the withdrawal and deposit transactions in question.

**Step 2**

Mark the two transactions as shown below, and then select **Merge.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1531382992/d20da675665898fc960491e9c0da/Screenshot-2B2023-09-07-2Bat-2B12_10_37-2BPM.png?expires=1776713400&signature=7fbdac94eaf733b006cad635caa481dc1920753569f20d09c556a23f07393795&req=dSUkF8p2n4hWW%2FMW1HO4zVR7J9K%2BPlPHq9Vod6zRfo6QuCPe%2B4jU6bP5ND%2FI%0AusIo%0A)

Select the transaction type you would like to merge them into,and then press **Done** to confirm the change **.**

​

Did this answer your question?

😞😐😃