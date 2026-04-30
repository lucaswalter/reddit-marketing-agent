[Skip to main content](https://help.coinledger.io/en/articles/10416095-what-should-i-do-if-i-have-duplicate-transactions-on-my-account#main-content)

# What should I do if I have duplicate transactions on my account?

Learn the common causes for duplicate transactions and how to resolve them

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 11 months ago

While CoinLedger automatically detects and filters out most duplicate transactions before they can be imported, some may slip through the cracks depending on the method you are using to import transactions into your account. This can be problematic, since duplicate transactions may lead to missing cost basis warnings and other inaccuracies with your tax report and portfolio tracking calculations. Read below to learn the scenarios where duplicate transactions might occur and how you can remove them from your account!

# How can I tell if there are duplicate transactions or imports on my account?

### Transactions with the same timestamp, assets and amounts

A telltale sign that you have duplicate transactions on your account is the presence of transactions which share the same exact timestamp, assets and amounts. For example, as shown below I can see two sets of transactions on Coinbase which are duplicated. The assets, amounts and even the timestamp for each set of transactions are the same.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338933240/7bb58da40af85ea7e66cb8dc2024/AD_4nXcVx14kKADIYkA1kSnMK4a6wBqivH3De3NkXFQKliKiIGolPo8wlCHuYEJVWvrd8VwYiN-KSc0J707p1Wy2h360F03xTTAZmzmePCCRkTXe4XbqG00YwLzlHwsgBF4_Hk9vjK-H?expires=1776713400&signature=94413de093eb9d8267401860cce981780c9426f8d6794e7e8b1f0e42bef4d0f1&req=dSMkHsB9noNbWfMW1HO4zf%2ByY1l3xEM6H8AEghZRilWaw0oVKVszS6jxy9sk%0A%2FsaZtK8SJkyZZZrMaso%3D%0A)

### The Missing Cost Basis Troubleshooting Tab

Another way to spot duplicate transactions on your account is to look at the [Missing Cost Basis Troubleshooting tab](https://app.coinledger.io/individual/missing-basis-troubleshooting) on your account. The Missing Cost Basis Troubleshooting Tab is a dynamic summary of all missing data on your account with specific suggestions on how to resolve your missing basis warnings. It appears anytime you have a MCB warning on your account, and can be accessed from the Transactions stage of the CoinLedger app.

If you have duplicate wallet or file imports anywhere on your account, those will be flagged as a potential cause of your missing cost basis warnings on the Troubleshooting Tab. See the example below:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338933248/e6bbe8bb3380255845aa1cb3931c/AD_4nXfA_v9FF7UcwNY6-l1Qx8aecjzMUk0G6Fe08nJ5xQzbbFwZk-TfoGBs8qymXhbzXJHyuczXWDQxZdpE2dQov1HBZBaLHqV6unpYKX85TnNYSNyFJhu3nyDJh-rufebRaT7xIZjI?expires=1776713400&signature=e8a5c4a62b8c4bb1fafaa100b7b5a80febf5f6c17165f38ff18bc90a9e0c83ce&req=dSMkHsB9noNbUfMW1HO4zXggCYJ0J7mvPN02c4L8sQ3v1cWeNbsu1HwNEevH%0ABKBV%2F6Fv4Be6EK88M2s%3D%0A)

In this example, CoinLedger is warning me that I have a duplicate ETH address imported in my account - and it's also warning me that I imported the same CSV file from Coinbase twice. To open the source of the duplicate data and remove the problematic imports, I would click directly on the underlined account within the warning card, as shown below. There, I can manage or delete my duplicate imports.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338933239/ae87964dcf2f527c9b8490a25243/AD_4nXePUo6PdO0f4VAS6sNqm-obmdl5yn690iS08F7OSeNoqEGEbMo-aEjMDPsIJYlt6uPerLrsE5DRitu04__OhqCbkJU15pteLT5QGh-FAK8EY0EO3VDp9274GlHHr5q1dNfrgAwopw?expires=1776713400&signature=3a8ef86d7eee06318fb9f3b419ce7598ec98f516de9a587dacee9f791a6306b4&req=dSMkHsB9noNcUPMW1HO4zWEyZfzh8glFp5aHqGB8T09exrMxOU9U17IT%2B7z%2B%0A41HyKvUYwDACeCU7zTQ%3D%0A)

# Common Causes of Duplicate Transactions

Below are some common causes of duplicate transactions and instructions on how to resolve them.

## Duplicate Wallet Addresses

Importing the same wallet address multiple times can cause duplicate transactions. To resolve this, first identify the wallet address that was imported multiple times. You can do this by using the [Missing Cost Basis Troubleshooting tab](https://app.coinledger.io/individual/missing-basis-troubleshooting) on your account.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1338933244/b2727c6dfec20042028ec3c56b5d/AD_4nXfA_v9FF7UcwNY6-l1Qx8aecjzMUk0G6Fe08nJ5xQzbbFwZk-TfoGBs8qymXhbzXJHyuczXWDQxZdpE2dQov1HBZBaLHqV6unpYKX85TnNYSNyFJhu3nyDJh-rufebRaT7xIZjI?expires=1776713400&signature=3b52523aede618e43fbd13c2a939c111c8c2d7356220bd90d81138e1ec62333e&req=dSMkHsB9noNbXfMW1HO4zd7qccDNmX%2Bsq91fXPd9Kpa1oSIP1YzS2cb3kvSH%0Ac%2B1Hefjx%2BfpRnZlnCV0%3D%0A)

If an address has been imported multiple times, you’ll need to keep one of the imports and delete the rest.

### You can delete any unwanted wallet address from your imports by following this process:

**Step 1**

First, head to the account containing the address(es) you'd like to delete. You can jump there directly from one of the warning cards shown on the Missing Cost Basis Troubleshooting Tab.

Then, press the drop-down carrot icon next to the icon which states how many wallet addresses you have connected for that account (the number will vary across each account, but it will say XXX NUMBER of addresses connected). After that, press **Delete**.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534074818/7fad5a6c84b73cd5633d6fcda54a/Screenshot%2B2025-04-23%2Bat%2B1_18_42-E2-80-AFPM.png?expires=1776713400&signature=58ddb4d6ae1d0a32cf3ea0bad5fc6582ace0a88efec0d5272c42ccf37b9f5759&req=dSUkEsl5mYleUfMW1HO4zYuVj%2F%2B5LOt%2F%2BRSKwJJsA4yUG69XNEdC4ymheweH%0ANSO6%0A)

**Step 2**

Here, you'll see a list of all the imported addresses for this account. If you see any wallet addresses listed multiple times on this pop-up menu, this is likely the source of your duplicate transactions. Choose one one of the addresses to keep, and then delete the other. Check the box next to the address(es) you'd like to delete, and then press the **Delete** button to fully delete that address.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534074824/317c975ed12c66829918ffa3f07d/Screenshot%2B2025-04-23%2Bat%2B1_21_34-E2-80-AFPM.png?expires=1776713400&signature=53331af4982dddbe1923d48ae0cc58d3a1258feb9b1c390fae44151ddfe25ee5&req=dSUkEsl5mYldXfMW1HO4zesdd2rVp8yOtQ%2FF%2Bxws4jYjCTlqNpsOyfVldcn6%0A6eSt%0A)

**Step 3**

If you clicked on the **Delete** button in Step 1 but don’t see any duplicate wallet addresses on your list of imports, it’s possible that you imported the same wallet address into _two separate accounts_ in CoinLedger.

For example, according to the MCB Troubleshooting Tab in my account, I imported the same ETH address in my Ethereum #2 and Ethereum #6 accounts.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534074817/f50458efeff38fd5a74e0c065f71/AD_4nXcv_mSyi9EVCxeF9GFHgEetShg5sgk5xWjOiiILUQdq2D_Ap_UYK1SnE47EaV6ZU9rFbItrsPJ1NPXtvYjgSRt0dGp1aC4Zml6df3LGFEqmlAjbBgWWI6TZsB7pMxFBn3ELNOSm?expires=1776713400&signature=be3653bc44312d4ff72c78e90439647885b9d4061500f4b7f09907ae02d48c5d&req=dSUkEsl5mYleXvMW1HO4zSGbLxJ100ptuqp7iK891viMrQlaKjgxiqBmvdvJ%0AHNEc%0A)

To resolve this, I would simply delete one of these accounts while keeping the other, as shown below:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534074821/bacbffac38ed112c7caf59203749/AD_4nXfkHBARY2whmqdBigCn4sGF1quDSUq-_mtkK9iWKwijysHEvphk0FvbNDnNCZg2Qc9YQjhPOqDLiuWyH9wiCzBHwsYXXeokPQmAWFZ3zyHczBbDr3iA27BmPluknWDA615K7XoxhQ?expires=1776713400&signature=bfe847680ecd6590717936632526d60be3f964f8425b88fc382fd7f4b19db4c1&req=dSUkEsl5mYldWPMW1HO4zSdH8VEyK%2Byrw38QLFUdIawf%2BJURGYTjP1Tb2xzn%0AVjwe%0A)

## Combining a File Import and API Import For the Same Exchange

Another cause of duplicate imports is combining a file import and API import for the same exchange. For example, if I imported my Coinbase transactions via CSV and API, there’s a high likelihood that duplicate transactions will be imported. This is because, while our system is able to filter out duplicates when importing via just CSV file or just API, it is not built to detect duplicates when combining the two.

### To resolve this, follow these steps:

**Step 1**

Locate the exchange where duplicate transactions have been imported.

**Step 2**

Click the clock icon in the top right corner to open up the Import History modal.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534078460/eadcce90cb1e80f94075480b9c81/AD_4nXeVFcloivCIrk3nbhtgq11YGUc6wXTvTRzioDrwq-qAW5bIhc4RkFxLhggQOj4o8XGK8pQfy6ds6t4bkAiqiFVYMLRQ9Zr7pnmhZGInuHxZ5nRf-hIeOYHt5-LWlKjyB1KIM8Et?expires=1776713400&signature=2910aa51241a0eadb5b7b6d5d379e77738910c79a805c41c42c08f981accc888&req=dSUkEsl5lYVZWfMW1HO4zQy3qHO95vX%2FM8q%2FQMoquyFHIrK0OqjCQsNIPwG%2F%0AAHSM%0A)

**Step 3**

On this menu you’ll see all of the imports you’ve made for this exchange. We recommend deleting either the file import or the API import and then keeping the other. You can delete an import by clicking **Delete Transactions** and then confirming the action by clicking **Delete Transactions** one more time.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534078464/c479a66a58e654a96a7196f32ee3/Screenshot%2B2025-01-21%2Bat%2B11_50_55-E2-80-AFAM.png?expires=1776713400&signature=1b06305ba9ebf2bb4feed477fe09eafb1abd60b3a83b9edaf529134be39fd5a5&req=dSUkEsl5lYVZXfMW1HO4zQBXoDzZQlv0jtcfNf1hPF3npTpSOj3u%2BiA10sEG%0Ajcu7%0A)

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1534078459/11a8b2344e4d1ba92ad9d85a42df/Screenshot%2B2025-01-21%2Bat%2B11_51_29-E2-80-AFAM.png?expires=1776713400&signature=8940073728825bf5e81dcaec6d8166397ae2aebaa2cc8f35605843b2f7941c7a&req=dSUkEsl5lYVaUPMW1HO4zRoPsYuuIMh7Q2NB1%2FxB2pZqGEi%2Fb9ExOyYCHvnI%0AAP%2B5%0A)

​

Have any questions? Our [support team](https://help.coinledger.io/en/articles/9251645-how-to-contact-coinledger-support) would be happy to help :)

Did this answer your question?

😞😐😃