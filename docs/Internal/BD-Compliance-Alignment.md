<link rel="stylesheet" href="../assets/spacing.css">

# R. Block Nation — Internal Compliance & Broker-Dealer Alignment (November 2025)

---

## ⚖️ 1. Purpose

To outline how **R. Block Nation** ensures that all crowdfunding and investment operations comply with **FINRA** and **SEC** requirements under the supervision of its broker-dealer partner **Andes Capital**.  
This page also serves as a reference for **North Capital** (escrow + KYC/AML) and any future **Transfer Agent (TA)** integration partners.

---

## 🧱 2. Core Compliance Architecture

| Component | Partner / Tool | Purpose |
|:--|:--|:--|
| **Broker-Dealer (BD)** | **Andes Capital** | Supervises all offerings; maintains WSP mapping and oversight. |
| **Escrow & KYC/AML** | **North Capital TransactAPI** | Performs investor identity verification and manages escrow funds. |
| **Transfer Agent / Cap-Table** | 🧩 In Progress | Replacing Kore with on-chain TA logic + optional API integration. |
| **Smart-Contract Backend** | **SettleMint ATK** | Manages token issuance, compliance roles, and transaction logs. |
| **UI / Frontend Portal** | **Custom React (Vite + Tailwind)** | Provides investor/issuer access while maintaining BD audit trail. |
| **Legal & Governance** | Outside Counsel (Post-Raise) | Oversees filings, corporate actions, and enforcement. |

---

## 🔐 3. Oversight Workflow

1. **Investor Onboarding / KYC**
   - Initiated via **North Capital TransactAPI**
   - Returns `kyc_verified = true`
2. **Broker-Dealer Approval**
   - Andes Capital reviews offering + escrow agreement
   - Status → `approved_for_funding`
3. **Funding in Escrow**
   - Investor wires funds → North Capital Escrow
   - Status → `funded_in_escrow`
4. **Close of Escrow**
   - BD confirms compliance → North Capital closes escrow
   - Status → `escrow_released`
5. **Token Issuance**
   - SettleMint mints RegCFToken / BFTKN
   - Status → `token_issued`
6. **Record Keeping**
   - BD and TA capture all events for audit / Form C / Form 1-A filings

---

## 🧩 4. Technical Controls

| Area | Validation | Current Status |
|:--|:--|:--|
| **TransactAPI (KYC/AML)** | `createParty`, `performKycAml`, `createAccount`, `getEscrowBalance` | ✅ All sandbox tests 200 OK |
| **Escrow Integration** | Sandbox UI demo planned for Pre-Live Certification | 🧩 Pending |
| **Smart Contracts** | On-chain AccessControl + event logging | ✅ Operational |
| **Subgraph** | Real-time indexing for KYC, Escrow, Token events | ✅ Running |
| **Transfer Agent Module** | `TransferAgent.sol` under construction | ⚙️ In Progress |

---

## 📁 5. Documentation & Records

| Category | Storage Location | Visibility |
|:--|:--|:--|
| **Investor KYC/AML Logs** | North Capital secure API + local audit backup | BD + Issuer on request |
| **Escrow Confirmations** | North Capital Dashboard + Platform UI | BD / Issuer access |
| **Token Issuance Events** | SettleMint Subgraph + Graph Node | Public read-only |
| **Compliance Docs + WSP Mappings** | RBlock-BD-Packet (MkDocs Repository) | Internal only |

---

## 🪜 6. Upcoming Compliance Milestones

| Phase | Deliverable | Target Date |
|:--|:--|:--|
| **Pre-Live Certification** | Recorded UI walk-through for North Capital + Andes | 🎯 November 2025 |
| **Transfer Agent Deployment** | Launch on-chain cap-table with BD oversight | 🎯 December 2025 |
| **Reg CF Raise #1 Launch** | BD-supervised retail raise via platform | ⏳ Post-Certification |
| **Reg A+ Preparation** | Legal review + token economics finalization | 🧩 Q1 2026 |

---

✅ **Overall Compliance Readiness:** ≈ 90 %  
🧭 **Next Focus:** UI demo for certification + TA integration validation.  

---

[← Back to Top](#r-block-nation--internal-compliance--broker-dealer-alignment-november-2025)

---


---


---


---

[← Back to Progress Report (Nov 2025)](../ProgressReport/)
[→ View Smart Contract Upgrades (Phase 2)](../SmartContract-Upgrades/)

---

## 🔗 Certification Continuity (2025-11-09)
See also:
- [Pre-Live Certification Packet](./PreLive_Certification_Packet_2025-11-09.md)
- [BD Readiness Checklist](./BD_Readiness_Checklist_2025-11-09.md)

Together these form the official **Pre-Live Certification Packet** for BD approval.
