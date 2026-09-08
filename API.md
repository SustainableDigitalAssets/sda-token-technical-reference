# Supply API reference

| Purpose | GET endpoint | Verified response on 2026-09-08 |
|---|---|---|
| Circulating supply | `https://sdafintech.com/api/supply/circulating` | `{"result":"4028420.000000"}` |
| Total supply | `https://sdafintech.com/api/supply/total` | `{"result":"100000000.000000"}` |

Both observed responses are JSON objects with a `result` string containing the SDA amount with six fractional digits. No fixed update schedule or availability SLA is published. Clients should observe response cache headers, handle non-2xx responses and invalid JSON, retain the last validated response according to their own policy, and verify the canonical mint independently on [Solscan](https://solscan.io/token/SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b).
