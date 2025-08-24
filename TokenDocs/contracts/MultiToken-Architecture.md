# R. Block Nation | Multi-Token Architecture Strategy

This document outlines the planned architecture for supporting multiple token types across the R. Block Nation platform, including equity (Reg CF/A/D), rev-share, real estate, and tokenized debt offerings.

---

## 🔐 1. RBCB: Equity (Class B Non-Voting) — ✅ Live

**Contract Name:** `RegCFToken`  
**Purpose:** Class B non-voting equity tokens (Reg CF-compliant)  
**Features:**
- Admin-gated minting after KYC + escrow settlement
- 12-month lockup (Reg CF rule)
- KYC-gated transfers + exemptions
- Cap table export support
- Treasury allocation (manual for now)

---

## 📈 2. RBTRev: Revenue Share Token — 🔄 Planned

**Contract Name:** `RevShareToken` *(planned)*  
**Use Case:** Franchises, creator IP, or businesses offering shared revenue  
**Key Features:**
- Transferable ERC20 with KYC gating
- Optional lockup period (not equity)
- Manual or programmatic revenue distribution
- Rev share structured as claimable or staked balance
- Can plug into franchise model or creative royalty splits

---

## 🏠 3. RBTReal: Real Estate Token — 🔄 Planned

**Contract Name:** `RealAssetToken` *(planned)*  
**Use Case:** Tokenizing fractional ownership of real estate  
**Key Features:**
- ERC20 or ERC721 hybrid
- KYC-gated transfer + compliance enforcement
- Whitelist-based issuance (SEC Reg A/D)
- Dividend or rental yield integration
- Escrow + legal entity link (LLC/SPV)

---

## 💳 4. RBTDebt: Debt Note Token — 🔄 Planned

**Contract Name:** `DebtNoteToken` *(planned)*  
**Use Case:** Representing fixed-term tokenized debt for businesses  
**Key Features:**
- Minted only after escrow + approval
- Non-transferable unless exemption applies
- Payment schedule mapped on-chain or off-chain via metadata
- Optional lockup or burn after payoff

---

## 🏛️ 5. Platform Treasury Allocation Logic (Optional)

To maintain competitiveness while supporting platform growth:

- Treasury may claim a % of token supply (equity, rev-share, etc.)
- Allocations to be **disclosed in Form C or issuer terms**
- Can support long-term platform valuation

Example logic (future optional):

```solidity
uint256 treasuryAmount = (amount * 2) / 100;
_mint(treasuryWallet, treasuryAmount);

💼 6. Issuer Governance Options

Each issuer may define:

Voting vs. non-voting tokens

Transfer restrictions

Rev share or not

Token class naming (Class B, Series A, etc.)

The platform will standardize onboarding, UI, compliance, and secondary listing, but governance terms remain per-issuer.

🚀 7. Long-Term: Investor Financing Tools

After “franchise theory” is proven:

Platform will explore enabling investors to obtain loans to:

Purchase full or remaining token supply in a deal

Access leveraged exposure (subject to compliance)

Potential use case:

Investor borrows to acquire 100 tokens = 100% stake in a local franchise

Loan repayable via yield or rev share

This model will be phased in strategically with proper legal + BD oversight.

📌 Note: All tokens issued will be subject to legal counsel review, platform terms, and FINRA/SEC guidance.

For questions:
📧 lester@rblockshareholdings.com
