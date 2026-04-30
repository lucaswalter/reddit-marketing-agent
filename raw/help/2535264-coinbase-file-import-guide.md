[Skip to main content](https://help.coinledger.io/en/articles/2535264-coinbase-file-import-guide#main-content)

# Coinbase - File Import Guide

How to import your trading history from Coinbase into CoinLedger

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 7 months ago

There are two options for importing your Coinbase trade history. You can upload your history via **CSV** files or import via a read-only access API. The CSV import process is laid out below.

**NOTE:** If you trade on Coinbase Advanced, we recommend switching to the API import method [detailed here](https://help.coinledger.io/en/articles/2986974-coinbase-api-import-guide).

Coinbase CSV Import Demo - 2025

**Step 1:**

​ [Login To Your Coinbase Account](https://www.coinbase.com/signin)

**Step 2:**

Click on the grid icon next to your profile button in the top right corner and then select **Accounts.**

![](https://downloads.intercomcdn.com/i/o/1064804192/36e90ca582ed3b236203e64c/Screenshot+2024-05-28+at+5_19_03%E2%80%AFPM.png?expires=1776713400&signature=3a5fb284113e0c895b87ec7e215ed3585694c0e132ffe6219db91da99083d80e&req=dSAhEsF%2BmYBWW%2FMW1HO4zXQaA5OIeUWFVuVmD%2BYNn%2BINkOV4qNr5QMDqoGSD%0Adcm60htoiuUBf1ZpooI%3D%0A)

![](https://downloads.intercomcdn.com/i/o/1064804284/4fcf6c1ca1abcdb8d895419f/Screenshot+2024-05-28+at+5_20_34%E2%80%AFPM.png?expires=1776713400&signature=aeebb3e78770fb3179cd406363b36d8adaf3dcea0c42723b93b69596e73a5e67&req=dSAhEsF%2BmYNXXfMW1HO4zTtJ5Veki4Hz1rem9ssl4PmHc1S9lyBCq0YKCyxS%0A4d%2FuIO6Uu9JSABPKqm4%3D%0A)

Be sure that you're viewing the regular Coinbase UI and **not** the Coinbase Advanced UI, as shown above.

You can also navigate directly to [https://accounts.coinbase.com/](https://accounts.coinbase.com/).

**Step 3:**

Next, select **Statements**. It's very important to select Statements and _NOT TAXES_ at this stage.

![](https://downloads.intercomcdn.com/i/o/1064808009/7526141aba737be3ea623576/Screenshot+2024-05-28+at+5_26_50%E2%80%AFPM.png?expires=1776713400&signature=cf9256084eb5005cc1e711551de2fe22e0610598d19ad9bc0a3d9db9fb361a8f&req=dSAhEsF%2BlYFfUPMW1HO4zXxTgoeOwCldQ7%2BR4nI7CIu04%2BE1ki6TIWqh%2FjxX%0Anjf1j0ijAmrR2l%2B9kJM%3D%0A)

Then, select **Transactions**. Please _do not_ select the Futures or Other tabs.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1360176501/f86dcc934a9f241bdc9502649f25/Screenshot+2025-01-31+at+2_28_35%E2%80%AFPM.png?expires=1776713400&signature=bbed1fb15982af29355ab43bcac28aadee08131ca09fbdd3ab87cf7ec315650b&req=dSMhFsh5m4RfWPMW1HO4zUGuBG4ZshJqh7RoIIvl%2FHMs6%2BW%2FNwfHG1GJfpkJ%0AGGavVljhmEJUB5eHqV8%3D%0A)

**Step 4:**

On the right side of your screen under Generate custom statement, create a **CSV** file according to these specifications:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1360170855/2e03bc987e953e4c40918bd6f83e/Screenshot+2025-01-31+at+2_23_45%E2%80%AFPM.png?expires=1776713400&signature=89791733fb22cc5a7587cb4f9a1b23d31b5b67dcd9c5c873775864c9cc16640c&req=dSMhFsh5nYlaXPMW1HO4zWg4muDQavgGtLfR%2BDjvsPoc5iyGDxyLapup8b%2F3%0AbrA2ia0DYDTsFZyxo2w%3D%0A)

It's important to ensure that **All assets** and **All transactions** are selected, and that the date range is set to **Custom.** Set your custom Start Date to as far back in your trading history as you can go. Our system needs all of your transaction history on Coinbase, for all years of trading, to ensure that your portfolio and tax report calculations are done correctly.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1360169731/fe729a5af40481f6e6d98b5d54d2/image.png?expires=1776713400&signature=df85261a34bd9d4b209eb6d075244901948127d7e834d6005f933d1a7b5d62d6&req=dSMhFsh4lIZcWPMW1HO4zR0Jtr65SskTLz6FySxGDDDNtVz6VAueeF8bciTS%0Agd3jmRFqyb%2Bcs57AgoY%3D%0A)

Finally, select **CSV**, and then click **Download**.

**Step 5:**

You will receive a file in **CSV** format. From our software, navigate to **1\. Import**. Select **Add Account** then choose the **Coinbase** tab on CoinLedger. Click on **Upload File** and drag your **CSV** file into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1360174458/d0161ca88439611219021d836b40/image.png?expires=1776713400&signature=e74331f888b48b3a45ec563e3c26725a3f98779fc98845d6ba002f0c68ccad8e&req=dSMhFsh5mYVaUfMW1HO4zTD%2BQyRxFuBLDzmO0KyOAHJr6%2B%2BCfkQLOCWWChRm%0A4vGha%2F0hugHDR2p0pxk%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

**Note:** Coinbase and Coinbase Pro, which has now transitioned to being Coinbase Advanced, were treated as two separate exchanges prior to 2024. If you used both, you need to import your history from each exchange. Here is the guide for [importing Coinbase Pro](https://help.cryptotrader.tax/en/articles/2535269-coinbase-pro-guide).

​

Did this answer your question?

😞😐😃