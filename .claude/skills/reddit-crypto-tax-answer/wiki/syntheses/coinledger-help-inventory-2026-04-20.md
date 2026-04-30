---
title: CoinLedger help center inventory (2026-04-20 snapshot)
type: synthesis
created: 2026-04-20
updated: 2026-04-20
tags: [inventory, coinledger-product, help-center]
---

## TL;DR

Snapshot of **324 CoinLedger help-center articles** on 2026-04-20 (Intercom-hosted). This is product support documentation — import how-tos, error explanations, billing/account FAQs, reconciliation workflow — not editorial. The shape of the help center tells you CoinLedger's product surface is **dominated by ingestion**: roughly **196/324 articles (~60%)** are pure import guides across exchanges, wallets, chains, or CSV templates. Another **~46** cluster around cost-basis, reconciliation, and import-troubleshooting — where users actually get stuck. Tax-report generation, filing-software integrations, account/billing, pro services, and portfolio-tracker docs round out the long tail. Four jurisdictions get their own help page (UK, AU, CA, NZ), each extremely thin — the heavy jurisdiction lift happens on the blog/guides, not the help center. Rev. Proc. 2024-28 / per-wallet cost-basis reallocation is the clear **2025–26 editorial push** inside the help center (8+ dedicated articles), mirroring the 1099-DA surge on the blog.

**Signal tiers:** 63 high · 229 medium · 32 low.

**Integration breadth from help-center coverage alone:** **91 exchanges**, **22 wallets**, **51 blockchains/networks**, **5 on-chain protocols** (DEX + NFT marketplace). This is an order of magnitude less than the homepage's "100+ exchanges / 60+ wallets / 30+ chains" and far less than the pricing page's "1,000+ integrations" claim. The gap is real: the help center only gets a dedicated article for the **top tier** of integrations — the long tail is served by universal CSV and wallet-address flows.

## Integration coverage table

Every exchange, wallet, chain, and on-chain protocol that has at least one dedicated help article. Method codes in parentheses reflect which import paths the help center documents for that integration (CSV = file upload, API = API keys, OAuth = OAuth-flow API, wallet-address = on-chain by address).

### Exchanges (91)

- **Abra** (CSV) — [[coinledger-help-2883872-abra-file-import-guide-2026-04-20]]
- **AnchorUSD** (CSV) — [[coinledger-help-5563401-anchorusd-file-import-guide-2026-04-20]]
- **BTC Markets** (CSV) — [[coinledger-help-3211479-btc-markets-file-import-guide-2026-04-20]]
- **BYDFi** (CSV) — [[coinledger-help-6678831-bydfi-file-import-guide-2026-04-20]]
- **Bibox** (API, CSV) — [[coinledger-help-5397368-bibox-file-import-guide-2026-04-20]], [[coinledger-help-5714606-bibox-api-import-guide-2026-04-20]]
- **Bilaxy** (CSV) — [[coinledger-help-5300306-bilaxy-file-import-guide-2026-04-20]]
- **Binance** (other) — [[coinledger-help-4993804-import-fiat-purchases-from-binance-2026-04-20]]
- **Binance (Convert)** (CSV) — [[coinledger-help-6036926-binance-convert-history-file-import-guide-2026-04-20]]
- **Binance (P2P)** (CSV) — [[coinledger-help-7174368-binance-p2p-trade-history-file-import-guide-2026-04-20]]
- **Binance.US** (API, CSV) — [[coinledger-help-4935722-binance-us-file-import-guide-2026-04-20]], [[coinledger-help-4936070-binance-us-api-import-guide-2026-04-20]]
- **Binance.com** (API, CSV) — [[coinledger-help-2757038-binance-com-api-import-guide-2026-04-20]], [[coinledger-help-5042261-binance-com-file-import-guide-2026-04-20]]
- **BitBuy** (CSV) — [[coinledger-help-6520289-bitbuy-file-import-guide-2026-04-20]]
- **BitMart** (API) — [[coinledger-help-5509368-bitmart-api-import-guide-2026-04-20]]
- **BitPay** (CSV) — [[coinledger-help-7257609-bitpay-file-import-guide-2026-04-20]]
- **Bitbns** (CSV) — [[coinledger-help-6868840-bitbns-file-import-guide-2026-04-20]]
- **Bitfinex** (API, CSV) — [[coinledger-help-3222934-bitfinex-file-import-guide-2026-04-20]], [[coinledger-help-5799736-bitfinex-api-import-guide-2026-04-20]]
- **Bitget** (API) — [[coinledger-help-9628213-bitget-api-import-guide-2026-04-20]]
- **Bitpanda** (CSV) — [[coinledger-help-6803203-bitpanda-file-import-guide-2026-04-20]]
- **Bitpanda Pro** (CSV) — [[coinledger-help-6803202-bitpanda-pro-file-import-guide-2026-04-20]]
- **Bitrue** (API, CSV) — [[coinledger-help-3620033-bitrue-file-import-guide-2026-04-20]], [[coinledger-help-9519226-bitrue-api-import-guide-2026-04-20]]
- **Bitstamp** (API, CSV) — [[coinledger-help-2819071-bitstamp-file-import-guide-2026-04-20]], [[coinledger-help-5509445-bitstamp-api-import-guide-2026-04-20]]
- **Bittrex** (CSV) — [[coinledger-help-2535265-bittrex-file-import-guide-2026-04-20]]
- **Blockonomics** (CSV) — [[coinledger-help-8513973-blockonomics-file-import-guide-2026-04-20]]
- **Bybit** (API, CSV) — [[coinledger-help-6588913-bybit-api-import-guide-2026-04-20]], [[coinledger-help-6601040-bybit-file-import-guide-2026-04-20]]
- **CEX.IO** (CSV) — [[coinledger-help-2993302-cex-io-file-import-guide-2026-04-20]]
- **Caleb & Brown** (CSV) — [[coinledger-help-10438698-caleb-brown-file-import-guide-2026-04-20]]
- **Cash App** (CSV) — [[coinledger-help-3226133-cash-app-by-square-file-import-guide-2026-04-20]]
- **Changelly** (CSV) — [[coinledger-help-2874136-changelly-file-import-guide-2026-04-20]]
- **CoinDCX** (CSV) — [[coinledger-help-6999470-coindcx-file-import-guide-2026-04-20]]
- **CoinEx** (API, CSV) — [[coinledger-help-10523461-coinex-api-import-guide-2026-04-20]], [[coinledger-help-5091142-coinex-file-import-guide-2026-04-20]]
- **CoinJar** (CSV) — [[coinledger-help-3009980-coinjar-file-import-guide-2026-04-20]]
- **CoinJar (OAuth)** (OAuth) — [[coinledger-help-5588645-coinjar-oauth-import-guide-2026-04-20]]
- **CoinJar Exchange** (API) — [[coinledger-help-5588686-coinjar-exchange-api-import-guide-2026-04-20]]
- **CoinSpot** (API, CSV) — [[coinledger-help-3211371-coinspot-file-import-guide-2026-04-20]], [[coinledger-help-6201854-coinspot-api-import-guide-2026-04-20]]
- **CoinStats** (partnership) — [[coinledger-help-6878347-coinstats-and-coinledger-partnership-details-2026-04-20]]
- **CoinSwitch** (CSV) — [[coinledger-help-6868850-coinswitch-file-import-guide-2026-04-20]]
- **Coinbase** (API, CSV) — [[coinledger-help-2535264-coinbase-file-import-guide-2026-04-20]], [[coinledger-help-2986974-coinbase-api-import-guide-2026-04-20]]
- **Coinbase Pro (legacy)** (CSV) — [[coinledger-help-2535269-coinbase-pro-file-import-guide-2026-04-20]]
- **Coinsquare** (CSV) — [[coinledger-help-10708065-coinsquare-file-import-guide-2026-04-20]]
- **Cointree** (API, CSV) — [[coinledger-help-6448568-cointree-file-import-guide-2026-04-20]], [[coinledger-help-9558925-cointree-api-import-guide-2026-04-20]]
- **Crypto.com** (API, CSV) — [[coinledger-help-10446058-crypto-com-api-import-guide-2026-04-20]], [[coinledger-help-3742825-crypto-com-file-import-guide-2026-04-20]]
- **Digital Surge** (API, CSV) — [[coinledger-help-6456629-digital-surge-file-import-guide-2026-04-20]], [[coinledger-help-6463765-digital-surge-api-import-guide-2026-04-20]]
- **EasyCrypto** (CSV) — [[coinledger-help-6721622-easycrypto-file-import-guide-2026-04-20]]
- **Gate.io** (API, CSV) — [[coinledger-help-2897126-gate-file-import-guide-2026-04-20]], [[coinledger-help-6404841-gate-api-import-guide-2026-04-20]]
- **Gemini** (API) — [[coinledger-help-5559374-gemini-api-import-guide-2026-04-20]]
- **Graviex** (CSV) — [[coinledger-help-5397389-graviex-file-import-guide-2026-04-20]]
- **HitBTC** (API, CSV) — [[coinledger-help-2956906-hitbtc-file-import-guide-2026-04-20]], [[coinledger-help-5609022-hitbtc-api-import-guide-2026-04-20]]
- **IDEX** (CSV) — [[coinledger-help-5144931-idex-file-import-guide-2026-04-20]]
- **Independent Reserve** (API, CSV) — [[coinledger-help-6466808-independent-reserve-file-import-guide-2026-04-20]], [[coinledger-help-6467089-independent-reserve-api-import-guide-2026-04-20]]
- **Kraken** (API) — [[coinledger-help-5509209-kraken-api-import-guide-2026-04-20]]
- **Kraken (Ledgers)** (CSV) — [[coinledger-help-5338231-kraken-ledgers-file-import-guide-2026-04-20]]
- **KuCoin** (API, CSV) — [[coinledger-help-2624452-kucoin-alternate-file-import-guide-2026-04-20]], [[coinledger-help-5603669-kucoin-api-import-guide-2026-04-20]], [[coinledger-help-8196376-kucoin-file-import-guide-2026-04-20]]
- **Liquid** (API) — [[coinledger-help-5721072-liquid-api-import-guide-2026-04-20]]
- **Luno** (CSV) — [[coinledger-help-6819251-luno-file-import-guide-2026-04-20]]
- **Luxor** (API, CSV) — [[coinledger-help-5541196-luxor-api-import-guide-2026-04-20]], [[coinledger-help-5541250-luxor-file-import-guide-2026-04-20]]
- **Lykke** (CSV) — [[coinledger-help-6580456-lykke-file-import-guide-2026-04-20]]
- **MEXC** (CSV) — [[coinledger-help-6929791-mexc-file-import-guide-2026-04-20]]
- **Mandala** (CSV) — [[coinledger-help-7210782-mandala-file-import-guide-2026-04-20]]
- **Mercatox** (CSV) — [[coinledger-help-6077956-mercatox-file-import-guide-2026-04-20]]
- **Metal Pay** (CSV) — [[coinledger-help-8538830-metal-pay-file-import-guide-2026-04-20]]
- **MoonPay** (CSV) — [[coinledger-help-7238606-moonpay-file-import-guide-2026-04-20]]
- **NDAX** (API, CSV) — [[coinledger-help-6518867-ndax-file-import-guide-2026-04-20]], [[coinledger-help-6563578-ndax-api-import-guide-2026-04-20]]
- **Nexo** (CSV) — [[coinledger-help-3646973-nexo-file-import-guide-2026-04-20]]
- **NiceHash** (API, CSV) — [[coinledger-help-5210159-nicehash-file-import-guide-2026-04-20]], [[coinledger-help-5521536-nicehash-api-import-guide-2026-04-20]]
- **OKX** (CSV) — [[coinledger-help-5052913-okx-okex-file-import-guide-2026-04-20]]
- **Paxful** (CSV) — [[coinledger-help-5357920-paxful-file-import-guide-2026-04-20]]
- **PayPal** (CSV) — [[coinledger-help-6531809-paypal-file-import-guide-2026-04-20]]
- **Phemex** (CSV) — [[coinledger-help-5338205-phemex-file-import-guide-2026-04-20]]
- **Pionex** (API, CSV) — [[coinledger-help-6975867-pionex-api-import-guide-2026-04-20]], [[coinledger-help-7175790-pionex-file-import-guide-2026-04-20]]
- **Poloniex** (CSV) — [[coinledger-help-2535271-poloniex-file-import-guide-2026-04-20]]
- **River** (CSV) — [[coinledger-help-8977397-river-file-import-guide-2026-04-20]]
- **Robinhood** (API) — [[coinledger-help-2886575-robinhood-api-import-guide-2026-04-20]]
- **Shakepay** (CSV) — [[coinledger-help-6534905-shakepay-file-import-guide-2026-04-20]]
- **ShapeShift** (CSV) — [[coinledger-help-5166199-shapeshift-file-import-guide-2026-04-20]]
- **SimpleSwap** (CSV) — [[coinledger-help-10574174-simpleswap-file-import-guide-2026-04-20]]
- **StormGain** (CSV) — [[coinledger-help-6998620-stormgain-file-import-guide-2026-04-20]]
- **Strike** (CSV) — [[coinledger-help-6611946-strike-file-import-guide-2026-04-20]]
- **Swan Bitcoin** (CSV) — [[coinledger-help-4986835-swan-bitcoin-file-import-guide-2026-04-20]]
- **Swyftx** (API, CSV) — [[coinledger-help-5210113-swyftx-file-import-guide-2026-04-20]], [[coinledger-help-5563259-swyftx-api-import-guide-2026-04-20]]
- **TradeStation** (CSV) — [[coinledger-help-6494746-tradestation-file-import-guide-2026-04-20]]
- **Uphold** (API, CSV) — [[coinledger-help-2949597-uphold-file-import-guide-2026-04-20]], [[coinledger-help-3522999-uphold-api-import-guide-2026-04-20]]
- **Venmo** (CSV) — [[coinledger-help-5964845-venmo-file-import-guide-2026-04-20]]
- **VirgoCX** (CSV) — [[coinledger-help-6521890-virgocx-file-import-guide-2026-04-20]]
- **Voyager (defunct)** (other, partnership) — [[coinledger-help-10317411-can-you-help-me-get-my-voyager-check-2026-04-20]], [[coinledger-help-5914394-voyager-and-coinledger-partnership-details-2026-04-20]], [[coinledger-help-8737058-how-do-i-report-my-voyager-bankruptcy-losses-on-my-taxes-2023-and-earlier-2026-04-20]], [[coinledger-help-9828969-how-do-i-report-my-voyager-bankruptcy-distribution-from-2024-on-my-taxes-2026-04-20]]
- **Waves** (CSV) — [[coinledger-help-7029564-waves-file-import-guide-2026-04-20]]
- **WazirX** (CSV) — [[coinledger-help-6796459-wazirx-file-import-guide-2026-04-20]]
- **Webull** (CSV) — [[coinledger-help-7266700-webull-file-import-guide-2026-04-20]]
- **WhiteBIT** (CSV) — [[coinledger-help-7056513-whitebit-file-import-guide-2026-04-20]]
- **XT.com** (CSV) — [[coinledger-help-6853409-xt-com-file-import-guide-2026-04-20]]
- **ZebPay** (CSV) — [[coinledger-help-6860164-zebpay-file-import-guide-2026-04-20]]
- **eToro** (CSV) — [[coinledger-help-6062743-etoro-file-import-guide-2026-04-20]]

### Wallets (22)

- **Arculus** — [[coinledger-help-10552877-arculus-wallet-blockchain-import-guide-2026-04-20]]
- **Argent** — [[coinledger-help-11635807-argent-wallet-blockchain-import-guide-2026-04-20]]
- **Atomic Wallet** — [[coinledger-help-6184950-atomic-wallet-blockchain-import-guide-2026-04-20]]
- **Coinbase Wallet** — [[coinledger-help-6185086-coinbase-wallet-blockchain-import-guide-2026-04-20]]
- **Electrum** — [[coinledger-help-10602298-electrum-wallet-blockchain-import-guide-2026-04-20]]
- **Exodus** — [[coinledger-help-2796020-exodus-file-import-guide-2026-04-20]]
- **Guarda** — [[coinledger-help-10573929-guarda-wallet-blockchain-import-guide-2026-04-20]]
- **Leather** — [[coinledger-help-10573916-leather-wallet-blockchain-import-guide-2026-04-20]]
- **Ledger** — [[coinledger-help-11463666-ledger-wallet-file-import-guide-2026-04-20]], [[coinledger-help-6191248-ledger-wallet-blockchain-import-guide-2026-04-20]]
- **MetaMask** — [[coinledger-help-6110244-metamask-blockchain-import-guide-2026-04-20]], [[coinledger-help-9086313-metamask-and-coinledger-partnership-details-2026-04-20]]
- **MyEtherWallet** — [[coinledger-help-10602165-myetherwallet-blockchain-import-guide-2026-04-20]]
- **Ngrave** — [[coinledger-help-10602368-ngrave-wallet-blockchain-import-guide-2026-04-20]]
- **Opera** — [[coinledger-help-10573890-opera-wallet-blockchain-import-guide-2026-04-20]]
- **Phantom** — [[coinledger-help-10458080-phantom-wallet-blockchain-import-guide-2026-04-20]]
- **Safe (Gnosis)** — [[coinledger-help-11635783-safe-wallet-gnosis-blockchain-import-guide-2026-04-20]]
- **SafePal** — [[coinledger-help-9472334-safepal-wallet-blockchain-import-guide-2026-04-20]]
- **Tangem** — [[coinledger-help-10546911-tangem-wallet-blockchain-import-guide-2026-04-20]]
- **Trezor** — [[coinledger-help-10546977-trezor-wallet-blockchain-import-guide-2026-04-20]], [[coinledger-help-11463230-trezor-wallet-file-import-guide-2026-04-20]]
- **Trust Wallet** — [[coinledger-help-6110365-trust-wallet-blockchain-import-guide-2026-04-20]]
- **Xverse** — [[coinledger-help-10602195-xverse-wallet-blockchain-import-guide-2026-04-20]]
- **Yoroi** — [[coinledger-help-7239248-yoroi-wallet-import-guide-2026-04-20]]
- **Zengo** — [[coinledger-help-10602255-zengo-wallet-blockchain-import-guide-2026-04-20]]

### Blockchains / networks (51)

- **Abstract** — [[coinledger-help-11955278-abstract-blockchain-import-guide-2026-04-20]]
- **Akash** — [[coinledger-help-9976376-akash-blockchain-import-guide-2026-04-20]]
- **Algorand** — [[coinledger-help-9715409-algorand-blockchain-import-guide-2026-04-20]]
- **ApeChain** — [[coinledger-help-10786820-apechain-blockchain-import-guide-2026-04-20]]
- **Arbitrum** — [[coinledger-help-6821127-arbitrum-blockchain-import-guide-2026-04-20]]
- **BNB Chain / BSC** — [[coinledger-help-6191928-binance-smart-chain-blockchain-import-guide-2026-04-20]]
- **Base** — [[coinledger-help-8257248-base-blockchain-import-guide-2026-04-20]]
- **Berachain** — [[coinledger-help-10715728-berachain-blockchain-import-guide-2026-04-20]]
- **Bitcoin** — [[coinledger-help-6341836-bitcoin-blockchain-import-guide-2026-04-20]]
- **Blast** — [[coinledger-help-9346654-blast-blockchain-import-guide-2026-04-20]]
- **Boba** — [[coinledger-help-10873957-boba-blockchain-import-guide-2026-04-20]]
- **Boba BNB** — [[coinledger-help-10873901-boba-bnb-blockchain-import-guide-2026-04-20]]
- **Canto** — [[coinledger-help-9888196-canto-blockchain-import-guide-2026-04-20]]
- **Cardano** — [[coinledger-help-7210960-cardano-blockchain-import-guide-2026-04-20]]
- **Celestia** — [[coinledger-help-9786847-celestia-blockchain-import-guide-2026-04-20]]
- **Celo** — [[coinledger-help-10944805-celo-blockchain-import-guide-2026-04-20]]
- **Cosmos** — [[coinledger-help-9503824-cosmos-blockchain-import-guide-2026-04-20]]
- **Dogecoin** — [[coinledger-help-10644439-dogecoin-blockchain-import-guide-2026-04-20]]
- **Ethereum** — [[coinledger-help-6097060-ethereum-blockchain-import-guide-2026-04-20]]
- **Fantom** — [[coinledger-help-6977401-fantom-blockchain-import-guide-2026-04-20]]
- **Fraxtal** — [[coinledger-help-9859122-fraxtal-blockchain-import-guide-2026-04-20]]
- **Hedera** — [[coinledger-help-8945280-hedera-hbar-blockchain-import-guide-2026-04-20]]
- **Hyperliquid** — [[coinledger-help-12589013-hyperliquid-blockchain-import-guide-2026-04-20]]
- **Injective** — [[coinledger-help-10100282-injective-blockchain-import-guide-2026-04-20]]
- **Kaspa** — [[coinledger-help-10113145-kaspa-blockchain-import-guide-2026-04-20]]
- **Kava** — [[coinledger-help-12832336-kava-blockchain-import-guide-2026-04-20]]
- **Linea** — [[coinledger-help-9065355-linea-blockchain-import-guide-2026-04-20]]
- **Lisk** — [[coinledger-help-9829027-lisk-blockchain-import-guide-2026-04-20]]
- **Litecoin** — [[coinledger-help-6499840-litecoin-blockchain-import-guide-2026-04-20]]
- **Mantle** — [[coinledger-help-9401064-mantle-blockchain-import-guide-2026-04-20]]
- **Merlin** — [[coinledger-help-9400800-merlin-blockchain-import-guide-2026-04-20]]
- **Mode** — [[coinledger-help-9346572-mode-blockchain-import-guide-2026-04-20]]
- **Oasis Sapphire** — [[coinledger-help-10452475-oasis-sapphire-blockchain-import-guide-2026-04-20]]
- **Optimism** — [[coinledger-help-6811722-optimism-blockchain-import-guide-2026-04-20]]
- **Osmosis** — [[coinledger-help-9612291-osmosis-blockchain-import-guide-2026-04-20]]
- **Polygon** — [[coinledger-help-6341830-polygon-blockchain-import-guide-2026-04-20]]
- **PulseChain** — [[coinledger-help-13941910-pulsechain-blockchain-import-guide-2026-04-20]]
- **Scroll** — [[coinledger-help-9346632-scroll-blockchain-import-guide-2026-04-20]]
- **Sei** — [[coinledger-help-10375837-sei-blockchain-import-guide-2026-04-20]]
- **Solana** — [[coinledger-help-6066844-solana-blockchain-import-guide-2026-04-20]]
- **Sonic** — [[coinledger-help-11771805-sonic-blockchain-import-guide-2026-04-20]]
- **Stacks** — [[coinledger-help-9921992-stacks-blockchain-import-guide-2026-04-20]]
- **Sui** — [[coinledger-help-9467963-sui-blockchain-import-guide-2026-04-20]]
- **TON** — [[coinledger-help-10375816-ton-blockchain-import-guide-2026-04-20]]
- **Taiko** — [[coinledger-help-10786775-taiko-blockchain-import-guide-2026-04-20]]
- **Telos** — [[coinledger-help-9833163-telos-blockchain-import-guide-2026-04-20]]
- **Terra / Luna** — [[coinledger-help-6066861-terra-luna-imports-for-coinledger-2026-04-20]]
- **Unichain** — [[coinledger-help-10730973-unichain-blockchain-import-guide-2026-04-20]]
- **World Chain** — [[coinledger-help-10786797-world-chain-blockchain-import-guide-2026-04-20]]
- **Zora** — [[coinledger-help-8646124-zora-blockchain-import-guide-2026-04-20]]
- **opBNB** — [[coinledger-help-9888314-opbnb-blockchain-import-guide-2026-04-20]]

### On-chain protocols / DEXs / NFT marketplaces (5)

- **Balancer** (DEX) — [[coinledger-help-6472141-balancer-blockchain-import-guide-2026-04-20]]
- **Jupiter** (DEX) — [[coinledger-help-11525113-how-can-i-import-my-jupiter-transactions-into-coinledger-2026-04-20]]
- **SushiSwap** (DEX) — [[coinledger-help-6106396-sushiswap-blockchain-import-guide-2026-04-20]]
- **Uniswap** (DEX) — [[coinledger-help-10670385-how-can-i-import-transactions-from-a-decentralized-exchange-like-jupiter-or-uniswap-2026-04-20]], [[coinledger-help-6105876-uniswap-blockchain-import-guide-2026-04-20]]
- **OpenSea** (NFT marketplace) — [[coinledger-help-6105701-opensea-blockchain-import-guide-2026-04-20]]

### Reconciliation vs. homepage / pricing claims

- **Homepage:** "500+ integrations", "100+ exchanges", "60+ wallets", "30+ chains" (per [[coinledger-homepage-2026-04-20]]).
- **Help-center reality:** 91 exchanges, 22 wallets, 51 chains, 5 on-chain protocols have dedicated articles.
- **Gap interpretation:** the homepage numbers are almost certainly including *any* integration reachable through a universal CSV template or wallet-address import, not just integrations with their own step-by-step help article. The help center is the conservative floor; the homepage is the inclusive ceiling.
- **Pricing page "1,000+ integrations":** not remotely reconcilable with dedicated help articles; likely a counted-any-way marketing number.

## By category (primary tag)

### Exchange import guides (113)

- [[coinledger-help-2883872-abra-file-import-guide-2026-04-20]] — Abra - File Import Guide
- [[coinledger-help-5563401-anchorusd-file-import-guide-2026-04-20]] — AnchorUSD - File Import Guide
- [[coinledger-help-3211479-btc-markets-file-import-guide-2026-04-20]] — BTC Markets - File Import Guide
- [[coinledger-help-6678831-bydfi-file-import-guide-2026-04-20]] — BYDFi - File Import Guide
- [[coinledger-help-5714606-bibox-api-import-guide-2026-04-20]] — Bibox - API Import Guide
- [[coinledger-help-5397368-bibox-file-import-guide-2026-04-20]] — Bibox - File Import Guide
- [[coinledger-help-5300306-bilaxy-file-import-guide-2026-04-20]] — Bilaxy - File Import Guide
- [[coinledger-help-6036926-binance-convert-history-file-import-guide-2026-04-20]] — Binance Convert History - File Import Guide
- [[coinledger-help-7174368-binance-p2p-trade-history-file-import-guide-2026-04-20]] — Binance P2P Trade History - File Import Guide
- [[coinledger-help-4936070-binance-us-api-import-guide-2026-04-20]] — Binance.US - API Import Guide
- _...and 103 more of the same pattern._

### Chain / on-chain import guides (54)

- [[coinledger-help-11955278-abstract-blockchain-import-guide-2026-04-20]] — Abstract - Blockchain Import Guide
- [[coinledger-help-9976376-akash-blockchain-import-guide-2026-04-20]] — Akash - Blockchain Import Guide
- [[coinledger-help-9715409-algorand-blockchain-import-guide-2026-04-20]] — Algorand - Blockchain Import Guide
- [[coinledger-help-10786820-apechain-blockchain-import-guide-2026-04-20]] — ApeChain - Blockchain Import Guide
- [[coinledger-help-6821127-arbitrum-blockchain-import-guide-2026-04-20]] — Arbitrum - Blockchain Import Guide
- [[coinledger-help-6472141-balancer-blockchain-import-guide-2026-04-20]] — Balancer - Blockchain Import Guide
- [[coinledger-help-8257248-base-blockchain-import-guide-2026-04-20]] — Base - Blockchain Import Guide
- [[coinledger-help-10715728-berachain-blockchain-import-guide-2026-04-20]] — Berachain - Blockchain Import Guide
- [[coinledger-help-6191928-binance-smart-chain-blockchain-import-guide-2026-04-20]] — Binance Smart Chain - Blockchain Import Guide
- [[coinledger-help-6341836-bitcoin-blockchain-import-guide-2026-04-20]] — Bitcoin - Blockchain Import Guide
- _...and 44 more of the same pattern._

### Wallet import guides (23)

- [[coinledger-help-10552877-arculus-wallet-blockchain-import-guide-2026-04-20]] — Arculus Wallet - Blockchain Import Guide
- [[coinledger-help-11635807-argent-wallet-blockchain-import-guide-2026-04-20]] — Argent Wallet - Blockchain Import Guide
- [[coinledger-help-6184950-atomic-wallet-blockchain-import-guide-2026-04-20]] — Atomic Wallet - Blockchain Import Guide
- [[coinledger-help-6185086-coinbase-wallet-blockchain-import-guide-2026-04-20]] — Coinbase Wallet - Blockchain Import Guide
- [[coinledger-help-10602298-electrum-wallet-blockchain-import-guide-2026-04-20]] — Electrum Wallet - Blockchain Import Guide
- [[coinledger-help-10573929-guarda-wallet-blockchain-import-guide-2026-04-20]] — Guarda Wallet - Blockchain Import Guide
- [[coinledger-help-10573916-leather-wallet-blockchain-import-guide-2026-04-20]] — Leather Wallet - Blockchain Import Guide
- [[coinledger-help-6191248-ledger-wallet-blockchain-import-guide-2026-04-20]] — Ledger Wallet - Blockchain Import Guide
- [[coinledger-help-11463666-ledger-wallet-file-import-guide-2026-04-20]] — Ledger Wallet - File Import Guide
- [[coinledger-help-6110244-metamask-blockchain-import-guide-2026-04-20]] — MetaMask - Blockchain Import Guide
- _...and 13 more of the same pattern._

### Manual / universal CSV import (3)

- [[coinledger-help-2584884-how-can-i-manually-import-transactions-into-coinledger-2026-04-20]] — How can I manually import transactions into CoinLedger? **[H]**
- [[coinledger-help-6173382-import-transactions-from-a-partially-supported-exchange-with-the-universal-import-template-csv-file-2026-04-20]] — Import transactions from a partially supported exchange with the Universal Import Template (CSV file) **[H]**
- [[coinledger-help-6028758-universal-manual-import-template-guide-2026-04-20]] — Universal Manual Import Template Guide **[H]**

### Import troubleshooting (11)

- [[coinledger-help-2559346-help-my-import-is-failing-what-should-i-do-2026-04-20]] — Help! My import is failing. What should I do? **[H]**
- [[coinledger-help-4357024-how-can-i-solve-a-historical-price-warning-2026-04-20]] — How can I solve a Historical Price Warning? **[H]**
- [[coinledger-help-2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do-2026-04-20]] — My capital gains/losses don't look correct. What should I do? **[H]**
- [[coinledger-help-4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting-2026-04-20]] — Troubleshooting Manual CSV File Import Failures (due to incorrect formatting) **[H]**
- [[coinledger-help-6100964-troubleshooting-turbotax-imports-2026-04-20]] — Troubleshooting TurboTax Imports **[H]**
- [[coinledger-help-10416095-what-should-i-do-if-i-have-duplicate-transactions-on-my-account-2026-04-20]] — What should I do if I have duplicate transactions on my account? **[H]**
- [[coinledger-help-10552450-why-am-i-seeing-a-gain-or-loss-on-a-non-taxable-transaction-2026-04-20]] — Why am I seeing a gain or loss on a non-taxable transaction? **[H]**
- [[coinledger-help-10548865-why-are-my-asset-balances-on-the-portfolio-tracker-incorrect-2026-04-20]] — Why are my asset balances on the Portfolio Tracker incorrect? **[H]**
- [[coinledger-help-10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger-2026-04-20]] — Why are the timestamps on my transactions different when I import them into CoinLedger? **[H]**
- [[coinledger-help-2749028-why-is-my-8949-only-one-line-2026-04-20]] — Why is my 8949 only one line? **[H]**
- [[coinledger-help-11088743-why-is-one-trade-sometimes-broken-up-into-multiple-entries-on-the-irs-form-8949-2026-04-20]] — Why is one trade sometimes broken up into multiple entries on the IRS Form 8949? **[H]**

### Cost basis / missing basis / Rev. Proc. 2024-28 (20)

- [[coinledger-help-10346496-2025-cost-basis-reallocation-changes-why-does-my-cost-basis-look-different-2026-04-20]] — 2025 Cost Basis Reallocation Changes — Why Does My Cost Basis Look Different? **[H]**
- [[coinledger-help-10657568-can-i-edit-the-cost-basis-of-a-transaction-2026-04-20]] — Can I edit the cost basis of a transaction? **[H]**
- [[coinledger-help-2865416-can-i-file-my-taxes-with-an-unresolved-missing-cost-basis-2026-04-20]] — Can I file my taxes with an unresolved Missing Cost Basis? **[H]**
- [[coinledger-help-12609869-can-i-ignore-a-missing-cost-basis-warning-2026-04-20]] — Can I ignore a Missing Cost Basis Warning? **[H]**
- [[coinledger-help-10080173-can-i-manually-enter-an-asset-s-cost-basis-aka-a-manual-position-2026-04-20]] — Can I manually enter an asset's cost basis (aka a 'Manual Position')? **[H]**
- [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]] — Common Causes of Missing Cost Basis Warnings **[H]**
- [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]] — Fixing Missing Cost Basis Issues After Transitioning to Per-Wallet Cost Basis Tracking **[H]**
- [[coinledger-help-10302709-how-are-cost-basis-numbers-in-the-portfolio-tracker-calculated-2026-04-20]] — How are cost basis numbers in the Portfolio Tracker calculated? **[H]**
- [[coinledger-help-10339065-how-can-i-download-a-snapshot-of-my-2025-cost-basis-reallocation-rev-proc-2024-28-2026-04-20]] — How can I download a snapshot of my 2025 cost basis reallocation (Rev. Proc. 2024-28)? **[H]**
- [[coinledger-help-10314185-how-do-i-change-my-cost-basis-reallocation-method-irs-rev-proc-2024-28-2026-04-20]] — How do I change my cost basis reallocation method (IRS Rev. Proc 2024-28)? **[H]**
- _...and 10 more of the same pattern._

### Reconciliation / classification workflow (5)

- [[coinledger-help-6110498-how-to-classify-uncategorized-transactions-2026-04-20]] — How To Classify Uncategorized Transactions **[H]**
- [[coinledger-help-8345587-how-can-i-import-bridge-transactions-2026-04-20]] — How can I import bridge transactions? **[H]**
- [[coinledger-help-11426960-how-can-i-reclassify-transactions-in-coinledger-2026-04-20]] — How can I reclassify transactions in CoinLedger? **[H]**
- [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]] — What is the Potential Bridges, Trades and Transfers tab? **[H]**
- [[coinledger-help-5915504-when-do-i-need-to-manually-classify-or-fix-my-crypto-transactions-2026-04-20]] — When do I need to manually classify or "fix" my crypto transactions? **[H]**

### Tax reports / 8949 / downloads (24)

- [[coinledger-help-13453951-how-do-i-generate-my-form-8949-2025-and-later-2026-04-20]] — How do I generate my Form 8949? (2025 and later) **[H]**
- [[coinledger-help-3578432-returning-users-how-to-pickup-where-you-left-off-and-generate-this-year-s-tax-reports-2026-04-20]] — Returning Users - How To Pickup Where You Left Off And Generate This Year's Tax Reports **[H]**
- [[coinledger-help-10548303-what-is-the-asset-balance-report-2026-04-20]] — What is the Asset Balance Report? **[H]**
- [[coinledger-help-6156314-what-s-the-end-of-year-eoy-positions-report-2026-04-20]] — What's the End of Year (EOY) Positions report? **[H]**
- [[coinledger-help-6026024-which-tax-reports-should-i-take-to-my-tax-professional-usa-2026-04-20]] — Which tax reports should I take to my tax professional? (USA) **[H]**
- [[coinledger-help-8619834-can-you-help-me-print-out-my-tax-forms-2026-04-20]] — Can you help me print out my tax forms?
- [[coinledger-help-11509317-how-can-i-claim-my-losses-from-crypto-on-my-taxes-2026-04-20]] — How can I claim my losses from crypto on my taxes?
- [[coinledger-help-10298549-how-can-i-freeze-a-tax-report-on-my-account-2026-04-20]] — How can I freeze a tax report on my account?
- [[coinledger-help-9011544-how-can-i-purchase-my-tax-report-2026-04-20]] — How can I purchase my tax report?
- [[coinledger-help-2896190-how-do-i-amend-previous-years-tax-returns-2026-04-20]] — How do I amend previous years tax returns?
- _...and 14 more of the same pattern._

### TurboTax integration (3)

- [[coinledger-help-6020888-can-i-import-my-exchanges-directly-into-turbotax-without-using-crypto-tax-software-2026-04-20]] — Can I import my exchanges directly into TurboTax without using crypto tax software?
- [[coinledger-help-2839171-delete-cryptocurrency-trades-turbotax-online-2026-04-20]] — Delete Cryptocurrency Trades - TurboTax Online
- [[coinledger-help-3733271-enter-crypto-income-turbotax-online-2026-04-20]] — Enter Crypto Income - TurboTax Online

### H&R Block integration (1)

- [[coinledger-help-6220960-how-do-i-import-my-transactions-into-h-r-block-2026-04-20]] — How do I import my transactions into H&R Block?

### TaxSlayer integration (1)

- [[coinledger-help-6210473-how-do-i-import-my-crypto-trades-and-transactions-into-taxslayer-2026-04-20]] — How do I import my crypto trades and transactions into TaxSlayer?

### Pricing / billing / refunds (4)

- [[coinledger-help-5915548-pricing-your-questions-answered-2026-04-20]] — Pricing: Your Questions Answered **[H]**
- [[coinledger-help-7039157-what-is-the-refund-policy-2026-04-20]] — What is the refund policy? **[H]**
- [[coinledger-help-8129375-how-can-i-download-a-receipt-for-my-coinledger-purchase-2026-04-20]] — How can I download a receipt for my CoinLedger purchase?
- [[coinledger-help-11159101-what-payment-methods-does-coinledger-accept-2026-04-20]] — What payment methods does CoinLedger accept?

### Account / login / security (11)

- [[coinledger-help-9251645-how-to-contact-coinledger-support-2026-04-20]] — How to contact CoinLedger Support **[H]**
- [[coinledger-help-10579522-is-it-safe-to-import-my-transactions-into-coinledger-via-api-2026-04-20]] — Is it safe to import my transactions into CoinLedger via API? **[H]**
- [[coinledger-help-12904021-notice-of-security-incident-involving-analytics-vendor-2026-04-20]] — Notice of security incident involving analytics vendor **[H]**
- [[coinledger-help-6161888-security-and-privacy-your-questions-answered-2026-04-20]] — Security and Privacy-Your Questions Answered **[H]**
- [[coinledger-help-7198665-how-to-set-up-single-sign-on-sso-for-your-coinledger-account-2026-04-20]] — How to set up Single Sign-On (SSO) for your CoinLedger account
- [[coinledger-help-10507971-help-i-m-not-receiving-emails-from-coinledger-what-can-i-do-2026-04-20]] — Help! I'm not receiving emails from CoinLedger. What can I do?
- [[coinledger-help-5915649-how-can-i-change-the-country-currency-and-time-zone-on-my-account-2026-04-20]] — How can I change the country, currency, and time zone on my account?
- [[coinledger-help-5937794-how-can-i-manage-or-delete-my-account-data-2026-04-20]] — How can I manage or delete my account data?
- [[coinledger-help-5968702-how-can-i-refer-my-friends-to-coinledger-and-earn-commission-affiliate-program-2026-04-20]] — How can I refer my friends to CoinLedger and earn commission? (Affiliate Program)
- [[coinledger-help-5915573-how-to-update-your-coinledger-account-settings-2026-04-20]] — How to update your CoinLedger account settings
- [[coinledger-help-10536084-i-created-my-coinledger-account-with-the-wrong-email-address-what-can-i-do-2026-04-20]] — I created my CoinLedger account with the wrong email address. What can I do?

### Portfolio tracker (3)

- [[coinledger-help-8681820-how-does-the-portfolio-tracker-work-2026-04-20]] — How does the Portfolio Tracker work? **[H]**
- [[coinledger-help-12109286-how-can-i-hide-dust-balances-from-my-portfolio-2026-04-20]] — How can I hide dust balances from my portfolio?
- [[coinledger-help-11145949-what-is-my-staked-balance-2026-04-20]] — What is my Staked Balance?

### Pro services (Done-For-You / Expert Review) (3)

- [[coinledger-help-8135954-what-can-i-expect-from-my-expert-review-2026-04-20]] — What can I expect from my Expert Review? **[H]**
- [[coinledger-help-9483228-what-is-coinledger-done-for-you-2026-04-20]] — What is CoinLedger Done For You? **[H]**
- [[coinledger-help-5915605-i-need-a-tax-professional-2026-04-20]] — I need a tax professional!

### DeFi / DEX (3)

- [[coinledger-help-6097108-what-blockchains-dapps-defi-protocols-do-you-integrate-with-2026-04-20]] — What blockchains / dApps / DeFi protocols do you integrate with? **[H]**
- [[coinledger-help-11525113-how-can-i-import-my-jupiter-transactions-into-coinledger-2026-04-20]] — How can I import my Jupiter transactions into CoinLedger?
- [[coinledger-help-10670385-how-can-i-import-transactions-from-a-decentralized-exchange-like-jupiter-or-uniswap-2026-04-20]] — How can I import transactions from a decentralized exchange like Jupiter or Uniswap?

### Staking (1)

- [[coinledger-help-11145964-does-coinledger-support-staking-2026-04-20]] — Does CoinLedger support staking?

### Jurisdiction: UK (1)

- [[coinledger-help-10064078-uk-crypto-taxes-2026-04-20]] — UK Crypto Taxes

### Jurisdiction: Australia (1)

- [[coinledger-help-3140420-australia-crypto-taxes-2026-04-20]] — Australia Crypto Taxes

### Jurisdiction: Canada (1)

- [[coinledger-help-8632780-canada-crypto-taxes-2026-04-20]] — Canada Crypto Taxes

### Jurisdiction: New Zealand (1)

- [[coinledger-help-8632806-new-zealand-crypto-taxes-2026-04-20]] — New Zealand Crypto Taxes

### General FAQ / feature questions (37)

- [[coinledger-help-2654206-coinledger-terminology-2026-04-20]] — CoinLedger Terminology **[H]**
- [[coinledger-help-6270051-common-api-import-limitations-2026-04-20]] — Common API Import Limitations **[H]**
- [[coinledger-help-9505113-how-can-i-import-my-margin-transactions-into-coinledger-2026-04-20]] — How can I import my margin transactions into CoinLedger? **[H]**
- [[coinledger-help-6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange-2026-04-20]] — How to edit a deposit into a buy to fix incomplete data exported by a crypto exchange **[H]**
- [[coinledger-help-9174597-i-m-a-first-time-coinledger-user-how-do-i-get-started-2026-04-20]] — I'm a first time CoinLedger user - how do I get started? **[H]**
- [[coinledger-help-2952368-import-your-ico-s-2026-04-20]] — Import your ICO's **[H]**
- [[coinledger-help-2535251-what-exchanges-does-coinledger-support-2026-04-20]] — What exchanges does CoinLedger support? **[H]**
- [[coinledger-help-8546372-what-transaction-types-does-coinledger-support-2026-04-20]] — What transaction types does CoinLedger support? **[H]**
- [[coinledger-help-3130354-which-report-calculation-methods-does-coinledger-support-2026-04-20]] — Which report calculation methods does CoinLedger support? **[H]**
- [[coinledger-help-6878347-coinstats-and-coinledger-partnership-details-2026-04-20]] — CoinStats and CoinLedger Partnership Details
- _...and 27 more of the same pattern._

## Most complex / heavily-documented support themes

Where CoinLedger support is clearly doing the most work — measured by article density, presence of multiple troubleshooting escalations, and high-signal flagging. These are the places users actually get stuck.

### 1. Missing Cost Basis (MCB) warnings

The single heaviest support theme. CoinLedger has at least **nine dedicated help articles** explaining why users see MCB warnings and how to resolve them. Patterns: missing exchange data, missing years, duplicates, uncategorized on-chain interactions, Coinbase↔Coinbase Pro splits, self-custody wallet buys, third-party fiat-onramp providers (MoonPay/Banxa/Transak), Binance.US one-sided buys, bridge transactions, and post-reallocation "first inflow" cases.

- [[coinledger-help-2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it-2026-04-20]] **[H]** — the canonical root-cause explainer
- [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]] **[H]** — 11-item cause taxonomy
- [[coinledger-help-2599667-rounding-errors-missing-cost-basis-warning-2026-04-20]] **[H]** — sub-type: dust/rounding MCB
- [[coinledger-help-6811823-how-to-fix-first-inflow-missing-basis-warnings-2026-04-20]] **[H]** — sub-type: first-inflow after reallocation
- [[coinledger-help-6105647-how-to-classify-nft-mint-transactions-and-remove-missing-cost-basis-warnings-2026-04-20]] **[H]** — NFT mint MCB fix
- [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]] **[H]** — post-Rev-Proc-2024-28 reallocation cases
- [[coinledger-help-12609869-can-i-ignore-a-missing-cost-basis-warning-2026-04-20]] **[H]** — "can I ship anyway?"
- [[coinledger-help-2865416-can-i-file-my-taxes-with-an-unresolved-missing-cost-basis-2026-04-20]] **[H]** — same question, older article

### 2. Rev. Proc. 2024-28 per-wallet cost-basis migration

The 2025–26 editorial push. CoinLedger built a whole workflow (reallocation breakdown report, basis reallocation transactions, cost-basis snapshot download) and wrote dedicated articles for each piece.

- [[coinledger-help-10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28-2026-04-20]] **[H]** — the marquee article (David Kemmerer, co-founder, authored)
- [[coinledger-help-10314185-how-do-i-change-my-cost-basis-reallocation-method-irs-rev-proc-2024-28-2026-04-20]] **[H]** — changing method (FIFO/LIFO/HIFO etc.)
- [[coinledger-help-10339065-how-can-i-download-a-snapshot-of-my-2025-cost-basis-reallocation-rev-proc-2024-28-2026-04-20]] **[H]** — snapshot download
- [[coinledger-help-10346496-2025-cost-basis-reallocation-changes-why-does-my-cost-basis-look-different-2026-04-20]] **[H]** — "my numbers changed" defense article
- [[coinledger-help-11962455-what-are-basis-reallocation-transactions-2026-04-20]] **[H]** — new synthetic transaction type
- [[coinledger-help-12771568-what-is-the-reallocation-breakdown-report-2026-04-20]] **[H]** — new report artifact
- [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]] **[H]** — cleanup path after migration

### 3. Form 8949 correctness and reconciliation math

Users distrust their generated 8949. Multiple articles exist to explain why it "looks wrong":

- [[coinledger-help-2642037-why-are-my-net-cost-basis-and-net-proceeds-on-the-form-8949-so-high-2026-04-20]] **[H]** — "my gross numbers are massive"
- [[coinledger-help-2749028-why-is-my-8949-only-one-line-2026-04-20]] **[H]** — "my 8949 is one line"
- [[coinledger-help-11088743-why-is-one-trade-sometimes-broken-up-into-multiple-entries-on-the-irs-form-8949-2026-04-20]] **[H]** — lot-splitting confusion
- [[coinledger-help-2654100-my-capital-gains-losses-don-t-look-correct-what-should-i-do-2026-04-20]] **[H]** — the catch-all
- [[coinledger-help-10552450-why-am-i-seeing-a-gain-or-loss-on-a-non-taxable-transaction-2026-04-20]] **[H]** — classification-driven surprise gains
- [[coinledger-help-13453951-how-do-i-generate-my-form-8949-2025-and-later-2026-04-20]] **[H]** — post-per-wallet 8949 generation

### 4. Transaction classification / reclassification / potential bridges

The reconciliation UI has its own mini-manual: uncategorized transactions, potential bridges/trades/transfers, bridge merging, deposit→buy editing, token migrations.

- [[coinledger-help-6110498-how-to-classify-uncategorized-transactions-2026-04-20]] **[H]**
- [[coinledger-help-11426960-how-can-i-reclassify-transactions-in-coinledger-2026-04-20]] **[H]**
- [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]] **[H]** — the "PBT" tab
- [[coinledger-help-8345587-how-can-i-import-bridge-transactions-2026-04-20]] **[H]**
- [[coinledger-help-6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange-2026-04-20]] **[H]**
- [[coinledger-help-10271029-how-can-i-represent-a-token-migration-or-swap-in-coinledger-2026-04-20]]

### 5. Import failure triage

General "my import is failing" escalation path plus common-API-limitations meta-doc, duplicate-transaction cleanup, TurboTax-export troubleshooting, CSV-formatting failures, bankruptcy exchange imports, and timestamps/timezone issues.

- [[coinledger-help-2559346-help-my-import-is-failing-what-should-i-do-2026-04-20]] **[H]**
- [[coinledger-help-6270051-common-api-import-limitations-2026-04-20]] **[H]**
- [[coinledger-help-4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting-2026-04-20]] **[H]**
- [[coinledger-help-10416095-what-should-i-do-if-i-have-duplicate-transactions-on-my-account-2026-04-20]] **[H]**
- [[coinledger-help-9707894-how-can-i-import-data-from-a-bankrupt-or-defunct-crypto-exchange-2026-04-20]]
- [[coinledger-help-6100964-troubleshooting-turbotax-imports-2026-04-20]] **[H]**
- [[coinledger-help-10327917-why-are-the-timestamps-on-my-transactions-different-when-i-import-them-into-coinledger-2026-04-20]] **[H]**

## Jurisdiction-specific help articles

Only **four** jurisdictions get dedicated help-center articles, all under the same "thin stub that redirects to the blog/guide" pattern — confirm the tax-settings country/currency choice, then link out to the editorial guide:

- [[coinledger-help-10064078-uk-crypto-taxes-2026-04-20]] — UK
- [[coinledger-help-3140420-australia-crypto-taxes-2026-04-20]] — Australia
- [[coinledger-help-8632780-canada-crypto-taxes-2026-04-20]] — Canada
- [[coinledger-help-8632806-new-zealand-crypto-taxes-2026-04-20]] — New Zealand

Notably absent as help-center pages: **US (implicit default), Germany (has special product logic per homepage), India, Ireland, Portugal, Singapore, Brazil, South Africa, Japan** — these jurisdictions are covered on the blog and/or the guides, but the help center assumes anything jurisdiction-shaped is a tax-settings toggle, not a documentation topic.

## Product features documented

### Portfolio tracker

- [[coinledger-help-8681820-how-does-the-portfolio-tracker-work-2026-04-20]] **[H]** — the canonical explainer
- [[coinledger-help-10302709-how-are-cost-basis-numbers-in-the-portfolio-tracker-calculated-2026-04-20]] **[H]**
- [[coinledger-help-10548865-why-are-my-asset-balances-on-the-portfolio-tracker-incorrect-2026-04-20]] **[H]**
- [[coinledger-help-12109286-how-can-i-hide-dust-balances-from-my-portfolio-2026-04-20]]
- [[coinledger-help-11145949-what-is-my-staked-balance-2026-04-20]]

### Tax reports and report types

- [[coinledger-help-13453951-how-do-i-generate-my-form-8949-2025-and-later-2026-04-20]] **[H]** — the flagship report
- [[coinledger-help-6156314-what-s-the-end-of-year-eoy-positions-report-2026-04-20]] **[H]** — EOY Positions
- [[coinledger-help-10548303-what-is-the-asset-balance-report-2026-04-20]] **[H]** — Asset Balance
- [[coinledger-help-12771568-what-is-the-reallocation-breakdown-report-2026-04-20]] **[H]** — Reallocation Breakdown (new 2025)
- [[coinledger-help-6026024-which-tax-reports-should-i-take-to-my-tax-professional-usa-2026-04-20]] **[H]** — the "which report for which purpose" doc
- [[coinledger-help-5915673-how-do-i-download-my-reports-2026-04-20]]
- [[coinledger-help-10298549-how-can-i-freeze-a-tax-report-on-my-account-2026-04-20]]
- [[coinledger-help-3578432-returning-users-how-to-pickup-where-you-left-off-and-generate-this-year-s-tax-reports-2026-04-20]] **[H]**

### Filing-software exports

- TurboTax: [[coinledger-help-2671099-upload-your-tax-report-turbotax-online-2026-04-20]], [[coinledger-help-2657181-upload-your-tax-report-turbotax-desktop-cd-version-2026-04-20]], [[coinledger-help-3733271-enter-crypto-income-turbotax-online-2026-04-20]], [[coinledger-help-2839171-delete-cryptocurrency-trades-turbotax-online-2026-04-20]], [[coinledger-help-6020888-can-i-import-my-exchanges-directly-into-turbotax-without-using-crypto-tax-software-2026-04-20]], [[coinledger-help-6100964-troubleshooting-turbotax-imports-2026-04-20]] **[H]**
- TaxAct: [[coinledger-help-5958351-upload-your-tax-report-taxact-2026-04-20]]
- H&R Block: [[coinledger-help-6220960-how-do-i-import-my-transactions-into-h-r-block-2026-04-20]]
- TaxSlayer: [[coinledger-help-6210473-how-do-i-import-my-crypto-trades-and-transactions-into-taxslayer-2026-04-20]]

### Pro services

- [[coinledger-help-9483228-what-is-coinledger-done-for-you-2026-04-20]] **[H]** — Done-For-You service overview
- [[coinledger-help-8135954-what-can-i-expect-from-my-expert-review-2026-04-20]] **[H]** — Expert Review tier
- [[coinledger-help-5915605-i-need-a-tax-professional-2026-04-20]] — referral funnel

## Content-hygiene patterns

- **Authorship is tightly centralized.** Benjamin Yoder (Support) writes the majority of import/troubleshooting articles. David Kemmerer (co-founder) authors the marquee infra pieces — Rev. Proc. 2024-28, per-wallet migration, the exchange-support list. Lucas Wyland authors the pricing FAQ, chains/dApps integration list, and referral/affiliate content.
- **"Updated X ago" rather than real dates.** Every article shows a relative-time "Updated over a year ago / 4 months ago / 10 months ago" instead of a hard date, making staleness hard to assess without loading each article. The Rev. Proc. 2024-28 cluster was updated recently (4 months ago); most CEX import guides are a year+ old.
- **Legacy-exchange cruft is still published.** [[coinledger-help-2535269-coinbase-pro-file-import-guide-2026-04-20]] is still live even though Coinbase Pro shut down in Nov 2022. Bittrex (shut down in 2023), Poloniex (US withdrawal), Bilaxy/Bibox/Graviex (largely-defunct tier-3 CEXs), Terra/Luna, Voyager, Shapeshift (discontinued CEX mode), AnchorUSD, Mercatox, and Mandala all still have dedicated pages. These are retained because historical-tax users still need to import legacy CSVs, but nothing in the help center flags them as legacy.
- **Two layers of URLs.** Articles freely cross-link to both `help.coinledger.io` (the canonical Intercom instance) and `help.cryptotrader.tax` (the pre-rebrand Intercom). Inbound links from the new URL pointing to the old brand are everywhere. This is technical debt from the 2022 rename.
- **Screenshot-heavy even for small articles.** Every import guide is 5-8 screenshots plus minimal prose. The text body is short; the UX value is entirely in the images. For an LLM index this means the raw markdown undersells the article content.
- **Duplicate or near-duplicate articles coexist.** KuCoin has three (`kucoin-file-import-guide`, `kucoin-alternate-file-import-guide`, `kucoin-api-import-guide`). Ledger has two (file-import + blockchain-import). Two separate articles ask "Can I file with an unresolved MCB?" (12609869 and 2865416) with different authors. Evidence of copy-drift rather than active curation.
- **Intercom-native artifacts.** "Did this answer your question? 😞😐😃" footer on every article. Intercom avatar URLs in every page. These don't affect readers but do signal the help center is hosted stock on Intercom rather than custom CMS — cheaper to run, harder to SEO.

## Gaps / notable absences

Product surfaces where you'd expect more help coverage than exists:

- **DeFi protocol depth.** Only Uniswap, SushiSwap, Balancer, Jupiter (via DEX-import FAQ), and a generic "DEX import" article. Nothing on Curve, Aave, Compound, GMX, dYdX, Raydium, Orca, Pump.fun, Hyperliquid vaults — all heavy-volume user activity.
- **NFT coverage is almost zero.** One OpenSea article and one "classify NFT mint" article. No Blur, Magic Eden, Tensor, Rarible, NFT royalties, airdrops, mint-vs-purchase distinction.
- **Staking depth is shockingly thin.** Literally one "does CoinLedger support staking" article and one "what is my staked balance" article. No chain-specific staking behavior (ETH LSTs, Solana validators, Cosmos re-staking, Lido/Rocket Pool treatment). The blog compensates but the help center defers entirely.
- **No FBAR / foreign-account help.** Given US customers heavily use non-US CEXs, the absence of any FBAR/FATCA-flavored help article is conspicuous.
- **No "tax-loss harvesting in app" workflow article.** There's a definitional TLH article but no product workflow doc even though TLH is a marketed feature.
- **No 1099-DA help article series.** The blog has 18 posts on 1099-DA. The help center has one definitional article ([[coinledger-help-6161985-what-is-form-1099-da-2026-04-20]]) and nothing about what to do when your 1099-DA disagrees with CoinLedger's 8949. Given the editorial push elsewhere, this is a real gap.
- **Jurisdiction support is severely under-documented.** Four country articles, each ~100 words. The "Germany has special logic" claim from the homepage is not explained in help at all.
- **Accountant / B2B flow absent.** No pro-plan onboarding, no team-member permissioning, no client-handoff workflow beyond "I need a tax professional" referral.
- **API integration limitations doc is one-size-fits-all.** The common-API-limitations article lumps all exchanges together; per-exchange limitation pages (e.g., "Binance.US one-sided buy issue") are scattered and inconsistent.
- **Wallet-tax-report feature set** — no article on importing hardware wallets directly (Trezor/Ledger file imports exist; no ledger-live-companion flow).

## Standouts (worth Lucas reading for product insight)

- [[coinledger-help-10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28-2026-04-20]] — David Kemmerer's marquee article. Clear, worked examples of universal vs. per-wallet accounting; the reference piece for how CoinLedger is positioning itself on the 2024-28 shift.
- [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]] — the 11-item MCB-root-cause taxonomy. A direct read of where users get stuck in production.
- [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]] — explains the "PBT" UI tab, which is the main reconciliation surface for on-chain activity. Reveals how the product models heuristic bridge/trade detection.
- [[coinledger-help-6097108-what-blockchains-dapps-defi-protocols-do-you-integrate-with-2026-04-20]] — Lucas's own article; the authoritative list of CoinLedger chain coverage. Canonical reconciliation target for integration claims.
- [[coinledger-help-2535251-what-exchanges-does-coinledger-support-2026-04-20]] — the CEX counterpart, by David Kemmerer. Useful for crosschecking against the homepage's "100+ exchanges".
- [[coinledger-help-9483228-what-is-coinledger-done-for-you-2026-04-20]] — full Done-For-You service flow. Only place the white-glove product is documented in detail.
- [[coinledger-help-6145354-how-is-cost-basis-calculated-2026-04-20]] — fundamentals article; useful cross-ref for cost-basis explainers elsewhere.
- [[coinledger-help-3130354-which-report-calculation-methods-does-coinledger-support-2026-04-20]] — FIFO/LIFO/HIFO/Spec ID availability by jurisdiction. The matrix of "what methods work where".
- [[coinledger-help-11088743-why-is-one-trade-sometimes-broken-up-into-multiple-entries-on-the-irs-form-8949-2026-04-20]] — lot-splitting explanation. Illuminates how the disposal engine actually works.
- [[coinledger-help-6708304-how-to-edit-a-deposit-into-a-buy-to-fix-incomplete-data-exported-by-a-crypto-exchange-2026-04-20]] — exposes the "we can't always trust exchange CSVs and here's the escape hatch" pattern.

