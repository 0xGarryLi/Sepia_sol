# Security policy

## Status

Everything in this repository is **pre-audit and not deployed**. There is no bug bounty yet; one will be announced with the Phase 1 mainnet deployment.

## Reporting a vulnerability

- Do **not** open a public issue for security problems.
- Use GitHub's **private vulnerability reporting** on this repository (Security → Report a vulnerability), or DM [@sepia_sol](https://x.com/sepia_sol) asking for a secure channel.
- Include: affected file and function, impact, and steps to reproduce (a failing `anchor test` or SDK test is ideal).

We aim to acknowledge reports within 72 hours.

## Scope

| In scope | Out of scope |
| --- | --- |
| `programs/sepia/**` | Third-party programs (pump.fun, PumpSwap, Jupiter, SPL) |
| `sdk/src/**` (key derivation, stealth math, scalar signing, event codec) | The website's marketing pages |
| Relayer API design in `relayer/` | Social engineering, phishing of users |

Areas we especially want eyes on: account validation in `withdraw_*`, the fee arithmetic in `split_fees`, PDA signing in the buyback and burn paths, and `signWithScalar` nonce derivation.

## Known design trade-offs (not vulnerabilities)

- Tier discounts require withdrawing to the wallet that holds `$SEPIA`, which links that withdrawal to that wallet. Documented in [docs/privacy-model.md](docs/privacy-model.md#tiers-and-privacy).
- A flash-borrowed `$SEPIA` balance can claim a tier for one transaction. The most it saves is the protocol fee (≤ 0.5%).
- Payer address, amount and time are public by design.

## Scam warning

The only `$SEPIA` mint is the one on the official website and on @sepia_sol. Sepia will never DM you an address, run a presale, or ask for a seed phrase or the Sepia key signature outside the official site.
