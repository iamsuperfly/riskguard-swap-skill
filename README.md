# RiskGuard Swap Skill

**Build X Season 2 Hackathon – Skills Arena Entry**  
**Author:** Superfly (@killsh0tx)  
**GitHub:** https://github.com/iamsuperfly/riskguard-swap-skill

A lightweight, reusable **safety-first swap skill** for any AI agent on X Layer.

Before any swap it:
1. Checks risk using Onchain OS skills (`okx-security` + `okx-dex-market`)
2. Only executes the swap if risk is low (`okx-dex-swap`)

### How to install in any agent (Cursor, Claude, etc.)
```bash
npx skills add https://github.com/iamsuperfly/riskguard-swap-skill
