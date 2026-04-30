[Skip to main content](https://help.coinledger.io/en/articles/6161888-security-and-privacy-your-questions-answered#main-content)

# Security and Privacy-Your Questions Answered

Read this article to learn more about CoinLedger's privacy and security philosophy, and why your data is safe and secure on our platform

![](https://static.intercomassets.com/avatars/2781162/square_128/intercom_1545091780223-1545091844.jpg)

Written by Lucas Wyland
Updated over a year ago

At CoinLedger, respect for the security of our users' data is foundational to our company and the products we offer. Below, we'll explain our security and privacy philosophy, and why you can be 100% confident in the safety of your data when using our service to do your crypto taxes or track your portfolio.

# Privacy-First, From Day One

Every aspect of our app-from the sign-up page, to the import process, and the final steps of generating your tax reports or tracking your portfolio-is designed with protecting your privacy and personal information in mind.

This starts when you first sign up for our service. When creating a new account, we don't require _any_ personal identifying information from our users. All that's needed to open an account with us is a valid email address-we will **_never_** prompt our users to share any of their personal information, such as a Social Security number, address, phone number or sensitive financial data during the account signup flow. This data is not needed to do your crypto taxes.

# No Information is Reported to the IRS

CoinLedger does not report **any** of your tax information to the IRS. Since we're not a cryptocurrency broker, we are not obligated by law to send any of your data to the IRS.

# Password & Credential Storage

CoinLedger enforces a password complexity standard and all credentials are hashed using a PBKDF2 function with HMAC-SHA256, 128-bit salt, 256-bit subkey, 10000 iterations.

# Traffic Encryption

All data sent to or from CoinLedger is encrypted in transit using 256 bit encryption. Our API and application endpoints are TLS/SSL only.

# Virtual Private Cloud

All of our servers are within our own virtual private cloud (VPC) with network access control lists (ACLs) that prevent unauthorized requests and malicious agents from getting to our internal network.

# Failover and Data Recovery

CoinLedger was built with disaster recovery in mind. Our infrastructure is spread across multiple availability zones and will continue to work should any one of them fail.

# PCI Obligations

All payments made to CoinLedger are processed through our payment partner, Stripe. Information about their security and PCI compliance can be found on Stripe’s [security page.](https://stripe.com/docs/security)

# Transaction Data

Exchange integrations require an API connection or a transaction history file to be uploaded. During API imports, CoinLedger requires read-only permissions and never has access to your funds or your private keys. During file imports, CoinLedger only reads the relevant transaction history into memory before discarding the file. Your personal information is never saved into our database.

# Data Control

From within your account, you have the ability to delete all transaction data and exchange API connections. This will completely delete all trades, incoming transactions, outgoing transactions, and exchange account connections. Learn more [here.](https://stripe.com/docs/security)

# Important Disclaimer

**CoinLedger does not offer phone support and will ONLY contact you via email**(or through Intercom chats if you have initiated a conversation with us). Our Support Team will NEVER contact you via phone. Only customers from CoinLedger's Done For You service may receive an occasional follow-up phone call from the CoinLedger team after filling out our Done For You questionnaire.

CoinLedger does not collect personal information such as phone numbers, addresses, or Social Security numbers from its users during our account signup flow.

Still have questions about your account data? We encourage you to reach out to our Customer Support Team anytime!

Did this answer your question?

😞😐😃