# Roadmap

Each phase ends with a **gate**. The next phase starts only when the gate is met. Dates are announced on [@sepia_sol](https://x.com/sepia_sol) as each gate gets close.

Legend: ✅ done · 🔄 in progress · ⬜ planned

## Phase 0 — Launch 🔄

| | Deliverable |
| --- | --- |
| ✅ | Brand: Sepia the cuttlefish, logo, banner |
| ✅ | Concept and token design: stealth payments, relayer, tiers, buyback and burn |
| ✅ | Website with roadmap, token page and app preview (Phantom, Solflare, Backpack) |
| ✅ | Link reservation: connect a wallet, sign once, get a Sepia ID |
| ✅ | X account [@sepia_sol](https://x.com/sepia_sol) |
| ✅ | This repository: protocol docs, Anchor program (draft), ed25519 SDK (alpha), relayer API spec |
| 🔄 | `$SEPIA` launch on pump.fun, mint address published on the site and X |
| ⬜ | Bonding curve completes, trading moves to PumpSwap |

**Gate →** `$SEPIA` graduated to PumpSwap, with the mint verified on the website and on X.

## Phase 1 — Private links ⬜

| | Deliverable |
| --- | --- |
| ⬜ | Program on devnet, public test round, then mainnet with a verified build |
| ⬜ | Admin and upgrade authority on a Squads multisig |
| ⬜ | Key setup in the app (one signature, double-signed determinism check) |
| ⬜ | Optional on-chain meta-address registration |
| ⬜ | Pay page: link + Solana Pay QR, works in any wallet, payer needs no account |
| ⬜ | SOL and USDC |
| ⬜ | Indexer for announcements; in-browser scanner with view tags |
| ⬜ | Relayer as fee payer, sanctions screening |
| ⬜ | Buyback and burn live; public burn counter on the website |

**Gate →** security review of the Sepia program and relayer finished and published; first real payments processed end to end.

## Phase 2 — Cashboxes ⬜

| | Deliverable |
| --- | --- |
| ⬜ | Holder tiers with on-chain discounts; time-weighted balances |
| ⬜ | Any SPL and Token-2022 token |
| ⬜ | Recurring payments to a Sepia link |
| ⬜ | Team cashboxes: shared links with roles for withdrawal |
| ⬜ | Auditor access: export a viewing key, read-only dashboard |
| ⬜ | CSV export for accounting; installable mobile web app |

**Gate →** external audit of the Sepia program published.

## Phase 3 — Network ⬜

| | Deliverable |
| --- | --- |
| ⬜ | Relayer staking in `$SEPIA`, slashing for censorship and invalid submissions |
| ⬜ | Open-source relayer client; app picks among staked relayers |
| ⬜ | SDK v1, a checkout button and Solana Pay integration for dApps and shops |
| ⬜ | Public stats: payments, active links, total burned |
| ⬜ | Research: ZK proof of holding, so a fresh destination still gets the tier discount |
| ⬜ | Research: confidential amounts with Token-2022, privacy pools with association sets where compliance allows |
| ⬜ | Upgrade authority revoked after audit |

**Done when →** independent staked relayers serve withdrawals alongside the Sepia relayer.
