<link rel="stylesheet" href="../assets/spacing.css">

# R. Block Nation — Smart Contract Upgrades (Phase 2)

---

## 🔹 1. TransferAgent.sol — Add AGM + eVote Hooks

**Purpose:**  
Automates the organization and execution of **Annual General Meetings (AGMs)** directly on-chain.  
Integrates **eVoting** for token holders, ensuring investor rights and participation parity with traditional shareholders — critical for **Reg A+** and higher-volume **Reg CF** offerings.

**Usefulness:**  
✅ Enhances **shareholder governance** within tokenized cap tables.  
⚖️ Strengthens compliance with investor-protection expectations (*“same rights as traditional shareholders”*).  
📊 Stores voting outcomes immutably on-chain for audit and regulatory transparency.

---

## 🔹 2. ComplianceRegistry.sol — Emit InvestorVerified

**Purpose:**  
Emits an event whenever an investor passes **KYC/AML** (or accreditation) checks, creating a verifiable, auditable on-chain compliance trail.

**Usefulness:**  
✅ Enables **transfer restrictions** (only verified investors may transfer).  
✅ Supports **ATS / secondary market readiness**.  
🛡️ Improves trust, transparency, and real-time oversight for broker-dealers and regulators.

---

## 🔹 3. GovernanceBoard.sol — Record Shareholder Resolutions

**Purpose:**  
Allows submission and recording of **shareholder resolutions**, including voting results, board approvals, and investor actions, stored immutably on-chain.

**Usefulness:**  
✅ Key for **tokenized equity** under Reg A+ or advanced Reg CF offerings.  
📘 Reinforces **corporate governance transparency** and issuer accountability.  
🔍 Meets audit and record-retention requirements under **FINRA Rule 4511**.

---

**Next Steps:**
These modules will be compiled and deployed alongside the upgraded `TransferAgent.sol`  
and indexed in your subgraph for automated governance and compliance reporting.

---

[← Back to Progress Report (Nov 2025)](../ProgressReport/)
[↔ View Internal Compliance & BD Alignment (Nov 2025)](../BD-Compliance-Alignment/)
