# Regulatory Map: United States

## Primary Framework

| Regulation | Regulator | Applies To |
|------------|-----------|------------|
| Securities Act of 1933 | SEC | Token offering registration / exemption |
| Securities Exchange Act of 1934 | SEC | Secondary market, broker-dealer registration |
| Reg D Rule 506(b) / 506(c) | SEC | Private placement to accredited investors |
| Reg S | SEC | Offerings to non-US persons |
| Reg A+ | SEC | Up to $75M offering, lighter disclosure |
| FINRA Rule 3110 | FINRA | Broker-dealer supervision |
| FINRA Rule 4511 | FINRA | Books and records |
| SEC Rule 17a-4 | SEC | Electronic recordkeeping |
| SR 11-7 | Federal Reserve / OCC | Model risk management |
| BSA / AML | FinCEN | AML program, SAR filing |

## Key Decision Points

### Is the token a security?
- Apply Howey Test: investment of money + common enterprise + expectation of profit + efforts of others
- If yes → must register or qualify for exemption
- Most RWA tokens (real estate, private credit, fund interests) = securities

### Which exemption?
| Exemption | Investors | Limit | Resale |
|-----------|-----------|-------|--------|
| Reg D 506(b) | Accredited (+ up to 35 sophisticated) | No cap | Restricted (Rule 144 lockup) |
| Reg D 506(c) | Accredited only (verified) | No cap | Restricted |
| Reg S | Non-US persons only | No cap | Restricted (40-day lockup) |
| Reg A+ Tier 2 | Anyone (with limits) | $75M/year | Freely tradeable after 1 year |

## ERC-3643 Mapping

| US Requirement | ERC-3643 Implementation |
|----------------|------------------------|
| Accredited investor verification | KYC + Accreditation claim in ONCHAINID |
| Restricted resale period | `TimeExchangeLimits` module |
| US person restriction (Reg S) | `CountryRestrict` module — block US country code |
| Investor count limit (3(c)(1): 100, 3(c)(7): 2000) | `MaxInvestors` module |
| Transfer agent functions | Smart contract compliance module + off-chain register |
