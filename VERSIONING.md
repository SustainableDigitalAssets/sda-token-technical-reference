# Versioning policy

This repository separates the version of a file's structure from the date on which a fact was observed or a document was published. A repository commit identifies an exact revision, but it does not replace verification against primary sources.

## Machine-readable files

Machine-readable contracts and schemas use semantic versioning in the form `MAJOR.MINOR.PATCH`.

- `MAJOR` changes indicate an incompatible field removal, rename, type change or semantic change.
- `MINOR` changes add backward-compatible fields or enumerated values.
- `PATCH` changes correct data without changing the schema, or clarify machine-readable descriptions.

`token.json` declares its JSON contract through the top-level `schemaVersion` field, currently `1.1.0`. The field versions the JSON contract, not the token, network, white paper or underlying facts. `catalog.json` declares its catalogue schema through `catalogVersion` and follows the same semantic-versioning rules.

## Documents and facts

Markdown documents use calendar-dated changelog entries in `YYYY-MM-DD` form. An entry records the publication or verified change date when known. If a date cannot be corroborated, the changelog states that it is unknown rather than inferring one.

Document versions, including MiCA white paper versions, retain the version assigned by their publisher. A document version is not a version of the token or this repository.

Facts such as the mint, token program, decimal precision, authorities, DTI, LEI and regulatory classification are recorded as observed values. Their history is maintained in `CHANGELOG.md`; they are not assigned artificial semantic versions.

## Deprecations and corrections

Deprecated fields remain available for at least one minor schema version when doing so does not preserve an unsafe or materially incorrect value. They must be marked as deprecated, identify the replacement and state the intended removal version or date.

Corrections are never silent. Every correction must be described in `CHANGELOG.md` with its date, affected artefact and source basis. A superseded value remains in the changelog for auditability, except where publication would expose private, security-sensitive or otherwise non-public information. Current files contain only the corrected value.

## Companion repositories

The `sda-energy-data` and `sda-integration-cookbook` repositories version independently. A release or schema change in either companion does not change this repository's versions. Cross-repository references should identify a release tag or commit when reproducibility requires an immutable revision; links to `main` identify the current public material.

## Independent verification

Do not trust a repository value solely because it appears in a file here.

1. Confirm the mint, token program, decimals, supply and revoked mint and freeze authorities against [Solscan](https://solscan.io/token/SDAmxfpgaGmtxTqcTcvr4yi2kBwEFxTLF2XU4oLFw4b) or a Solana mainnet query implemented from the [Solana documentation](https://solana.com/docs).
2. Confirm the issuer, DTI, classification, competent authority, document version and regulatory scope in the [current MiCA white paper](https://sdafintech.com/legal/mica/whitepaper/SDA-Token-MiCA-Whitepaper-v1.3-2026_07_16.xhtml).
3. Confirm the issuer LEI through the [GLEIF LEI record](https://search.gleif.org/#/record/89450058XEES8WCSCQ03).
4. Record the source, retrieval date and discrepancy before proposing a correction.
