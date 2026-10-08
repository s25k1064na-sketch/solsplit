# SolSplit

_On-chain bill splitting and group payments that settle instantly in stablecoins_

## Summary

SolSplit lets friends, roommates, or travel groups split expenses and settle debts instantly using USDC on Solana, removing the friction of IOUs and manual tracking. A smart contract nets multiple debts between group members into the minimum number of transactions, saving fees and time.

## Target users

Groups of friends, roommates, travelers who share expenses regularly

## Problem

Splitting group expenses across apps like Venmo or Splitwise requires manual settlement and doesn't work well across borders or currencies.

## Solution

A Solana program that tracks shared expenses, nets balances automatically, and settles in USDC with one click, working globally without bank accounts.

## MVP features

- Create expense groups and add shared bills with photo receipts
- Automatic debt netting algorithm to minimize number of settlement transactions
- One-click settle in USDC via Solana wallet
- Expense history and balance dashboard per group
- QR code invite to join a group instantly

## Chains

Solana

## Tech

Anchor, Rust, React, Solana Pay, USDC, Phantom Wallet Adapter

## Category

Payments

## Why now

Stablecoin payments are becoming mainstream and Solana's low fees make micro-settlements between friends economically viable for the first time.

## Roadmap

- Add multi-currency support with on-chain FX via Jupiter
- Launch mobile app with push notifications for pending debts
- Partner with travel and expense-tracking apps for integration
