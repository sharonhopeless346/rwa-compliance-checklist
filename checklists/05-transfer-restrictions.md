# Checklist 05: Transfer Restrictions

## 5.1 Transfer Restriction Design
- [ ] Transfer restriction policy documented
- [ ] On-chain restrictions mapped to off-chain regulatory requirements
- [ ] Transfer restriction table completed (see template)
- [ ] Restricted jurisdiction list finalized
- [ ] Legal review of transfer restriction structure obtained

## 5.2 On-Chain Implementation (ERC-3643)
- [ ] `CountryRestrict` module: restricted country codes configured
- [ ] `MaxInvestors` module: maximum holder count set (if applicable)
- [ ] `MaxBalance` module: per-investor cap configured (if applicable)
- [ ] `TimeExchangeLimits` module: lockup period configured (if applicable)
- [ ] Compliance module tested on testnet before mainnet deployment
- [ ] Transfer restriction tests documented and passed

## 5.3 Secondary Market Controls
- [ ] Secondary market trading policy documented
- [ ] Approved trading venues listed (ATS, regulated market, OTC only)
- [ ] Unapproved transfer attempt handling defined (revert behavior tested)
- [ ] Investor notification of secondary market restrictions in subscription agreement

## 5.4 Corporate Actions
- [ ] Transfer restriction update procedure on corporate action (split, merger, etc.) documented
- [ ] Force transfer capability (regulatory seizure / court order) documented
- [ ] Recovery procedure for lost/locked wallets documented

## 5.5 Ongoing Monitoring
- [ ] Transfer log reviewed monthly
- [ ] Failed transfer attempts reviewed and investigated
- [ ] Claim expiry alerts actioned before transfer failures occur
