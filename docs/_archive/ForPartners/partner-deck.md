# Partner Deck — Overview

_Last updated: 2025-09-28_

## Who We Are
**R. Block Nation** partners with a FINRA broker-dealer to run compliant private offerings while we provide the technology stack (front end + smart contracts + integrations).

## What We’re Proposing
1) **Reg CF proof-of-concept raise** to fund platform buildout.  
2) **Follow-on raises** (CF/Reg A) as traction grows, with BD supervision end-to-end.

See the full POC packet: [CF Proof-of-Concept](./CF-POC-Packet/index.md)

---

## Architecture (High Level)
- **Front end:** Kore white-label UI (pages pre-cleared by BD).
- **Compliance & Cap Table:** Kore (KYC/AML, investor records, transfer agent).
- **Escrow:** North Capital (BD-supervised integrations, reconciliations).
- **Smart contract:** BusinessFranchiseToken (ERC-20) on Sepolia testnet.
- **Orchestration/Node:** SettleMint for RPC + deploys.
- **Books & Records:** BD owns/archives communications & artifacts (SEA 17a-4).

More detail: [Roles & Oversight (WSP)](./CF-POC-Packet/roles-and-oversight.md) · [Compliance Readiness](./CF-POC-Packet/compliance-readiness.md) · [Data Room Checklist](./CF-POC-Packet/data-room-checklist.md)

---

## Token & Contract (Testnet POC)
- **Name/Symbol:** FranchiseToken (**FTKN**)  
- **Network:** Sepolia (testnet)  
- **Contract:** `0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858`  
- **Etherscan:** https://sepolia.etherscan.io/address/0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858#code  
- **Features:** Role-based access (DEFAULT_ADMIN/ADMIN/KORE_OPERATOR), funding window, pause, escrow wallet integration, optional pricing toggle.

---

## Raises & Timeline
- **Raise #1 — Buildout (CF):** fund core platform + marketing ops (Year 1–2).  
- **Raise #2 — Scale (CF/Reg A):** expand features, reduce unit costs, hire dev/ops (Year 2–3).  
Details: [Buildout](./CF-POC-Packet/raise-1-buildout.md) · [Scale](./CF-POC-Packet/raise-2-scale.md)

---

## BD Supervision (Summary)
- Pre-clear UI/templates, supervise communications (WSP).
- Archive on-platform content; enforce “platform-only” rule for offers/updates.
- Approve escrow flows and reconcile subs/funding/returns before closing.
- Independent principal reviews R. Block Nation communications when we are issuer.

Full mapping: [Roles & Oversight](./CF-POC-Packet/roles-and-oversight.md)

---

## KPIs for POC
- Time-to-clear investment (CIP/KYC → escrow → allocation)  
- On-platform Q&A/updates archived  
- On-chain events match escrow & cap table states (reconciliations)

---

## Contacts
**Owner:** Lester Sawyer  
**Email:** contact@rblockshareholdings.com  
**Company:** R. Block Share Holdings, LLC

> **Disclaimer:** For demonstration only. Testnet contracts are not for investment. All offerings will be conducted under BD supervision and applicable securities laws.

---

## Smart Contract Links

- **Reg CF Token (Sepolia):**  
  [0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f](https://sepolia.etherscan.io/address/0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f#code)

- **Reg A Token — BFTKN (Sepolia):**  
  [0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858](https://sepolia.etherscan.io/address/0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858#code)
