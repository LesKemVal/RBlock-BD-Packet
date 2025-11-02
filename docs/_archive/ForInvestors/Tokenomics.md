# 🪙 Tokenomics Strategy

This document outlines the token structure and mechanics behind R. Block Nation’s dual-raise strategy: issuing equity tokens (REGCFToken) under Regulation CF and non-dilutive revenue-share tokens (BFTKN) under Regulation A+ (if and when the platform scales).

---

## 🎯 Purpose of Dual Tokens

We use **two distinct tokens** to align investor classes and platform phases:

| Token Name        | Regulation | Purpose              | Type             | Issued To              |
|------------------|------------|----------------------|------------------|------------------------|
| REGCFToken        | Reg CF     | Equity + governance  | ERC-20 (Class B) | Early retail investors |
| BFTKN (Fallback)  | Reg A+     | Revenue-share only   | ERC-20           | Public retail token buyers |

---

## 🧱 Modular Deployment Logic

- **Month 0–3**: Only REGCFToken is issued through a funding portal via Form C filing.
- **BFTKN (Reg A+) is conditional**: Issued only if CF raise(s) gain traction and platform readiness is proven.
- REGCFToken and BFTKN will **never convert into each other** or co-mingle rights.

---

## 🔐 REGCFToken (Equity Token)

| Attribute            | Value                                  |
|----------------------|----------------------------------------|
| Regulation           | Reg CF                                 |
| Token Type           | ERC-20 Class B                         |
| Rights               | Equity ownership (non-voting)          |
| Lockup Period        | 12 months                              |
| Tradability          | Secondary transfer after lockup        |
| Offered Through      | FINRA-registered funding portal        |
| KYC/AML              | Enforced by portal + KoreConX          |
| Governance           | Class B (no voting)                    |
| Cap Table            | Integrated via KoreConX                |

> 🔒 REGCFToken holders are equity stakeholders, subject to the same cap table protections as other members.

---

## 📈 BFTKN (Non-Dilutive Token)

| Attribute            | Value                                  |
|----------------------|----------------------------------------|
| Regulation           | Reg A+ (future, conditional)           |
| Token Type           | ERC-20                                 |
| Rights               | Fixed revenue share (non-equity)       |
| Price Logic          | Linear bonding curve                   |
| Lockup / Transfers   | Transfer-restricted, allowlist enforced|
| Offered Through      | Reg A+ broker-dealer or funding portal |
| Escrow & Issuance    | North Capital + Settlemint             |
| Tradability          | ATS once qualified + matched           |
| Platform Fee         | 0–2%                                   |

> 🧪 **Note**: BFTKN is a fallback model to scale participation without further equity dilution.

---

## 🧮 Summary of Token Utility

| Feature                    | REGCFToken       | BFTKN            |
|----------------------------|------------------|------------------|
| Equity Ownership           | ✅ Yes            | ❌ No             |
| Revenue Sharing            | ❌ No             | ✅ Yes (fixed %)  |
| Voting Rights              | ❌ No             | ❌ No             |
| Transfer Restriction       | 12-month lockup   | Allowlist only   |
| Regulation Used            | Reg CF            | Reg A+ (future)  |
| Issuance Partner(s)        | Funding Portal    | KoreConX/NorthCap|

---

## 📢 Disclaimer

This tokenomics document is for **illustrative and strategic purposes only** and does not constitute an offer to sell or a solicitation of an offer to buy any securities or tokens. Any offerings will be made solely pursuant to a qualified offering under applicable securities regulations (e.g., Form C or Form 1-A), with full disclosure provided to investors.

---

Let me know when it’s pasted so we can stage, commit, and push.

