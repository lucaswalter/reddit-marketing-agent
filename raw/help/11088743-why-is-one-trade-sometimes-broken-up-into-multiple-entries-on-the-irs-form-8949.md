[Skip to main content](https://help.coinledger.io/en/articles/11088743-why-is-one-trade-sometimes-broken-up-into-multiple-entries-on-the-irs-form-8949#main-content)

# Why is one trade sometimes broken up into multiple entries on the IRS Form 8949?

![](https://static.intercomassets.com/avatars/5378340/square_128/IMG_7309-1710949486.jpeg)

Written by Benjamin Yoder
Updated over 8 months ago

Occasionally, one "disposal" or sale of crypto will be listed on the IRS Form 8949 as multiple smaller transactions. If you see this on your Form 8949, don't panic! What you’re seeing is normal and is not an error with your report. Instead, it's a result of how crypto trades are broken down on the IRS Form 8949.

Specifically, the IRS Form 8949 displays your "disposals" of crypto (events where you sold or traded away your crypto) according to the **date acquired** and the **date sold.** The _date acquired_ \+ _cost or other basis_ columns represent your [cost basis](https://help.coinledger.io/en/articles/6145354-how-is-cost-basis-calculated) (how much you purchased your crypto for and when you purchased it), while the _date sold_ \+ _proceeds_ columns represent the day the transaction occurred + the proceeds from the transaction.

The reason that one crypto disposal is sometimes broken down into multiple lines on the Form 8949 is because our software is showing the IRS which cost basis "lots" we [drew from](https://help.coinledger.io/en/articles/3130354-which-crypto-tax-accounting-methods-does-coinledger-support) when calculating your gains and losses. This isn’t a bug or an attempt to mislead— **_it’s actually CoinLedger following IRS guidelines and presenting your trades on the 8949 in the manner that the government requires._** We have to show the IRS which cost basis we used when calculating your gains and losses.

Here's an example illustrating what this looks like.

Let's say I bought a total of 2,000 USDT across seven different occasions in 2023:

April 9th, 2023

April 9th, 2023

May 8th, 2023

June 5th, 2023

June 26th, 2023

July 16th, 2023

October 19th, 2023

Each of these different purchases become my cost basis for USDT.

Later, on March 6th, 2024 I decide to sell this 2,000 USDT. This one disposal will be broken up into seven different lines on the IRS Form 8949 to show the IRS which cost basis is being used to calculate my capital gains. In other words, these seven different lines represent the seven different acquisitions of my USDT.

Here's what this will look like on the 8949:

![](https://downloads.intercomcdn.com/i/o/q3bdiij1/1477471971/c2a3a4e21f38b791d328f9c7c6bd/Screenshot%2B2025-04-14%2Bat%2B11_49_44-E2-80-AFAM.png?expires=1776713400&signature=d99a762f7edb729523130cc33b60c0df9a2f9c7a8078204a0f2148f2ed0181d8&req=dSQgEc15nIhYWPMW1HO4zZvZiGKucu1UEo9tsHaYVfSj%2F8omRhNEb1XOx4%2FJ%0ARvJrBjkrKz7sSYGbcMk%3D%0A)

On each line, you can see the Date Acquired and the Date Sold, broken down like this:

Line 3: Date Acquired: May 8th \| Date Sold: March 6th

You can also see the **_Cost Basis_** used to calculate your gains and losses on each line. Remember that cost basis represents the original value of an asset for tax purposes. It is used to determine your capital gains/losses incurred whenever you dispose of your crypto. The cost basis CoinLedger uses for your disposals depends on the report calculation method on your account. To learn more about how calculation methods work, please see this guide: [https://help.coinledger.io/en/articles/3130354-which-report-calculation-methods-does-coinledger-support](https://help.coinledger.io/en/articles/3130354-which-report-calculation-methods-does-coinledger-support)

So, in summary, if you're seeing one crypto trade broken down into multiple entries on your Form 8949, this isn't an error with your report. It is CoinLedger following IRS guidelines and showing the IRS:

1. How you acquired your crypto and when

2. What cost basis was used to determine your proceeds

3. The proceeds from this transaction

4. The gain or loss from this transaction


It is perfectly normal for one disposal to be split up into multiple entries on this form.

Did this answer your question?

😞😐😃