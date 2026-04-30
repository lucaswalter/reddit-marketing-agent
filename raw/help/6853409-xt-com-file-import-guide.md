[Skip to main content](https://help.coinledger.io/en/articles/6853409-xt-com-file-import-guide#main-content)

# XT.Com - File Import Guide

How to import your transaction history from XT.Com into CoinLedger

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

**Step 1:**

[Log into your XT.Com account](https://www.xt.com/en/accounts/login)

**Step 2:**

In the top right corner, click on the **Funds** button and then select **Spot (Deposit & Withdraw)** option from the dropdown list.

![](https://downloads.intercomcdn.com/i/o/641804708/10a4cf356387ef9c80ece920/image.png?expires=1776713400&signature=e548ffaf355473499d5ef63046c18ed9ce736bd87b2051a42cd76aa1aa7e5931&req=ciQmHsl6moFXFb4f3HP0gKh9OrvxQQkeP%2FFAV5NbQyaeLCD5sWkjf0YxT8AR%0As3SFdFjkk7p14ZMhlw%3D%3D%0A)

**Step 3:**

Click on the **Export icon** on the upper right side of the UI. This will open **Fund Records** screen.

![](https://downloads.intercomcdn.com/i/o/641805154/865f4b7372db02acd2a959db/image.png?expires=1776713400&signature=9545cf3a6a0dd4e35dbb635a45e2f29367b13be77c3ad172e02547921c4573dd&req=ciQmHsl7nIRbFb4f3HP0gBMZDfzqahMkUBwR78smA6Us9M9FBh3CElZgUpAR%0AgWaN3xa5eyGPXqeu0A%3D%3D%0A)

**Step 4:**

Select **Deposit** tab and then click on the **Export** button on the upper right side of the UI.

![](https://downloads.intercomcdn.com/i/o/641806179/36c9f075256460a9a2db47b7/image.png?expires=1776713400&signature=59e0cd305b8b303a59ad973d3fabdb82810b80bdbdb03e97323cc4b18ee6d504&req=ciQmHsl4nIZWFb4f3HP0gHMpHnpnZLIho9vKq4Z3XrOQVcG2F5%2Bw6cKnCOkX%0AmaUx%2Bodlh9NJSxQ0sg%3D%3D%0A)

**Step 5:**

Select the Date range for your transactions and then click on the **Export Now** button.

**Note:** It may take a while until XT.Com generates your history file for you.

![](https://downloads.intercomcdn.com/i/o/641806396/ed876379624dd9752c093d03/image.png?expires=1776713400&signature=769cb335ac0d9b88f57b0f793d5f0f5029ce260844807b6176d239bc0b8057d9&req=ciQmHsl4nohZFb4f3HP0gAOy4BiG99hjaQ%2FhJ8Z6mvxjvMax9eoU8t88bLjl%0AjobaPKRHCGK3X1Ssdw%3D%3D%0A)

**Step 6:**

Once the history file is ready, download it. The download file will have XLSX extension.

**Step 7:**

Repeat steps 4-6 for **Withdraw** and **Trade History** tabs on the Fund Records screen.

**Step 8:**

XT.Com will give you a zip file by default. Unzip that file so you have the **.csv** that is inside.

**Step 9:**

Open our software and navigate to **Step 1. Import**. Select _Add Account_ then choose the **XT.Com** tab. Click on _Upload File_ and drag your **XLSX** file into the box to import your transactions.

![](https://downloads.intercomcdn.com/i/o/641969368/a77d76ecee34460b668e9c0b/Screenshot+2022-12-27+at+16.01.59.png?expires=1776713400&signature=fbb3703880e090163e8bcb09bf21f531c50465c0889f207bead1cb20c4fa35a6&req=ciQmH893nodXFb4f3HP0gPNFilXvSIMqxHMPn1wfPw07Aq%2F9iNHRseL8GdzQ%0ABmyMQl3I%2BLUQOL20DQ%3D%3D%0A)

When importing a transaction history CSV, you will have the option to specify a start date for your import under the **Drag and Drop Files Here** box. This feature is designed to prevent duplicate data from being imported. You can access this feature by hitting the **Import Settings** drop down menu, as shown below, and then specifying a date for your import to start from. All transactions after this date will be imported. You should not do this if you are importing all of your transactions into CoinLedger for the first time.

![](https://downloads.intercomcdn.com/i/o/1135277331/96b03130391f69e1cfcfeda3/Screenshot+2024-08-02+at+1_25_10%E2%80%AFPM.png?expires=1776713400&signature=0738665e75bccda7739463c875a5df05ac33614af9b516939ba8199ca5393863&req=dSEkE8t5moJcWPMW1HO4zbqA%2BQ3JelhIVq0ry1MQHpxFbjDsb8H9OY1rgI%2Ft%0A0m4ANPKlp27QWCHaFiQ%3D%0A)

​ **Important Note:** XT.Com does not export a complete transaction file that includes all transaction types. Instead, XT.Com exports few different file types: **Withdrawals**, **Deposits**, and **Trades**. Each of these files contains completely separate transactions.

For this reason, it is very important to carefully review all transaction types that you had on XT.Com and then export each file that contains these transaction types. This guide includes descriptions of the data included in each file as well as step-by-step instructions for importing each file into CoinLedger.

Did this answer your question?

😞😐😃