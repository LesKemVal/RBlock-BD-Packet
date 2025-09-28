# Compliance Readiness Checklist (Reg CF)

Use this checklist before each CF raise. Aligns with BD supervision, FINRA 17a-4 books/records, and platform governance.

## 1) Governance & Roles
- [ ] BD engagement letter active; scope & WSP mapping documented
- [ ] Supervisory Principal assigned (independent of issuer conflicts)
- [ ] Tech vendor responsibility matrix (RACI) approved (R. Block / BD / Kore / Escrow)
- [ ] Incident response owners & contacts listed

## 2) Disclosures & Offering Docs
- [ ] Form C filed (and any amendments) — links surfaced on offer page
- [ ] Risk factors, use of proceeds, conflicts, fees disclosed on-platform
- [ ] Marketing rules: platform-only materials, deep-link back to offering page

## 3) Platform Controls
- [ ] UI templates pre-cleared by BD; change log archived
- [ ] Ads/social content pre-cleared; archived with timestamps
- [ ] Investor Q&A and updates on-platform and archived

## 4) Onboarding & Escrow
- [ ] CIP/KYC/AML configuration validated (North Capital)
- [ ] Funding flow tested end-to-end; recon reports available to BD
- [ ] Threshold/close rules documented; exception handling defined

## 5) Smart Contract / On-Chain
- [ ] Contract verified on Etherscan; address linked in docs
- [ ] Funding window configured; admin/operator roles granted to BD/Kore principals
- [ ] Revenue/transfer restrictions match offering terms
- [ ] Deployment tag and artifacts archived (ABI, bytecode, deployments JSON)

## 6) Books & Records (17a-4)
- [ ] Archival system captures: offering page, investor comms, confirmations, docs
- [ ] Immutable retention policy set; export tested
- [ ] Daily/weekly data recon between on-chain, escrow, cap table

## 7) Security & Privacy
- [ ] Access reviews for admins; least privilege enforced
- [ ] Vendor due diligence (SOC/ISO, BCP, uptime/SLA) current
- [ ] PII handling & DPA in place; breach notification terms agreed

## 8) Launch Readiness
- [ ] Dry run completed with BD sign-off
- [ ] Support runbooks & escalation paths published
- [ ] Post-launch monitoring dashboards live (exceptions, recon, uptime)

**Links**
- [Raise #1 — Buildout](./raise-1-buildout.md)
- [Raise #2 — Scale](./raise-2-scale.md)
- [BD Oversight & WSP Mapping](./roles-and-oversight.md)
- [Data Room / Diligence Checklist](./data-room-checklist.md)
