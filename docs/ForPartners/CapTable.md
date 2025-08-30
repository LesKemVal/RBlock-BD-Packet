# 📊 Cap Table & Token Allocation Strategy

This cap table reflects our dual-raise strategy using both Reg CF (equity) and Reg A+ (non-dilutive revenue-share token). The structure is designed to support investor transparency, regulatory compliance, and long-term founder control.

---

## 💡 Raise Strategy Overview

| Raise Type | Method               | Vehicle                     | Investor Rights        | Cap     | Platform Fee | Notes                       |
|------------|----------------------|------------------------------|-------------------------|---------|---------------|-----------------------------|
| Reg CF     | Equity               | Class B Units (REGCFToken)  | Equity ownership        | $1.2M   | 6–8%          | Up to 23.08% equity diluted |
| Reg A+     | Revenue-share Token  | ERC20: BusinessFranchiseToken (BFTKN) | Revenue share         | TBD     | 0–2%          | Non-dilutive fallback       |

---

## 🎯 Allocation Breakdown (Post-Raise Scenarios)

### 📌 Scenario 1: Reg CF Raise Only (Equity Offering)

| Stakeholder         | % Ownership (Post-CF) | Notes                       |
|---------------------|-----------------------|-----------------------------|
| Founders (Class A)  | ≥ 51%                 | Retain full control         |
| Reg CF Investors    | 23.08% (Class B)      | Equity stake via REGCFToken |
| Platform/Reserves   | ~25.92%               | Ops, hires, partnerships    |

### 📌 Scenario 2: Dual Raise — Reg CF + Reg A+ Token (Equity + Revenue-Share)

| Stakeholder            | % Equity Ownership | % Revenue Share | Notes                                                    |
|------------------------|--------------------|------------------|----------------------------------------------------------|
| Founders (Class A)     | ≥ 51%              | Varies           | Control + long-term platform stewardship                 |
| Reg CF Investors       | 23.08%             | Optional         | Class B equity via REGCFToken                            |
| Reg A+ Tokenholders    | 0%                 | Contract-based   | Non-dilutive holders of BFTKN                            |
| Platform/Reserves      | ~25.92%            | Varies           | May reserve tokens for treasury or incentive allocation  |

> 🧮 **Note**: The Reg A+ token (BFTKN) uses a linear bonding curve, escrow-based distribution, and is not convertible to equity.

---

## 🪙 BFTKN Token Details (Reg A+)

| Feature              | Value                           |
|----------------------|---------------------------------|
| Token Name           | BusinessFranchiseToken (BFTKN)  |
| Symbol               | BFTKN                           |
| Standard             | ERC20 w/ bonding curve          |
| Issuer               | R. Block Share Holdings, LLC    |
| Rights               | % revenue share (contract-based)|
| Distribution Logic   | Escrow Wallet → Investors       |
| Price Model          | Linear bonding curve            |
| KYC/AML              | Enforced via allowlist          |
| Tradability          | Restricted transfers only       |

---

## 🔐 Legal Safeguards

- **Reg CF** equity tokens (REGCFToken) are issued through a FINRA-regulated funding portal.
- **Reg A+ fallback token** (BFTKN) is non-dilutive, non-equity, and SEC-qualified when offered.
- Offerings are integrated via KoreConX (cap table), North Capital (escrow), and Settlemint (token issuance).

---

## ⚠️ Disclaimer

> **This capital strategy involves one or more exempt securities offerings under U.S. law. R. Block Nation may offer securities under Regulation Crowdfunding (Reg CF), Regulation A+, or both.**
>
> - **The Reg CF raise is equity-based**, conducted via a registered funding portal. Investors receive Class B Units in R. Block Share Holdings, LLC through REGCFToken, subject to transfer restrictions.
>
> - **The Reg A+ raise (if used) offers BFTKN**, a revenue-share token issued via smart contract. BFTKN is not equity and confers no ownership or voting rights.
>
> - This dual-offering structure allows R. Block Nation to fund operations and regulated crowdfunding infrastructure development, even if the Reg CF raise is undersubscribed.
>
> - Compliance is ensured through KoreConX (onboarding, cap table), North Capital (escrow, KYC), and Settlemint (contract issuance and logic).
>
> **Investments are speculative and illiquid. Past performance is not indicative of future results. This content is not legal or investment advice.**


