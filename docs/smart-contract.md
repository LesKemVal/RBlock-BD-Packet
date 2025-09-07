# Smart Contracts

This section provides details on the smart contracts supporting the R. Block investment framework. These contracts are deployed on the Ethereum Sepolia testnet for transparency and compliance verification.

> **Disclaimer:**  
> This platform reflects a proposed model for JOBS Act-compliant investing focused on expanding access to non-traditional communities. While the core mission — transparency, community ownership, and regulatory integrity — remains fixed, I am open to adapting aspects of the business model or tech stack to align with a regulated broker-dealer or funding portal relationship. My domain and investor UI are essential components of the brand experience, and I seek partnerships that allow for long-term valuation growth and operational integrity.

---

## ⚖️ Reg CF Token — Class B Non-Voting Membership Units

**Contract Address:**  
[`0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f`](https://sepolia.etherscan.io/address/0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f#code)

**Network:** Sepolia Testnet  
**Symbol:** TBD  
**Decimals:** 0 or 2 (configurable)  

# Smart Contracts

This section outlines the smart contracts used for our investor tokens, deployed to the Ethereum Sepolia testnet for testing and demonstration.

---

## 📘 Reg CF Token (Class B Non-Voting Units)

**Network:** Sepolia Testnet  
**Symbol:** TBD  
**Decimals:** 0 or 2 (configurable)  
**Contract Address:** [`0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f`](https://sepolia.etherscan.io/address/0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f)

### 🔍 Summary

This ERC-20 contract represents **Class B non-voting membership units** offered under **Regulation CF**. Key features:

- ✅ **KYC Whitelist**: Only approved investors can receive tokens.
- ⏱️ **12-Month Lockup**: Required by Reg CF. Applies to all holders.
- 🔁 **Limited Transfers** during lockup:
  - To issuer (admin-controlled wallets)
  - To accredited investors
  - To trusts controlled by investors
  - Pre-approved FROM→TO pairs (estate/divorce transfers)
- 📅 **Global Unlock Option**: Transfers may be unlocked for all after 12 months (still KYC-gated).
- 📋 **Cap Table Tools**: View holder list on-chain for compliance.

This contract is designed for compliance and integrates easily with KoreConX, transfer agents, or broker-dealers.

---

## 📘 Reg A Token (Coming Soon)

**Contract Address:** _To be added_

### 🔍 Summary

This token will represent **Regulation A+ Tier 2 offerings**, and include features like:

- ✅ Transferable after qualification (with optional KYC gating)
- 🧩 Integration hooks for cap table & compliance
- 📊 Structured for investor liquidity and secondary trading

---


