# Regulatory Map: European Union

## Primary Framework

| Regulation | Regulator | Applies To |
|------------|-----------|------------|
| MiCA (EU 2023/1114) | ESMA / NCAs | Crypto-asset issuers and service providers |
| MiFID II | ESMA / NCAs | Financial instruments (tokenized securities) |
| AIFMD | ESMA / NCAs | Tokenized fund interests |
| AMLD6 | National FIUs | AML obligations |
| GDPR | DPAs | Personal data in KYC processes |

## MiCA Token Classification

| Token Type | MiCA Category | Key Obligations |
|------------|--------------|------------------|
| Stablecoin (fiat-referenced) | E-money token (EMT) | E-money institution authorization |
| Multi-asset backed token | Asset-referenced token (ART) | MiCA authorization, reserve assets, white paper |
| Other crypto-assets | CASP regime | White paper, marketing rules |
| Security token | Outside MiCA → MiFID II | Prospectus / private placement |

> **Note**: Security tokens that qualify as MiFID II financial instruments fall outside MiCA. Check with EU counsel.

## MiCA ART Issuer Key Requirements

- **Authorization**: Required from competent national authority before issuance
- **White paper**: Filed with CNA + published before offering
- **Own funds**: Min EUR 350,000 or 2% of reserve assets
- **Reserve assets**: Held in custody, invested in low-risk instruments only
- **Redemption**: At par, on demand, within defined timeframe
- **Ongoing reporting**: Periodic reports to CNA

## ERC-3643 Mapping

| EU Requirement | ERC-3643 Implementation |
|----------------|------------------------|
| Professional investor only | Investor type claim in ONCHAINID |
| EEA-only distribution | `CountryRestrict` module — whitelist EEA country codes |
| Redemption mechanism | Off-chain process + on-chain burn function |
| Reserve asset transparency | Off-chain reporting + optional on-chain attestation |
