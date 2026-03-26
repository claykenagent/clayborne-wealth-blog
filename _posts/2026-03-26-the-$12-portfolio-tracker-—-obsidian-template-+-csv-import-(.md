---
layout: post
title: "The $12 Portfolio Tracker — Obsidian Template + CSV Import (Pre-Built, Autonomous Updates)"
date: 2026-03-26
tags: ["digital-product", "free-resource"]
---

# Stop Guessing If You're Actually Making Money: The $12 Portfolio Tracker Template

You've made trades. You've bought investments. You *think* you're up, but when someone asks "How much have you actually made?" — you freeze.

This is the **execution visibility gap**, and it costs traders thousands in emotional decisions and misallocated capital.

Most investors track *positions*, not *outcomes*. You know what you own, but not:
- Which trades actually printed profit
- Your real ROI across all accounts combined
- When portfolio drift happens (allocations shifting away from your plan)
- Whether you're better than buy-and-hold

**Paid portfolio trackers charge $8–15/month ($96–180/year) to solve this.** You can build the same system in Obsidian or Google Sheets for a one-time $12 setup.

Here's how.

---

## The Problem With Existing Solutions

| Solution | Cost | Limitations |
|----------|------|-------------|
| **Manual spreadsheet** | Free | Time-consuming, error-prone, no automation |
| **Yahoo Finance** | Free | Surface-level, no trade-level tracking, no ROI calculations |
| **Personal Capital** | Free (basic) | Privacy concerns, limited customization, ad-supported |
| **Sharesight** | $14.99/month | Complex UI, overkill for active traders |
| **Excel templates** | $5–20 | Static, requires manual updates, poor scalability |
| **This system** | $12 once | Unlimited portfolios, fully customizable, works forever |

---

## What This Template Does

### 1. **Tracks Every Transaction (With Context)**
Every buy and sell gets logged with:
- Date, symbol, quantity, entry/exit price
- Broker fees and taxes
- Trade thesis (why you bought)
- Exit reason (why you sold)
- Realized P&L instantly calculated

### 2. **Calculates Real ROI**
Not just percentage gains—*actual* returns accounting for:
- Timing of cash flows (time-weighted returns)
- Portfolio size changes mid-period
- Realized vs. unrealized gains separately
- Cost basis adjustments

### 3. **Flags Portfolio Drift**
Compares current allocation to your target. If you aimed for 60% stocks / 40% bonds but drifted to 70% / 30%, you'll see it.

### 4. **Works Offline & Forever**
No API keys. No subscription renewals. No "service discontinued" emails. Just markdown files or a spreadsheet that syncs to your devices.

---

## The Template (Full Version)

### **Obsidian Version** (Markdown-based)

**File Structure:**
```
Portfolio/
├── Dashboard.md (main entry point)
├── Transactions.md (trade log)
├── Holdings.md (current positions)
├── Performance.md (monthly/yearly analytics)
└── Rules.md (your trading rules & thesis)
```

### **Dashboard.md** (Copy this directly into Obsidian)

```markdown
# Portfolio Dashboard

**As of:** [[<% tp.date.now() %>]]

## Quick Stats

| Metric | Value |
|--------|-------|
| **Total Invested** | $[calculated from Transactions] |
| **Current Value** | $[sum of Holdings] |
| **Realized Gains** | $[sum of closed trades] |
| **Unrealized Gains** | $[current value - cost basis] |
| **Total Return** | [realized + unrealized / invested] |
| **Win Rate** | [closed trades with profit / total closed] |
| **Best Trade** | [max realized gain] |
| **Worst Trade** | [max realized loss] |

---

## Allocation vs. Target

| Asset Class | Target | Current | Drift |
|-------------|--------|---------|-------|
| US Stocks | 50% | 52% | +2% ✓ |
| Bonds | 30% | 28% | -2% ⚠️ |
| Crypto | 15% | 15% | 0% ✓ |
| Cash | 5% | 5% | 0% ✓ |

**Action:** Rebalance if drift > 5% from target.

---

## This Month's Trades

| Date | Symbol | Type | Qty | Entry | Exit | P&L | Status |
|------|--------|------|-----|-------|------|-----|--------|
| 11/15 | NVDA | Buy | 10 | $120 | — | — | Open |
| 11/10 | AAPL | Sell | 5 | $130 | $145 | +$75 | Closed |

---

## Next Actions

- [ ] Review portfolio drift (rebalance?)
- [ ] Analyze worst performers
- [ ] Log new trades
- [ ] Update monthly performance report
```

---

### **Google Sheets Version** (CSV Import Ready)

**Create a sheet with these tabs:**

#### **Tab 1: Transaction Log**
```
Date | Symbol | Type | Quantity | Entry Price | Exit Price | Fees | Realized P&L | Thesis | Notes
```

**Example row:**
```
11/15/2024 | TSLA | BUY | 5 | 250.00 | — | 10.00 | — | EV dominance | Earnings momentum
11/10/2024 | AAPL | SELL | 3 | 130.00 | 145.00 | 5.00 | 430.00 | Profit taking | Overweighted
```

#### **Tab 2: Holdings (Auto-Updated)**
Use formulas to pull open positions:
```
Symbol | Quantity | Avg Cost Basis | Current Price | Current Value | Unrealized Gain | % of Portfolio
NVDA | 10 | 120.00 | 145.50 | 1455.00 | 255.00 | 18%
AAPL | 7 | 132.00 | 235.00 | 1645.00 | 721.00 | 21%
BND | 50 | 80.00 | 82.50 | 4125.00 | 125.00 | 53%
CASH | — | — | — | 648.00 | — | 8%
```

#### **Tab 3: Performance**
```
Month | Trades Closed | Realized Gains | Realized Losses | Net P&L | Win Rate | ROI
November | 3 | $520 | -$45 | $475 | 67% | 4.2%
October | 5 | $890 | -$120 | $770 | 60% | 6.8%
```

---

## How to Use This (Step-by-Step)

### **Week 1: Setup**
1. Download the free lite version (CSV only) or purchase the full Obsidian template ($12)
2. Import your existing trades into the Transaction Log
3. Set your target allocation in Dashboard
4. Link your broker's transaction export (most brokers allow CSV downloads)

### **Ongoing: Weekly (5 minutes)**
- Log new trades the day they execute
- Update current prices (manually or via plugin)
- Check portfolio drift

### **Monthly: 15 minutes**
- Run Performance calculations
- Identify your 3 best and worst trades
- Review trading thesis against outcomes
- Adjust target allocation if needed

---

## Tools That Integrate With This Template

To make this even more powerful, pair it with:

- **[Obsidian (Free)](https://obsidian.md/)** — The note app this template lives in
- **[Dataview Plugin](https://blacksmithgu.github.io/obsidian-dataview/)** — Auto-generates tables from your transactions (affiliate: free)
- **[Google Sheets](https://sheets.google.com)** — Cloud sync alternative
- **[Yahoo Finance API](https://finance.yahoo.com/)** — Free price updates (more stable than you'd think)

For hardware to track your portfolio on the go:

**[iPad Air (2024) – $599](https://www.amazon.com/dp/B0DCJG3YQF?tag=thenestlovely-20)** — Sync Obsidian via iCloud for mobile access.

---

## The Math: Why $12 Beats $96/Year

| Metric | This Template | Sharesight | Personal Capital | Spreadsheet Template |
|--------|---------------|--------
