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
# Proof-of-Reserves (PoR) Checklist for USBTC on Liquid

- [ ] **Publish Reserve Addresses**
  - Maintain a list of Bitcoin addresses (or xpubs) holding BTC reserves.
  - Ensure public verifiability via any Bitcoin block explorer.
  - Optional: Engage a 3rd-party auditor for ownership confirmation.

- [ ] **Signed Message Verification**
  - Create signed messages for each reserve wallet, e.g.:
    ```
    This wallet proves control of BTC reserves for USBTC as of YYYY-MM-DD.
    ```
  - Make signed messages publicly accessible for verification.

- [ ] **Link Reserves to USBTC Issuance**
  - Include in Liquid asset metadata:
    - URL to BTC reserve addresses list.
    - Latest signed PoR message.
    - Peg-in transaction IDs (if part of reserves are in L-BTC).

- [ ] **Maintain 1:1 Collateral Ratio**
  - Track that BTC in reserve addresses ≥ USBTC in circulation.
  - Use scripts or API feeds to monitor the ratio in real-time.

- [ ] **Publish Periodic Snapshots**
  - Produce weekly or monthly PoR reports.
  - Include blockchain proofs and USBTC circulating supply screenshots from Liquid explorer.
  - Timestamp reports on-chain (OP_RETURN in BTC or Liquid).

- [ ] **Optional Peg-in for Liquidity**
  - Peg a small portion of BTC to L-BTC for operational liquidity.
  - Keep the majority of reserves on the main BTC chain to preserve BTC-native backing.
  - Enable USBTC issuance without moving all holdings.
