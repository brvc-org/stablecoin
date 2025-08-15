# Satoshi Stablecoin

Initial idea:

$100M initial circulation, backed by Satoshi wallets 3 through 22

Stablecoin value: $1.39

71,942,446 initial coin supply

Potential ticker symbol: USBTC


STEPS:

Draft a “BRVC Stability Policy” outlining collateral type, reserve audit frequency, governance model, and compliance strategy

Build or adopt a Proof-of-Reserve tool so users can verify backing in real-time

Define your collateral and redemption mechanics — capped supply, mint & burn formulas, risk buffers

Map out governance: e.g. multisig signers, emergency pause functions, DAO thresholds

Plan AML/KYC and compliance logistics — especially given cross‑border implications

***
# USBTC on Liquid — Full Setup Checklist

## 1. Network & Infrastructure
- [ ] Set up a Liquid node or connect to a trusted provider
- [ ] Create separate wallets for issuing USBTC, operational fees, and reserves
- [ ] Implement secure key management (multi-sig recommended)
- [ ] Set up monitoring for node health and transactions

## 2. Proof-of-Reserves (PoR)
- [ ] Maintain a list of BTC reserve addresses or xpubs
- [ ] Sign messages for each reserve wallet
- [ ] Publish PoR metadata with USBTC asset
- [ ] Automate reserve vs. supply checks

## 3. Collateral & Issuance Management
- [ ] Define 1:1 collateral ratio policy
- [ ] Automate verification that reserves ≥ USBTC supply
- [ ] Set rules for peg-in and peg-out transactions
- [ ] Establish limits for minting and burning USBTC

## 4. Governance & Compliance
- [ ] Define governance for mint/burn operations
- [ ] Document audit and PoR reporting schedule
- [ ] Publish risk disclosures and disclaimers
- [ ] Keep logs of issuance, redemption, and reserve updates

## 5. Monitoring & Reporting
- [ ] Dashboard for reserves, supply, and collateral ratio
- [ ] Publish regular snapshots with blockchain proofs
- [ ] Timestamp reports on-chain
- [ ] Optional third-party audits

## 6. User & Liquidity Operations
- [ ] Pre-fund L-BTC for operational liquidity
- [ ] Enable redemption flow for USBTC to BTC or L-BTC
- [ ] Provide wallet support and user guides
- [ ] Test edge cases and failure scenarios

## 7. Security & Backup
- [ ] Secure storage of all keys (cold wallets, hardware wallets, multi-sig)
- [ ] Implement disaster recovery procedures
- [ ] Monitor for unusual or suspicious activity
