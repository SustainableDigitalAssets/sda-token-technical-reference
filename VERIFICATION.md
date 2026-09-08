# Verification guide

1. Open the [Solscan token page](https://solscan.io/token/SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b) and confirm the mint exactly matches `SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b`.
2. Confirm the token uses the Token-2022 program and has six decimals.
3. Confirm maximum supply is `100,000,000 SDA`.
4. Confirm mint authority and freeze authority are revoked.
5. Compare the on-chain values with [`token.json`](token.json), the [circulating supply API](https://sdafintech.com/api/supply/circulating), and the [total supply API](https://sdafintech.com/api/supply/total).
6. Confirm the [notified white paper](https://sdafintech.com/legal/mica/whitepaper/SDA-Token-MiCA-Whitepaper-v1.3-2026_07_16.xhtml) identifies DTI `ZHSMZL7F9`, Sustainable Digital Assets Inc., FIN-FSA, and the 29-EEA-state notification scope. A [PDF version](https://sdafintech.com/legal/mica/whitepaper/SDA-Token-MiCA-Whitepaper-v1.3-2026_07_16.pdf) is also available.
7. Record the check date and any discrepancy without changing the canonical values until the discrepancy is resolved.

Additional references: [CoinGecko](https://www.coingecko.com/en/coins/sda-token), [Coinstore SDAUSDT](https://www.coinstore.com/spot/SDAUSDT), and [BTCC SDAUSDT](https://www.btcc.com/en-US/spot/SDAUSDT).
