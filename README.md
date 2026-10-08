# SolSplit
![SolSplit logo](assets/logo.png)

**On-chain bill splitting and group payments that settle instantly in stablecoins**

## Overview

SolSplit lets friends, roommates, and travel groups split shared expenses and settle debts instantly using USDC on Solana. A smart contract nets multiple debts between group members into the minimum number of transactions, saving fees and time compared to manual tracking.

## Problem

Splitting group expenses across apps like Venmo or Splitwise requires manual settlement and doesn't work well across borders or currencies. Groups end up with unresolved IOUs, slow bank transfers, and confusing currency conversions.

## Solution

SolSplit is a Solana program that tracks shared expenses, nets balances automatically between all group members, and settles everyone in USDC with one click. It works globally, without requiring a bank account.

## Features (MVP)

- Create expense groups and add shared bills with photo receipts
- Automatic debt netting algorithm to minimize the number of settlement transactions
- One-click settle in USDC via a Solana wallet
- Expense history and balance dashboard per group
- QR code invite to join a group instantly

## Tech stack

- Anchor, Rust (on-chain program)
- React (frontend)
- Solana Pay (payment flow)
- USDC (settlement currency)
- Phantom Wallet Adapter (wallet connection)

## How it works

1. A user creates a group and invites members with a QR code.
2. Members add shared bills with photo receipts to the group.
3. The app computes each member's balance and runs a netting algorithm to find the minimum set of transfers.
4. Members approve a one-click settlement, which triggers USDC transfers via the Anchor program.

```
[React App] -> [Solana Pay / Wallet Adapter] -> [Anchor Program on Solana]
      |                                              |
   Add bills, view balances                 Store group & expense state
      |                                              |
  Trigger settle -----------------------------> Execute minimal USDC transfers
```

## Roadmap

- Add multi-currency support with on-chain FX via Jupiter
- Launch a mobile app with push notifications for pending debts
- Partner with travel and expense-tracking apps for integration

## Pitch

- Slides: [docs/pitch.pdf](docs/pitch.pdf)
- Script: [docs/pitch-script.md](docs/pitch-script.md)

## Team

- Name / role - placeholder
- Name / role - placeholder
- Name / role - placeholder

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://s25k1064na-sketch.github.io/solsplit/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
