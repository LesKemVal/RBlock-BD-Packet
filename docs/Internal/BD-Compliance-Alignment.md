# R. Block Nation — Internal Compliance & Broker-Dealer Alignment (November 2025)

---

## 🧭 Overview

This page provides Andes Capital and other broker-dealer partners with a clear view of the internal compliance architecture, audit controls, and supervisory procedures currently active within the **R. Block Nation** ecosystem.  

All items below have been verified internally in preparation for **Pre-Live Certification** under broker-dealer supervision.

---

## 🧾 1. Written Supervisory Procedures (WSP) Mapping

R. Block Nation’s compliance framework maps each operational function to applicable SEC and FINRA rules:

| Function | Regulatory Basis | Enforcement Mechanism |
|-----------|------------------|------------------------|
| Investor Onboarding / KYC / AML | SEC Rule 227.304 | North Capital TransactAPI (`performKycAml`) |
| Escrow Management | SEC Rule 15c2-4 | North Capital Escrow API (`createAccount` / `balance`) |
| Books & Records Retention | FINRA Rule 4511 | Immutable Subgraph + Evervault archive (5-year retention) |
| Transfer Agent Function | SEC Rules 17Ad-1 & 17Ad-4 | `TransferAgent.sol` contract + IPFS metadata |
| Advertising & Communications | FINRA Rule 2210 / CF 203 | Archived via SMTP + IPFS hashing |
| Shareholder Governance | Reg A § 251 / CF 204 | `GovernanceBoard.sol` on-chain voting |

📄 *Full WSP mapping document stored under*  
`/Internal/ProgressReport/`

---

## 🗂 2. Books & Records Capture

- **Immutable on-chain audit trail** — every event (KYC verified, escrow funded, token issued) is indexed by The Graph Node and timestamped for audit retrieval.  
- **Redundant storage** — Postgres + Evervault + IPFS backup ensures tamper-evident records.  
- **Retention policy:** Five-year digital preservation per FINRA 4511.  
- **Data access controls:** Restricted API keys + read-only BD dashboard visibility.

---

## 🧠 3. Data Protection & Access Control

- Role-based `AccessControl` (`BD_SUPERVISOR_ROLE`, `ISSUER_ROLE`, `INVESTOR_ROLE`) implemented at the contract level.  
- All PII encrypted at rest through Evervault; wallet data remains on-chain only.  
- GDPR / CCPA disclosures and data-erasure procedures drafted and posted in the **Terms** directory.

---

## 🧩 4. Reg CF vs. Reg A Structural Separation

- Distinct contract namespaces: `RegCFToken.sol` and `BFTKN.sol`.  
- Dedicated subgraph entities and schemas for each regulation type.  
- UI segmentation ensures CF and A+ offerings are never cross-displayed to investors.  
- Compliance flags within each contract prevent mis-issuance or cross-sale.

---

## 📜 5. Communication Supervision

- All system emails and announcements routed through Evervault SMTP and archived to IPFS.  
- Communication IDs hash-linked to transaction events for FINRA 2210 audit retrieval.  
- Internal policy: no public posting or investor communication occurs without record capture.  
- Broker-Dealer visibility: read-only access to all archived threads and platform logs.

---

## 🔍 6. Sandbox Certification Preparation

**Validated API Tests stored in `/src/lib/`:**

kycAmlTest.ts — Auto-approved status proof
escrowTest.ts — Balance verification
escrowAccountTest.ts — Account creation confirmation



- Pre-Live Checklist: Each UI action triggers and logs a real API response for certification review.  
- Mock Investors: Demonstrate positive, negative, and pending KYC scenarios for testing.

---

## 🏛 7. Broker-Dealer Visibility

- BD Dashboard provides read-only access to investor activity, issuer approvals, and token issuances.  
- Offering documents and escrow agreements are stored in an encrypted vault with BD API pull rights.  
- Audit trail automatically exports to CSV and JSON for FINRA or SEC review.  
- `BD_SUPERVISOR_ROLE` smart-contract permission ensures no offering goes live without BD sign-off.

---

## 🎬 Pre-Live Certification Walk-Through

A recorded **8-minute walk-through** will be provided to Andes Capital demonstrating:

- Investor onboarding flow (`createParty` → `performKycAml` → `createAccount`)  
- Compliance dashboard and books-and-records capture  
- Token issuance and subgraph event verification  
- BD visibility and oversight controls  
- Closing and next steps for production API transition  

The video link will be shared privately for internal compliance review and certification files.

---

## ✅ Summary

R. Block Nation’s compliance infrastructure now meets all core requirements for broker-dealer supervision and Reg CF / Reg A onboarding.  

With North Capital handling KYC/AML and escrow, and on-chain Transfer Agent logic replacing third-party dependencies, the platform is ready for **final certification and production approval** under Andes Capital’s oversight.

---

📄 **Last Updated:**  
**November 1, 2025** — Prepared by *Lester Sawyer, Founder, R. Block Nation*

---

[← Back to Progress Report (Nov 2025)](../ProgressReport.md)  
[Back to top](#r-block-nation--internal-compliance--broker-dealer-alignment-november-2025)

