# Checklist 03: KYC / AML Program

## 3.1 KYC Program Foundation
- [ ] KYC policy documented and approved
- [ ] KYC provider selected and integrated (e.g., Sumsub, Jumio, Onfido)
- [ ] KYC levels defined:
  - Level 1: Identity verification (ID + selfie)
  - Level 2: Enhanced DD (proof of address, source of funds)
  - Level 3: Institutional / corporate KYC
- [ ] KYC renewal schedule set (recommended: annual refresh)

## 3.2 AML Screening
- [ ] Sanctions screening integrated: OFAC SDN, EU consolidated, UN list
- [ ] PEP (Politically Exposed Person) screening integrated
- [ ] Adverse media screening implemented
- [ ] Ongoing monitoring for existing investors configured
- [ ] SAR filing procedure documented (US: FinCEN; EU: FIU)

## 3.3 On-Chain Identity Claims (ERC-3643)
- [ ] KYC claim issued to verified investors via approved claim issuer
- [ ] AML claim issued after screening clearance
- [ ] Claim expiry dates set and renewal alerts configured
- [ ] Revocation procedure documented (for failed renewals or adverse events)

## 3.4 Travel Rule Compliance (FATF)
- [ ] VASP registration determined (jurisdiction-dependent)
- [ ] Travel Rule solution integrated if transfers > $1,000 / €1,000
- [ ] Counterparty VASP verification procedure documented

## 3.5 Record Retention
- [ ] KYC records retained for minimum 5 years post-relationship end
- [ ] AML screening records retained
- [ ] SAR records retained for minimum 5 years
