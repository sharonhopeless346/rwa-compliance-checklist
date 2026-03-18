# Checklist 02: Token Design & On-Chain Architecture

## 2.1 Token Classification
- [ ] Token type confirmed: **security token** (equity, debt, fund interest, real estate)
- [ ] Legal opinion on token classification obtained
- [ ] Token economics documented (supply, distribution, rights of holders)

## 2.2 Smart Contract Architecture
- [ ] Token standard selected: **ERC-3643 / T-REX** (recommended for security tokens)
- [ ] Smart contract audit completed by reputable auditor
- [ ] Audit report published
- [ ] Upgradeability strategy defined (proxy pattern or immutable)

## 2.3 ERC-3643 / T-REX Implementation
- [ ] ONCHAINID identity registry deployed
- [ ] Compliance module deployed and configured
- [ ] Transfer restriction module active
- [ ] Claim topics registry configured
- [ ] Trusted claim issuers list established
- [ ] Token factory or direct deployment completed

## 2.4 Compliance Module Configuration
- [ ] Country restriction module configured
- [ ] Maximum investor count set (if applicable)
- [ ] Per-investor balance cap set (if applicable)
- [ ] Lockup / holding period configured (if applicable)
- [ ] Investor type restriction configured (accredited / qualified)

## 2.5 Multi-sig & Key Management
- [ ] Owner / admin keys secured in multi-sig wallet
- [ ] Key management policy documented
- [ ] Emergency pause function tested
- [ ] Recovery procedure documented
