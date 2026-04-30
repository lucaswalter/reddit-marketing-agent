[Skip to main content](https://help.coinledger.io/en/articles/10574174-simpleswap-file-import-guide#main-content)

# SimpleSwap - File Import Guide

How to import your trading history from SimpleSwap into CoinLedger

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 5 months ago

**Step 1**

Login to your [SimpleSwap account](https://simpleswap.io/).

**Step 2**

Click on the **My Account** drop down in the top right corner and then select **History.** This will bring you to a page detailing your transaction history.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1384626682/135f16bb29dda370c6b8139adab9/Screenshot+2025-02-17+at+5_42_31%E2%80%AFPM.png?expires=1776713400&signature=fc83cf02216d591f48c9a22451dc324ebc3b4d9ea1e657c4d7ce1e0af8fc8690&req=dSMvEs98m4dXW%2FMW1HO4zWRxJpwNE8DEmrdvxT2DteVN5AWVNnG10c4%2F540T%0AEeSDIbqAFcK5vKJVpSA%3D%0A)

**Step 3**

Next, select the **History** tab.

**Step 4**

After that, set the time range for your transactions to **All**, as shown below. Do not select any specific From or To currencies at this stage, as CoinLedger needs all of your transactions for all assets/currencies in order to accurately calculate your gains and losses.

Then, press **Export** next to Exchange History.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1384627410/ce77f037c2c01b6f8f488b741116/Screenshot+2025-02-17+at+5_40_10%E2%80%AFPM.png?expires=1776713400&signature=7d949c41dc8f2b2bcf1c5707bdf40e31a09b074b91fe181b70fa3cae0111fe5b&req=dSMvEs98moVeWfMW1HO4zTicNbEDQFA%2B5QPkDhlhO7b0jbVcRkKJ6xcrU3HB%0Ac9YXfA7P0C1AOjeSOq0%3D%0A)

**Step 5:**

You will receive a file in **CSV** format. From our software, navigate to **1\. Import**. Select **Add Account** then choose the **SimpleSwap** tab on CoinLedger. Click on **Upload File** and drag your **CSV** file into the box to import your transactions.

​

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1384628133/d9de98b89fb15520d75f9ae21c0a/image.png?expires=1776713400&signature=6c34834e65a86594913465b74cdaa7e0923101e6813e2e9409eda0f6c7994244&req=dSMvEs98lYBcWvMW1HO4zU5TuGPXpE%2FMhGNLIETCq%2FAcGPf1ns57j2oZQgnX%0ATL7xeHBnMDsRNX1LuG0%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1384628448/4c17c1612a5de530ab11d3228d81/Screenshot%2B2024-08-02%2Bat%2B1_25_10-E2-80-AFPM.png?expires=1776713400&signature=9a1647dd37fe3b064ef6f98bb4b3f3b0c933aef557885191e4b0efcdddf819bb&req=dSMvEs98lYVbUfMW1HO4zbXQWkXfxYxbUen%2Fviz2rwzcyCerq21GBmbk1C6Y%0AtE5DFLXlwwc64kQavw8%3D%0A)

## Simple Swap Limitations

SimpleSwap exports timestamps in UTC, which may differ from your local timezone and the actual blockchain transaction time. This time difference could affect automatic transfer matching if you're also importing wallet history. Review your Transfers section after import to ensure transactions are properly consolidated.

​

Did this answer your question?

😞😐😃