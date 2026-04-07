# 🔴 Solana RC Scanner

**Live Solana token analytics dashboard powered by the Ruslan Coefficient Framework**

🌐 **[Live Demo → ruslankarymov.github.io/rc-scanner](https://ruslankarymov.github.io/rc-scanner)**

---

## What is the Ruslan Coefficient?

The **Ruslan Coefficient (RC)** is a quantitative signal for identifying high-probability entry points in Solana memecoin trading.

```
RC = Buy Pressure × Volume Velocity × 10

Buy Pressure    = buys_h1 / (buys_h1 + sells_h1)
Volume Velocity = vol_h1 / reserve_in_usd
```

| RC Score | Signal |
|---|---|
| RC ≥ 2.5 | 🟢 **STRONG BUY** |
| RC ≥ 1.44 | 🟢 **BUY** |
| RC ≥ 0.8 | 🟡 **NEUTRAL** |
| RC < 0.8 | 🔴 **AVOID** |

> The 1.44 threshold was derived from bootstrapped cross-validation across 1,000+ trade iterations.  
> See the full statistical framework: [Ruslan Coefficient Framework →](https://github.com/ruslankarymov/solana-trading-analytics)

---

## Features

- 📡 **Live data** — GeckoTerminal API, 40 trending Solana pools, auto-refresh every 60s
- 📊 **RC Score** per token — buy pressure × volume velocity signal
- 🔍 **Filters** — sort by RC / Volume / 24h Change / Newest
- 🎯 **Signal filter** — show only BUY signals (RC > 1.44) or AVOID (RC < 0.8)
- 📋 **Grid / Table** view toggle
- 🌙 **Dark / Light mode**
- 📱 **Responsive** — works on mobile

---

## Tech Stack

- Vanilla HTML/CSS/JS — zero dependencies, zero build tools
- GeckoTerminal Public API (no key required)
- Hosted on GitHub Pages

---

## Related Projects

- 🧮 [Ruslan Coefficient Framework](https://github.com/ruslankarymov/solana-trading-analytics) — full Python statistical model with bootstrapped CV

---

*Built by [Ruslan Karymov](https://github.com/ruslankarymov) · Data & BI Analyst · Solana DeFi Analytics*
