# BD Readiness Checklist — R. Block Nation (2025-11-09)

This checklist ensures every component required for BD compliance and RWA readiness has been verified.

---

## 1. Environment Verification
☑️  Node / Yarn environment validated  
☑️  Hardhat compile & clean runs successfully (`npx hardhat clean && npx hardhat compile --force`)  
☑️  .env contains valid keys for:
- AGORA_APP_ID
- PRIMARY_CERTIFICATE
- NORTHCAP_API_KEY / ESCROW_API_KEY
- POSTGRES_URL / GRAPH_NODE_URL

---

## 2. Smart Contract Verification
| Contract | Status | Address |
|-----------|---------|----------|
| RegCFToken | ✅ Verified | 0x769780C2BA4492Ac4B0C3C38fbD0B2CB4bb9Ba5f |
| BFTKN | ✅ Verified | 0x9F2bc4CC40f7e39866F7DcBFe0127E9Dbc925858 |
| TransferAgent | ✅ Deployed | Local / Sepolia |
| GovernanceBoard | ✅ Deployed | Local / Sepolia |

☑️  Contract ABIs exported to `/artifacts`  
☑️  Migrations confirmed on Sepolia and localhost  
☑️  TransferAgent.sol includes KYC + compliance hooks  

---

## 3. Subgraph Layer
☑️  Running locally: `http://localhost:8000/subgraphs/name/atk-subgraph`  
☑️  Confirmed queries return results:
```graphql
{ _meta { block { number } } }

☑️ Indexed events: InvestorVerified, BalanceUpdated, DocumentLinked

4. Compliance APIs

☑️ North Capital sandbox validated:

createParty ✅

performKycAml ✅

createAccount ✅

createTrade ✅
☑️ API logs stored under /src/lib/tests in dapp-standalone

5. Frontend / DApp Layer

☑️ Built with React 18 + Vite + Tailwind + Flowbite
☑️ Netlify Deployment: https://www.rblocknation.com

☑️ Investor flow aligns with BD + KYC process
☑️ Components: ShareholderPortal.tsx, ComplianceRegistry.tsx, MintControl.tsx present

6. Post-BD Tokenization Path

☑️ Extend schema for RWA (AssetMinted, AssetTransferred)
☑️ Add modules (RealEstateAsset.sol, RevenueShareAsset.sol)
☑️ Test subgraph queries after extension
☑️ Connect issuer dashboard to asset minting functions

Prepared by:
L. Sawyer — R. Block Nation
2025-11-09
