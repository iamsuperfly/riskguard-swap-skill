---
name: riskguard-swap
version: 1.0
description: Risk-aware token swap skill for X Layer. Checks security first using okx-security, then executes safe swap via okx-dex-swap.
author: iamsuperfly
tags: [swap, risk, security, dex, xlayer]
requires: [okx-security, okx-dex-swap, okx-dex-market]
---

# RiskGuard Swap Skill

Type: Composite Skill
Chain: X Layer Mainnet

Purpose
Prevent bad swaps by running risk detection before execution.

How agents call this skill
Use RiskGuard to swap [amount] [fromToken] to [toToken] if risk is low

Internal flow
1. okx-security.check returns risk score
2. If risk score less than 30 then okx-dex-swap.execute
3. Returns tx hash

This skill is fully compatible with Onchain OS. Install once with npx skills add and use forever.
