# Roles & Oversight (WSP Mapping)

This page maps platform roles and controls to broker-dealer Written Supervisory Procedures (WSP).

## Parties
- **Broker-Dealer (BD):** Supervisory principal(s), books & records, marketing review, exception handling.
- **R. Block Nation (Tech Partner / Issuer for POC):** Front-end build, integrations, on-platform comms.
- **KoreConX:** KYC/AML/CIP workflow, cap table, TA.
- **North Capital (Escrow):** Subscriptions, funds flow, reconciliation, returns.
- **SettleMint:** Node/orchestration for contract deployment & transactions.

## Key Controls
- **UI / Offering Pages:** BD pre-clears templates; all investor interactions occur on-platform; external ads link back.
- **Marketing Review:** BD reviews and archives all communications; independent principal for conflict scenarios.
- **KYC/AML/CIP:** Performed in Kore; statuses fed to BD; exceptions escalated prior to closing.
- **Funds / Escrow:** NC maintains escrow; BD receives periodic feeds/recons; close only when conditions met.
- **Books & Records (17a-4):** BD retains official records; platform data exported/archived per policy.
- **Change Management:** Version tags (git), release notes, rollback plan; BD notified of material changes.
- **Smart Contract:** Verified on Etherscan (Sepolia); deployment tagged in repo; ABI + address recorded.

## Initial Role Grants (POC)
- **DEFAULT_ADMIN_ROLE:** Deployer (temporary, to be replaced by multisig/custodian).
- **ADMIN_ROLE:** BD-designated admin for pause/unpause and revenue distribution.
- **KORE_OPERATOR_ROLE:** Kore operations service account for funding windows / mint ops.

> All permissions reviewed by BD prior to go-live. Conflicts disclosed when RBN is both tech partner and issuer.
