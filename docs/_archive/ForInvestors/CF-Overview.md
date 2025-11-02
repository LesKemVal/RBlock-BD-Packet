# 🪙 REGCFToken — Reg CF Equity Overview

This document outlines the structure and investor logic of the **REGCFToken**, a Class B equity token issued under Regulation Crowdfunding (Reg CF) and designed to form the **foundation of R. Block Share Holdings, LLC’s multi-raise strategy**.

The Reg CF raise activates the platform, validates traction, and unlocks future offerings, such as the non-dilutive BFTKN (Reg A+).

---

## 🎯 Purpose of the REGCFToken

- **Equity Participation**: Tokenholders receive a proportional Class B equity interest in the platform’s issuing entity.
- **12-Month Lockup**: In compliance with Reg CF, tokens are subject to a 12-month restricted transfer period.
- **Governance Limits**: Class B tokens do not confer voting rights, preserving founder control.
- **Perk Optionality**: Platform may offer early investor perks tied to token ownership (e.g., access, discounted fees, gated features).
- **KYC/AML**: All purchasers are verified via a funding portal partner (e.g., KoreConX, RaiseGreen, etc.).

---

## 🔍 Technical Token Overview

| Property             | Value                                                  |
|----------------------|--------------------------------------------------------|
| Token Name           | REGCFToken                                             |
| Standard             | ERC-20                                                 |
| Chain                | Ethereum Sepolia (testnet)                            |
| Issuer               | R. Block Share Holdings, LLC                           |
| Rights               | Equity (Class B Units)                                 |
| Transferability      | 12-month lock per Reg CF; ATS-optional thereafter      |
| Smart Contract       | [0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f](https://sepolia.etherscan.io/address/0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f?utm_source=chatgpt.com#code) |
| Compliance Stack     | KoreConX, North Capital, Settlemint                   |

---

## 🛠️ Smart Contract Notes

The REGCFToken includes allowlist enforcement and minting logic consistent with crowdfunding rules:

- Minting is paused until escrow settlement is confirmed
- Wallets must pass portal-issued KYC before receiving tokens
- Transfers are restricted for 12 months, with admin-controlled override for exempt scenarios

---

## 📈 Why Start with Reg CF?

Launching with Reg CF allows the platform to:

- ✅ Validate product-market fit before scaling
- ✅ Bring in early believers as equity-aligned stakeholders
- ✅ Prove traction for follow-on Reg A+ raises
- ✅ Maintain compliance and trust via FINRA-regulated intermediaries
- ✅ Access both retail and community investors on a low-barrier basis

---

## ⚖️ Legal Disclaimer

This token represents a security issued pursuant to Regulation Crowdfunding and may only be offered via a FINRA-registered funding portal. All investments are subject to risk. This document does not constitute an offer to sell or a solicitation of an offer to buy any securities. 

All transactions are subject to regulatory review and approval. Investors must review the full Form C offering documents before committing capital.

---

© R. Block Share Holdings, LLC — All Rights Reserved

