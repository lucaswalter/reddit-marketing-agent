[Skip to main content](https://help.coinledger.io/en/articles/10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28#main-content)

# How will CoinLedger support new per-wallet cost basis tracking rules (IRS Rev. Proc 2024-28)?

What is required of me to comply with these changes?

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 4 months ago

IRS Per-Wallet Reporting Explained (2026) — What CoinLedger Users Need to Do - YouTube

Tap to unmute

[IRS Per-Wallet Reporting Explained (2026) — What CoinLedger Users Need to Do](https://www.youtube.com/watch?v=cs_oT9scPn8) [CoinLedger](https://www.youtube.com/channel/UCFSHCk0kap5Y8aWyAQau8YQ)

![thumbnail-image](https://yt3.ggpht.com/ctd8ZHtWdh8skDTCpCWDGp39j3Y1hFRNTV0DQmHlAj7VlNPh9ZfPaF3YA4RJjYKWqpwG7f-SZA=s68-c-k-c0x00ffffff-no-rj)

CoinLedger13.5K subscribers

In July 2024, the IRS issued [Revenue Procedure 2024-28](https://www.irs.gov/irb/2024-31_irb#REV-PROC-2024-28) (Rev. Proc. 2024-28). This procedure makes it mandatory for US crypto investors to use a per-wallet cost-basis tracking method when calculating gains and losses for tax purposes starting January 1, 2025. The universal cost basis tracking method will no longer be allowed beginning in tax year 2025.

## Universal vs. Per-Wallet Cost Basis Tracking (Explained)

Historically, most crypto investors have used a universal cost basis tracking method when accounting for their gains or losses each year. This is the method that CoinLedger has used for US-based investors. Moving forward, it is now mandatory for US investors to use a per-wallet cost basis tracking method. Read the examples below for a breakdown of Universal vs Per Wallet tracking.

### Universal Tracking Method Example

Under the Universal tracking method, all transactions for a particular coin across various wallets are combined into a single queue for accounting purposes. This means the cost basis used when accounting for the sale of a coin may originate from any wallet, irrespective of where the sale occurs.

To help illustrate Universal tracking, let’s say you have the following transaction history:

- **Jul 1** \- Buy 1 BTC @ $10,000 in Exchange A

- **Aug 1** \- Buy 1 BTC @ $20,000 in Exchange B

- **Sep 1** \- Buy 1 BTC @ $30,000 in Exchange C

- **Oct 1** \- Sell 1 BTC @ $40,000 in Exchange C


Under universal tracking, this transaction history gets combined into one queue for accounting purposes—as if all of this history occurred within 1 exchange or 1 wallet.

When crypto tax software like CoinLedger is accounting for the sale of 1 BTC from Exchange C, it can pull the ‘tax lot’ from Exchange A.

In fact, this is exactly what CoinLedger would do when using [First-in First-out (FIFO)](https://coinledger.io/blog/cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained). It would look for the first BTC purchase and account for that unit being sold first (hence first-in, first-out). Therefore, using the universal tracking method, your taxable gain for the Sep 1 sale would be **$30,000** ($40,000 - $10,000).

### Per-Wallet Cost Basis Tracking Example

Let's again use the same example transaction history:

- **Jul 1** \- Buy 1 BTC @ $10,000 in Exchange A

- **Aug 1** \- Buy 1 BTC @ $20,000 in Exchange B

- **Sep 1** \- Buy 1 BTC @ $30,000 in Exchange C

- **Oct 1** \- Sell 1 BTC @ $40,000 in Exchange C


Under the per-wallet cost basis tracking method, CoinLedger can’t pull ‘tax lots’ from wallets or exchanges outside of the one where the sale is actually occurring. The cost basis for the Sep 1 sale from Exchange C has to come **from Exchange C**, hence ‘per-wallet’ tracking.

So using the per-wallet tracking method, CoinLedger would calculate this user’s gain to be $10,000 ($40,000 - $30,000).

## How can I migrate to per-wallet cost basis tracking?

If you are an existing user that used CoinLedger before 2026, you will need to opt-in to per wallet cost basis tracking to ensure that you are in compliance with the new IRS rules. You can do so by following the steps below.

**NOTE**: If you are a new US user that signed up for CoinLedger after November 4th, 2025, per wallet cost basis tracking will be enabled on your account by default. No action needs to be taken to migrate your account to per wallet tracking.

Before migrating to per wallet tracking, we recommend going through the following steps on your account:

- Import all exchanges, wallets and blockchains you have used over the years, going back to the beginning of your trading history

- Review and resolve [Missing Cost Basis Warnings](https://help.coinledger.io/en/articles/2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it) or [Historical Price Warnings](https://help.coinledger.io/en/articles/4357024-how-can-i-solve-a-historical-price-warning) on your account

- Merge all potential trades, transfers and bridges on the Transactions page (more information [here](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab))

- Review and resolve all uncategorized transactions (more information [here](https://help.coinledger.io/en/articles/6110498-how-to-classify-uncategorized-transactions))


Once you have completed these steps, you can begin the migration process.

**Step 1**

Navigate to the Tax Reports page, and opt-in to per wallet tracking by hitting **Accept and Continue** on the menu shown below.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1814814826/1ee31d09cc3e362e809d4ab716f0/Screenshot+2025-11-05+at+9_52_23%E2%80%AFAM.png?expires=1776713400&signature=006010223bfde95cb316f488237fc7d4ae5e2dca2e2f00c167d1297d9b8730e5&req=dSgmEsF%2FmYldX%2FMW1HO4zaPDmhYcg9WSztRTESxjqr2Dfcic1d0KOiNrQ24U%0AChNujJkp73QdDeo6A60%3D%0A)

**Step 2**

Now, your account will be switched to per wallet cost basis tracking. To confirm that the migration was successful, navigate to the 2025 Tax Report page. If the migration was successful, your Cost Basis Tracking method will show as **Per-Wallet.**

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1814917228/f7439d94cba722e09a35ce61aea0/Screenshot+2025-11-05+at+11_12_19%E2%80%AFAM.png?expires=1776713400&signature=5a642c7d6320badb759bd84faf227e39f6d2d22a744e1d369081973f57213e38&req=dSgmEsB%2FmoNdUfMW1HO4zcUHTEMHgH0vWVJsKdzRKj06dcHInYUX9uAnIifK%0AHCgG62lExgKdw68GZpY%3D%0A)

**Step 3**

After this, we recommend reviewing your asset balances on the [Portfolio Tracker](https://app.coinledger.io/individual/portfolio) to ensure that they match your actual holdings. If your portfolio balances are not accurate, this is a signal that you are missing transaction history data, which may have affected the cost basis reallocation process.

**Step 4**

Next, we recommend checking your account for any [Potential Trades, Transfers and Bridges](https://help.coinledger.io/en/articles/10714995-what-is-the-potential-bridges-trades-and-transfers-tab) that have been flagged by our system. If you see any of these on the [Transactions page](https://app.coinledger.io/individual/transactions), you should merge them together. Merging unmatched transfers and bridges together is crucial to ensuring that your cost basis is carried over correctly under the per-wallet rules.

**Step 5**

Finally, now that the migration process has been completed, we recommend reviewing the [Reallocation Breakdown Report](https://app.coinledger.io/individual/reallocation-breakdown-report) to see how your tax lots were reallocated. You should check for any [Unmatched Deposits and Withdrawals](https://help.coinledger.io/en/articles/12771568-what-is-the-reallocation-breakdown-report#:~:text=Unmatched%20Deposits%20and%20Withdrawals%3A) and other warnings on this page.

If you’ve completed each of these steps, your migration to per-wallet cost basis tracking is now complete. You are now in compliance with the latest IRS rules.

## How does the cost basis reallocation process work?

If you have used CoinLedger in the past, and you have cryptocurrencies that you are still holding, then CoinLedger needs to allocate the outstanding cost basis of your holdings to the specific accounts (wallets/exchanges) you hold crypto in. This will enable CoinLedger to calculate your gains/losses on a per-wallet basis in the future.

To facilitate users with this migration, CoinLedger will automatically allocate any outstanding basis to your wallets based on a Lowest-Cost, Highest-Wallet method. CoinLedger will also provide support for Highest-Cost, Highest-Wallet reallocation, and this can be configured on your tax settings.

Click the drop-down menu below to learn more about the Lowest-Cost, Highest-Wallet method.

### Lowest-Cost, Highest-Wallet reallocation

Here's an example of Lowest-Cost, Highest-Wallet reallocation.

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1527657763/a8326c639552afbb5b524f0745f3/AD_4nXdVJ3YxMVSz1q-_lzvf8mtS50Y6SJw6aer49oNGuuY5YbCCDhcMozm85LpJai1kdXRzqrcEUsJoOa9eVdYKnfe68cH8i_EQroxpd8wxKAyHjgVu4WN0q9mpF6F4jXz--jTUzA4?expires=1776713400&signature=093eba7bc3b7fe66e5fa766b2219995120fa77d43209542c1e3a3111283325db&req=dSUlEc97moZZWvMW1HO4zcjGgs97f%2FgW1Vv9uik5cdIX%2FfNC%2FVHEVinER%2FmI%0A64zd%0A)

In the image above, we can see that we have 4 outstanding tax lots of Ethereum. Each lot was purchased at a different spot price of ETH (per unit price), and each tax lot thus has different cost basis.

Under the universal method, CoinLedger is accounting for this outstanding basis in the same queue (or in one _universal_ wallet). To migrate to per-wallet tracking, we need to allocate the outstanding cost basis to the three different wallets we hold ETH in.

By using the lowest-cost highest-wallet method, we will allocate the **lowest** per-unit cost basis lot, lot 1, to the wallet with the **highest** balance of ETH, Wallet A. Lot 1 has 1.35 units of ETH (at $1,290 per ETH), so we completely expend this lot when allocating to Wallet A.

We then go to the next lowest cost tax lot, lot 2. With only 0.578 units of ETH in this tax lot, we also completely expend this lot allocating to Wallet A. So now, Wallet A has been allocated 1.928 ETH (1.35 + 0.578).

We repeat this process again and go to the next lowest cost tax lot, lot 3. This lot consists of 2.57 total ETH (at $2,876 per ETH), so we first allocate 1.072 of this ETH to Wallet A (which completely exhausts wallet A as it has now been allocated 3 units of ETH). We then allocate the remaining 1.498 ETH to Wallet B, which is the next highest balance wallet of ETH across our three wallets.

We repeat this same process until all of our outstanding tax lots, and the associated cost basis, have been allocated.

Now in the future, when we make a sale from Wallet A, Wallet B, or Wallet C, we can pull from the cost basis that were allocated to each individual wallet.

## Do you offer other cost-basis reallocation methods?

Yes. In addition to lowest-cost, highest-wallet, CoinLedger also supports highest-cost, highest-wallet.

If you hold most of your crypto in a cold storage wallet, using the lowest-cost, highest-wallet method (default) will allocate your lowest cost basis coins to that cold wallet. This can be helpful for qualifying for long-term capital gains and minimizing your tax burden.

There may be circumstances where you want to allocate your highest cost coins to your highest balance wallets. This method is also supported, but it is not the default method.

You should select which method you want CoinLedger to use on your account before Jan 1, 2025. You can do this by making this selection within the **Tax Settings** of your CoinLedger account. Learn more about this process [HERE](https://help.coinledger.io/en/articles/10314185-how-do-i-change-my-cost-basis-reallocation-method-irs-rev-proc-2024-28).

By default, USA users will be selected to use the lowest-cost, highest-wallet method.

Consult your tax professional if you have questions about which reallocation method is best for your specific circumstances.

## What was required of me before Dec 31st, 2024 to comply with this new IRS guidance?

There are two things you were required to do before Dec 31st, 2024 to be in compliance with these new IRS rules:

1. Declaring your cost basis reallocation method by saving the email sent from CoinLedger

2. Making sure your CoinLedger account was fully up to date on Dec 31


## Learn more about these actions taken before December 31st, 2024:

In Rev. Proc 2024-28, the IRS stated that you must declare the method you are using to allocate outstanding cost basis prior to Jan 1, 2025. If you did not make this declaration, you may not have qualified for Safe Harbor protection.

On Dec 20 through Dec 22, 2024, CoinLedger sent email communications to all US users defining this reallocation method. You should have saved a copy of this email for your records as your declaration.

Note - to make your declaration, you did not need to physically send anything to the IRS. You simply needed to have records of the declaration that clearly documented the process by which you were allocating your outstanding cost basis.

Additionally, prior to the end of the year and on Dec 31, 2024, you should have made sure that your CoinLedger account was fully up to date. This means you should fully import all of your 2024 and prior transactions, add all wallets and or exchanges, and make sure the tracked balances in your Portfolio are accurate.

## Frequently Asked Questions

Below are the most common questions we receive from users about the switch from Universal cost basis tracking to Per-Wallet cost basis tracking.

## FAQ's

## What do I need to do before Dec. 31, 2024 to prepare for this change?

You should do two things prior to the end of the year to prepare for this change:

1. Declare the reallocation method you are using (by saving the email from CoinLedger)

2. Make sure your CoinLedger account is up to date on Dec 31


## Should I transfer all of my crypto/consolidate it into one wallet or account before Jan 1st?

This is not necessary. However, it can make future cost basis tracking easier, as it essentially replicates the universal wallet tracking method that CoinLedger has used historically.

## Can I use the email CoinLedger sent as a declaration letter?

Yes, you should save the email CoinLedger sent you as the declaration for the reallocation method you are using. CoinLedger will also save the reallocation method used on your account for future reference.

## Do I need to physically sign a form or send one to the IRS to declare my cost basis reallocation method?

No. You do not need to send a physical form to the IRS or sign a physical form in order to declare how you are reallocating your outstanding cost basis. You simply need to have records of the declaration that clearly document the process by which you are allocating your outstanding cost basis.

On Dec 20 through Dec 22, 2024, CoinLedger sent email communications to all US users defining this reallocation method. You should save a copy of this email for your records as your declaration.

## Will CoinLedger send me a 1099-DA? If so, will I need to fill anything in the 1099 DA and send it to the IRS?

CoinLedger is not a broker nor a cryptocurrency exchange, and thus is not the entity required to file 1099’s to you nor the IRS. You will only receive 1099-DA’s from the brokers you used starting in Jan. 2026. You can use future 1099-DA’s in tandem with CoinLedger to effectively track and report your crypto tax activity.

[Learn more about 1099-DA here](https://coinledger.io/blog/form-1099-da).

## Will you be using FIFO for your digital asset allocation plan?

No. CoinLedger will be defaulting all US users to use the lowest-cost, highest-balance allocation method.

## How will you assign cost basis? Will you assign it to hosted accounts first, and then unhosted accounts?

Cost basis will be assigned based on wallet holdings. Lowest cost tax lots will be allocated to highest wallet balances first.

## What if I store my crypto in self custody/cold storage wallets?

This is normal, and you do not need to move any of your crypto to comply with these requirements. You should however have your self-custody wallet and the associated transactions (deposits, withdrawals, and transfers) imported to CoinLedger.

## What if I use only one exchange for all my transactions?

If you are using only one exchange (e.g., Coinbase) without any connected external wallets, you may not need to configure additional settings for per-wallet cost basis. This is because account-specific exchanges internally allocate cost basis, which CoinLedger can directly report. However, ensuring completeness of your transactions is still essential.

## What if I don't have the email communications or files from CoinLedger?

If you failed to receive critical updates or documents (e.g., the CoinLedger email introducing these rules), you can retrieve the necessary steps and declarations from official CoinLedger support channels or documentation.

Did this answer your question?

😞😐😃