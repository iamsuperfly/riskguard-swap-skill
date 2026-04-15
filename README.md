# RiskGuard Swap Skill

A lightweight, reusable **safety-first swap skill** for any AI agent on X Layer.

Before executing any swap it:
1. Checks risk using Onchain OS skills (okx-security + okx-dex-market)
2. Evaluates conditions in real-time
3. Executes swap only if risk is low (okx-dex-swap)

### How to install in any AI agent
```bash
npx skills add https://github.com/iamsuperfly/riskguard-swap-skill
```

### How to test with AI agents (Claude, Cursor, etc.)
Open your AI agent and type a prompt like:

> Use RiskGuard to swap 1.5 USDC to USDT on X Layer if the risk is low

The agent will automatically:
- Run risk checks first
- Only swap if everything is safe

### Onchain Proof
**Transaction Hash:** `0xe7eb7632d7c51391f2b4ed9ac142074a4248cdc125a0b09ae946213db334c187`  
**Details:** 1.5 USDC → USDT swap on X Layer Mainnet (done in OKX Wallet)  
**Explorer:** https://www.oklink.com/x-layer/tx/0xe7eb7632d7c51391f2b4ed9ac142074a4248cdc125a0b09ae946213db334c187

### Local Test (optional)
```bash
node test-riskguard.js
```

> **Build X Season 2 Hackathon – Skills Arena Entry**  
**Author:** Superfly (@killsh0tx)
