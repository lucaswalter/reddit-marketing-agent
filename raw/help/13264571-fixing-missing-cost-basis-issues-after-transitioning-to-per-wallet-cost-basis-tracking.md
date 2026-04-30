[Skip to main content](https://help.coinledger.io/en/articles/13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking#main-content)

# Fixing Missing Cost Basis Issues After Transitioning to Per-Wallet Cost Basis Tracking

Fix Missing Cost Basis Warnings, inaccurate capital gains, or other data issues from the switch to per wallet cost basis tracking

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 4 months ago

If you are seeing Missing Cost Basis Warnings, inaccurate capital gains or other data issues on your account after transitioning to [per-wallet cost basis tracking](https://help.coinledger.io/en/articles/10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28), it’s likely that one of your **Transfer transactions** is missing. This guide details how to fix this issue.

## Why Transfers Are So Important

[The IRS’s new per-wallet regulations](https://help.coinledger.io/en/articles/10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28) require you to import all of your transactions, including deposits and withdrawals, into CoinLedger. These deposits and withdrawals should be marked as Transfers to ensure that your cost basis carries over correctly between wallets.

If you transferred crypto from one wallet or exchange to another, you should double check that CoinLedger imported this transaction as a **Transfer**. Most of the time our system will, but occasionally you’ll need to manually change your deposits and withdrawals into Transfers.

This is crucial to ensuring that your tax report is accurate, since standalone withdrawal and deposit transactions are considered non-taxable self-transfers that _do not carry any cost basis_ balance.

As a first step, we recommend filtering for Transfers on the [Transactions page](https://app.coinledger.io/individual/transactions) of your account. You should review each Transfer transaction here and ensure that none are missing.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1909960946/892fc239d056abd9dc67131fc8bd/Screenshot+2025-12-31+at+11_24_41%E2%80%AFAM.png?expires=1776713400&signature=16678d89b35c6b0059b0783ab40f342cbd9d9a4f2b7262e7294dccec0f0a8779&req=dSknH8B4nYhbX%2FMW1HO4zc1ItsuIT0qVcZb5ASJid7JRoV9ULlgwE8pxjdZc%0ANKcREFMkSBp%2BnQVDY1U%3D%0A)

If you realize a Transfer is missing, you can troubleshoot this issue through the process below.

## Fixing a Missing Transfer

To fix a missing Transfer, you should start by merging together any Potential Bridges, Trades and Transfers that our system has flagged on the [Transactions page](https://app.coinledger.io/individual/transactions). To accept these suggestions and merge them together, check the box on the Potential Bridges, Trades and Transfers tab (as shown below) and then select **Save All** at the bottom of your screen.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1909961740/78b456f359578628e6b316ddac29/676c2148-8968-4ec1-981d-8783d7e7e9d5?expires=1776713400&signature=e5465d5faa931f6592e740eca65b9c2053f5601ba64f85d50890a9cdea8c48be&req=dSknH8B4nIZbWfMW1HO4zXrKXG1SVLlym7zCMfuIukC%2FdOc%2BbXow7daIibCV%0AGkcHWj8qxw0ftI5rHmA%3D%0A)

Most of the time, CoinLedger will detect any unmatched Potential Transfers on your account so you can merge them together through this process. However, if our system missed a Potential Transfer and did not suggest it on the Transactions page, you’ll need to merge these transactions yourself.

Head to the Transactions step of the CoinLedger app and locate the withdrawal and deposit transactions in question. Then, mark the transactions as shown below, and select **Merge**. Make sure you select **Transfer** as the transaction type.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1909961739/89d9fc3d486ed15bad15427358c6/2e465be1-e795-48ce-bc02-dd28c48a99c5?expires=1776713400&signature=d1320013e1b18f41099208729132ed81eb444c209604766a9f55aea7f4f7008b&req=dSknH8B4nIZcUPMW1HO4zSjVm4x%2F%2B6Npf3CCxRu0rDUEyaaJJnW5nCj1oxLw%0Ahp2dWNVD7bIfEk1dRY8%3D%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1909961741/b6f5193da335c4b4ea4272f801a2/18b9e72d-7283-4f33-b450-e9a633530ecc?expires=1776713400&signature=cadceaf8ae8f73bed3209f5bbc6ed2921712184bdb16655f15bb38a2e98e6226&req=dSknH8B4nIZbWPMW1HO4zWz2S5ixyBxMtq4Xby4BycmgstNYh6FE1GX9gCio%0AqfDY4JSj3NwVSHVkkgc%3D%0A)

**💡 NOTE:** CoinLedger may prompt you to edit one or both of the transactions before merging them together. Usually, this is because the amounts sent and received in each transaction do not match. You can fix this by editing one of the transactions and changing the amount of crypto sent or received to match exactly what is shown in the other transaction. Learn more about this process [here](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab#:~:text=Why%20is%20my%20merge%20failing%3F).

## What if my Transfers are present, but I'm still seeing issues with my data?

If all of your Transfer transactions are present but you are still seeing issues with your data, it's possible that a wallet or exchange you used in the past has not yet been imported. We recommend reviewing each of your imports to make sure that all of your wallets are accounted for.

Additionally, we recommend checking your account for Uncategorized Transactions. You can learn more about this process [here](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions).

Finally, it's possible that a Buy or Sell of crypto was imported as a nontaxable deposit or withdrawal transaction in your CoinLedger account. You can troubleshoot that issue through [this process](https://help.coinledger.io/en/articles/5915504-when-do-i-need-to-manually-classify-or-fix-my-crypto-transactions).

Still having questions about this issue? Feel free to [reach out to our Support Team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) anytime!

Did this answer your question?

😞😐😃