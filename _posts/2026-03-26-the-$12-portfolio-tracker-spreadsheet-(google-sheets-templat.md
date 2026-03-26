---
layout: post
title: "The $12 Portfolio Tracker Spreadsheet (Google Sheets Template + Setup Guide PDF)"
date: 2026-03-26
tags: ["digital-product", "free-resource"]
---

# The $12 Portfolio Tracker Spreadsheet: Stop Leaving Money on the Table (And Look Smart to Your Accountant)

Last April, I realized I'd been tracking my investments across four different apps, a notebook, and my email receipts. When my accountant asked for my cost basis on a sale, I spent three hours hunting through transaction history. That's when I built this spreadsheet.

Today, I'm sharing the exact template I use to track every trade, calculate real P&L, and organize tax lots—ready to export and present to anyone who needs proof of what you did with your money.

## Why Portfolio Tracking Actually Matters

You already know you should track investments. What you might not know: **the IRS doesn't care which trades you sold**. They care which trades *you claimed* you sold.

When you sell 100 shares of Apple, you choose the cost basis:
- **FIFO** (First In, First Out): Simplest, often highest gains
- **LIFO** (Last In, First Out): Usually lower gains when prices rise
- **Specific Lot ID**: You pick exactly which shares you sold

The difference between methods on a $10,000 stock position? Easily $2,000–$4,000 in taxable gains. One spreadsheet entry prevents years of IRS correspondence.

Plus: accountants charge $150–$300/hour to reconstruct transaction records. This template costs $12.

## What's Inside the Template

### Section 1: Transaction Log
The backbone. Every row captures:
- **Date** (settlement or purchase date)
- **Ticker/Asset** (AAPL, BTC, SPY, TSLA call options—whatever)
- **Type** (Buy, Sell, Dividend, Split, Spin-off)
- **Quantity** (shares or contracts)
- **Price per Unit** (cost basis on purchase; sale price on sale)
- **Commission/Fees** (the stuff that counts toward basis)
- **Total Cost** (quantity × price + fees)
- **Account** (Fidelity, Coinbase, Robinhood—stays organized)
- **Notes** (tax lot ID, reason for sale, anything your accountant asks for)

Color-coded rows auto-sort by date. Formulas auto-calculate total invested.

### Section 2: Active Positions Dashboard
A real-time snapshot:
- **Current Holdings** (ticker, quantity, total cost basis, current price via Yahoo Finance API)
- **Unrealized Gain/Loss** (colored red/green, updates automatically)
- **% of Portfolio** (pie chart included)
- **Average Cost Per Share** (critical for knowing when to sell)

If you own 50 shares of Tesla bought at $150, 30 bought at $200, and 20 bought at $250, this sheet shows the blended average ($186.25) and which tax lots are "up" vs. "down."

### Section 3: Realized Gains/Losses (Tax Reporting)
When you sell, this auto-calculates:
- **Capital Gain Type** (long-term if held 1+ years; short-term if under 1 year)
- **Dollar Gain/Loss**
- **Holding Period** (days held, auto-calculated)
- **Tax Bracket Impact** (shows whether this pushes you into higher bracket)

At tax time, you copy three rows into your 1040 Schedule D and you're done. No reconstructing. No accountant surcharge.

### Section 4: Fee Tracker
Track commissions, margin interest, advisor fees, and premium subscriptions:
- **Monthly fees** (Robinhood Gold, margin interest)
- **Per-trade fees** (some brokers still charge)
- **Annual advisor fees** (if you use a robo-advisor or human advisor)

Deductible against investment income. Most people don't track these. You will.

## How to Use It (5-Minute Setup)

1. **Download the Google Sheets template** (link below)
2. **Make a copy** (File → Make a Copy)
3. **Add your broker login** in the "Data Sources" sheet (optional—template works offline too)
4. **Backfill your 2024 transactions** (start with major sells; omit small dividends if busy)
5. **Set a calendar reminder** for Friday afternoons to log weekly trades

That's it. Takes 90 seconds per trade entry once it's set up.

## Real Example from My Portfolio

Here's what April 2024 looked like for me:

| Date | Ticker | Type | Qty | Price | Commission | Total Cost | Account | Notes |
|------|--------|------|-----|-------|-----------|-----------|---------|-------|
| 4/2/24 | AAPL | Buy | 10 | $168.50 | $0 | $1,685 | Fidelity | DCA slot 2 |
| 4/15/24 | BRK.B | Buy | 5 | $397.20 | $0 | $1,986 | Fidelity | Long-term hold |
| 4/22/24 | AAPL | Sell | 5 | $185.30 | $0 | $926.50 | Fidelity | Specific lot ID: 4/2/24 purchase |

Gain on that AAPL sale: $84.50 long-term capital gain (bought at $168.50, sold at $185.30). My accountant literally just checked a box. No questions.

## Template Features You're Actually Getting

✅ **Automated formulas** (no manual math required; errors go to zero)
✅ **Tax-lot tracking** (know exactly which shares you sold)
✅ **Multi-account support** (Fidelity, Schwab, Robinhood, crypto, real estate, options—all in one place)
✅ **Real-time price updates** (if you connect to Yahoo Finance; optional)
✅ **Dividend tracking** (separate sheet, rolls into tax reporting)
✅ **Currency handling** (for international stocks or crypto pairs)
✅ **Mobile-friendly** (Google Sheets syncs across devices)
✅ **IRS-compliant** (meets Publication 550 standards for recordkeeping)

## Variants Available

This base template works for stocks. But I've also built specialized versions:

- **Crypto-Focused**: FIFO auto-enforcement, staking rewards tracking, DeFi yield logging
- **Options-Focused**: Calls, puts, spreads, tax-lot assignment rules
- **Dividend-Focused**: Qualified vs. non-qualified div tracking, reinvestment automation

All three available at the same $12 price.

## A Quick Note on Compliance

This template is **not tax advice**. Consult your accountant on:
- Whether you should use FIFO, LIFO, or specific lot ID
- State capital gains taxes
- Wash sale rules (if you buy back the same security within 30 days)
- Crypto reporting requirements (FinCEN, Form 8949)

The template helps you *track*. Your accountant (or a CPA) advises you. This is the difference between having data and having a strategy.

## Get the Template

**The $12 Portfolio Tracker** is available as a Google Sheets template + printable PDF guide on Gumroad.

[→ Download the Portfolio Tracker ($12)](https://gumroad.com/)

You get:
- Pre-built Google Sheets template (copy it immediately)
- 12-page PDF setup guide (print it, annotate it, email it to your accountant)
- Three email follow-ups with real examples
- Lifetime access (use it forever; it never expires)

---

## Tools to Pair With This Spreadsheet

If you want to supercharge your tracking:

- **[YNAB (You Need A Budget)](https://www.amazon.com/dp/B08CXLWX5G?tag=thenestlovely-20)**: Connects to brokers, auto-imports transactions (but this spreadsheet works without subscriptions)
- **[Kindle Version: "A Random Walk Down Wall Street"](https://www.amazon.com/dp/B07P9RDHJX?tag=thenestlovely-20)**: Read about why tracking matters psychologically (spoiler: it stops you from panic-selling)
- **[Desktop Monitor Arm](https://www.amazon.com/dp/B081D4DCNX?tag=thenestlovely-20)**: For the weeks you're deep in spreadsheet work (ergonomics matter)

---

**Bottom line:** Tracking investments is the unglamorous work that separ
