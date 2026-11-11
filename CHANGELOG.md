# Changelog

## 0.2.0 — 2026-11-11 · Solana

Sepia moves to Solana.

- **Program:** Anchor program `sepia` replaces the EVM contracts. `send_sol` / `send_token` with `emit_cpi!` announcements; `withdraw_sol` / `withdraw_token` with the relayer as native fee payer; 1% fee ceiling as a program constant; on-chain holder tiers; fee vault PDA; buyback release; permissionless SPL burn of `$SEPIA`; withdrawals can never be paused.
- **SDK:** rewritten for ed25519. Keys from one Phantom `signMessage`; `st:sol:` meta-addresses; one-time addresses as ordinary Solana accounts; RFC 8032 signing from a raw scalar; Announcement event codec; fee quote mirroring the program. 11 tests, signatures cross-checked with OpenSSL.
- **Docs:** how it works, withdrawals, architecture, privacy model and token rewritten for Solana. Tier passes replaced by an on-chain check.
- **Relayer API:** quote returns an unsigned v0 message with the relayer as fee payer.
- **Token:** `$SEPIA` launches on pump.fun, 1B fixed supply, then PumpSwap.

## 0.1.0 — 2026-11-10

- First draft for an EVM chain: router and fee contracts, ERC-5564 secp256k1 SDK, docs and relayer spec.
