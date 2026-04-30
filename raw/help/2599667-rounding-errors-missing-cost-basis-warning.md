[Skip to main content](https://help.coinledger.io/en/articles/2599667-rounding-errors-missing-cost-basis-warning#main-content)

# Rounding Errors - Missing Cost Basis warning

Rounding errors can lead to Missing Cost Basis warnings. Here's how to work around it.

![](https://static.intercomassets.com/avatars/2783295/square_128/Image_from_iOS_%284%29-1558111212.jpg)

Written by David Kemmerer
Updated over 2 years ago

# Detecting Rounding Errors on Your Account

Cryptocurrencies that have a very low value when compared to the likes of ETH or BTC have long decimal values that are very important and significant even far after zero.

An example would be XVG. In December of 2018, 5,000 XVG was worth just 0.5 ETH.

Unfortunately, some exchanges like Binance round off these decimals rather early in the trade history file that you export. These rounding errors can add up and make it look like you are selling more of the cryptocurrency than you own when you import your CSV files into CoinLedger.

You will likely be able to tell if your Missing Cost Basis warning is being caused by a rounding error if you hover over the warning icon and see that the amount of XXX coin that you own at the time is very close but slightly less to what it says you are selling.

There are a few options for correcting these rounding errors.

# Switch to API Import

If you notice that a rounding error from the CSV import is affecting your account, you may want to switch to API import. If you do not see that API is supported for the exchange, feel free to [send a feature request](https://coinledger.canny.io/) to our Customer Support team.

# Enter the Missing Decimal Amount Manually

A temporary fix is to add an income transaction into our [Universal Manual Import template.](https://help.coinledger.io/en/articles/6028758-universal-manual-import-template-guide)

For example, if the Missing Cost Basis warning says you are attempting to sell more XVG than you own at the time of the trade and the amount you are selling is 4997, yet the amount that you own is 4994, then you should add an incoming transaction to your account showing that you received XVG at a date prior to when you were selling this coin. You can also do this [by adding a single transaction](https://help.coinledger.io/en/articles/6125080-how-to-add-single-transactions-in-app) into the CoinLedger app showing you received XVG.

This fix will have little to no effect on your true tax position as long as you add enough of the coin just to fix the rounding error.

Did this answer your question?

😞😐😃