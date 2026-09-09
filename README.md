# SDA Token Technical Reference

SDA Token (SDA) is a utility token on Solana mainnet issued by Sustainable Digital Assets Inc. It uses the Solana SPL Token-2022 program. SDA is not a security token and is supervised under MiCA as a Title II crypto-asset other than an ART or EMT.

## Canonical identity

- Mint: `SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b`
- Decimals: `6`
- Maximum supply: `100,000,000 SDA` (fixed)
- Mint authority: revoked
- Freeze authority: revoked
- Issuer LEI: `89450058XEES8WCSCQ03`
- Registered DTI: `ZHSMZL7F9` (ISO 24165)

Current utility comprises platform access, project data and analytics, non-financial governance participation, and priority feature access. The platform's ESG oracle publishes verifiable CO2-avoided data on-chain.

## Repository map

- [`README.md`](README.md): overview, canonical identity, references and repository map.
- [`token.json`](token.json): machine-readable token record.
- [`REGULATORY.md`](REGULATORY.md): regulatory identity and primary evidence.
- [`VERIFICATION.md`](VERIFICATION.md): independent verification steps.
- [`API.md`](API.md): supply API response and client guidance.
- [`CHANGELOG.md`](CHANGELOG.md): dated public changes and separated historical internal records.
- [`VERSIONING.md`](VERSIONING.md): versioning, deprecation and correction policy.
- [`llms.txt`](llms.txt): concise content index for language-model retrieval.
- [`catalog.json`](catalog.json): machine-readable catalogue of artefacts across the three public repositories.

## Companion repositories

- [SDA Energy Data](https://github.com/SustainableDigitalAssets/sda-energy-data) provides European grid emission factors, ENTSO-E mappings and a glossary.
- [SDA Integration Cookbook](https://github.com/SustainableDigitalAssets/sda-integration-cookbook) provides read-only TypeScript and Python examples for supply, mint information and balances.

## References

The current white paper is version 1.3, notified via FIN-FSA for 29 EEA states and published on 2026-07-16 in inline XBRL.

- [Machine-readable token record](token.json)
- [Regulatory identity](REGULATORY.md)
- [Verification guide](VERIFICATION.md)
- [Supply API reference](API.md)
- [Canonical website](https://sdafintech.com)
- [White paper page](https://sdafintech.com/documentation/whitepaper)
- [White paper in inline XBRL](https://sdafintech.com/legal/mica/whitepaper/SDA-Token-MiCA-Whitepaper-v1.3-2026_07_16.xhtml)
- [White paper in PDF](https://sdafintech.com/legal/mica/whitepaper/SDA-Token-MiCA-Whitepaper-v1.3-2026_07_16.pdf)
- [Litepaper](https://sdafintech.com/documentation/litepaper)
- [Solscan](https://solscan.io/token/SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b)
- [CoinGecko](https://www.coingecko.com/en/coins/sda-token)
- [Circulating supply API](https://sdafintech.com/api/supply/circulating)
- [Total supply API](https://sdafintech.com/api/supply/total)
