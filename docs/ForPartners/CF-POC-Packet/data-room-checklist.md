# Data Room / Diligence Checklist (Reg CF POC)

Use this list when sharing materials with the Broker-Dealer and vendors (Kore, North Capital, SettleMint).

## 1) Company & Governance
- [ ] Articles/Operating Agreement; cap table summary
- [ ] Key personnel bios; org chart; conflict disclosures (issuer + tech provider)
- [ ] Key policies: InfoSec, privacy, incident response, change management

## 2) Offering Documents
- [ ] Draft/Form C (and expected amendments)
- [ ] Risk factors; use of proceeds; fee schedules; marketing standards
- [ ] Subscription docs & investor acknowledgments (platform templates)

## 3) Technology (Platform & Vendors)
- [ ] Architecture diagram (front-end, Kore, SettleMint, escrow, chain)
- [ ] Environment matrix (prod/test), access controls, audit logs
- [ ] Vendor DDQ/SOC/ISO summaries (Kore, North Capital, SettleMint)
- [ ] Uptime/SLA, BCP/DR, data residency, PII handling/DPA

## 4) Books & Records (17a-4)
- [ ] Archiving approach for pages, comms, confirmations, Q&A, ads/social
- [ ] Retention settings (immutable/WORM), export/ediscovery procedures
- [ ] Example daily/weekly reconciliation reports

## 5) Escrow & KYC/AML
- [ ] Escrow agreement; flow diagrams; exception handling playbooks
- [ ] CIP/KYC/AML configuration (rules, sanctions lists, flags)
- [ ] Funding/returns workflows; reconciliations; close/contingency rules

## 6) Smart Contracts / On-Chain
- [ ] Etherscan link (verified):  
  - Reg A (BFTKN): `https://sepolia.etherscan.io/address/0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858#code`
- [ ] Artifacts bundle (ABI, bytecode, deployments JSON, tag notes)
- [ ] Role assignments (DEFAULT_ADMIN, ADMIN, KORE_OPERATOR) and change log
- [ ] Config: funding window, escrow wallet, transfer logic overview

## 7) Marketing & Communications
- [ ] Pre-cleared UI templates, disclaimers/legends
- [ ] Ads/social content plan; deep-linking back to offering page
- [ ] Monitoring & approval workflow; archive samples

## 8) Financial & Ops
- [ ] Budget/use-of-proceeds; vendor costs; platform OPEX
- [ ] Success fee model (BD) and *non-BD* compensation (R. Block Nation tech)
- [ ] KPIs for POC (time-to-clear, recon match rate, uptime)

---

**Related**
- [Roles & Oversight (WSP Mapping)](./roles-and-oversight.md)
- [Compliance Readiness Checklist](./compliance-readiness.md)
- [Raise #1 — Buildout](./raise-1-buildout.md)
- [Raise #2 — Scale](./raise-2-scale.md)
