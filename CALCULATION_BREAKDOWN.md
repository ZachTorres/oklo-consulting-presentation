# OKLO PRESENTATION - COMPLETE CALCULATION BREAKDOWN

## Overview
This document traces **every number** in the "OKLO - From Reactors to Revenue" presentation and shows where the calculations come from.

---

## SLIDE 2: Market Opportunity
### Numbers Presented:
- **80+ startups** need regulatory help
- **~$4B+** in total funding

### Calculation Source:
- **80+ startups**: This appears to be a market research figure representing advanced nuclear reactor startups
- **$4B+ funding**: Sum of major startup funding rounds mentioned in Slide 3 script:
  - TerraPower: $1.4B
  - X-energy: $1.0B
  - Kairos: $0.629B
  - Newcleo: $0.677B
  - **Total from these 4 alone: $3.706B** ≈ **$4B+ claimed**

**⚠️ ISSUE**: The presentation only shows 4 companies totaling ~$3.7B, not $4B+. The claim needs additional companies or is rounded up.

---

## SLIDE 4: What Startups Need
### Numbers Presented:
- **10+ years** of licensing timeline
- **$50M+** in regulatory costs
- **Zero** reactor experience

### Calculation Source:
These are **industry benchmarks**, not calculations:
- **10+ years**: Based on NuScale's timeline (referenced in speaker script - took years for approval)
- **$50M+**: Estimated regulatory compliance cost for advanced reactors
- **Zero experience**: Qualitative statement (most new startups haven't submitted NRC applications)

**⚠️ NO SOURCE PROVIDED** in presentation for these specific numbers.

---

## SLIDE 5: Oklo's Knowledge Asset
### Numbers Presented:
- **2020**: First NRC Application
- **2022**: NRC Rejection
- **2025**: Current year
- **$140M** Knowledge Asset / Expertise

### Calculation Source:
- **Timeline**: Historical facts (Oklo's actual NRC filing dates)
- **$140M valuation**: This is the **TARGET REVENUE BY 2030**, not an asset valuation
  - **IMPORTANT**: This number is recycled from Slide 6 total revenue target
  - It's presented as "knowledge asset" but really means "revenue potential"

**⚠️ MISLEADING**: $140M is revenue projection, NOT an asset valuation.

---

## SLIDE 6: Three Revenue Streams (2030 TARGETS)
### Numbers Presented:
- **$75M** - Licensing & Regulatory
- **$42M** - Safety & Simulation
- **$23M** - Fuel Cycle
- **Total: $140M** (2030 Annual Revenue Targets)

### Calculation Check:
```
$75M + $42M + $23M = $140M ✓ (CORRECT)
```

### Calculation Source:
**WHERE DO THESE NUMBERS COME FROM?**

These appear to be **ASSUMPTIONS** based on:

#### Licensing & Regulatory ($75M):
- **Script mentions**: "$50-80M/yr target" (per CLAUDE.md)
- **Mid-point chosen**: $75M

#### Safety & Simulation ($42M):
- **Script mentions**: "$30-50M/yr target" (per CLAUDE.md)
- **Chosen value**: $42M (exactly matches EBITDA on Slide 9 - suspicious?)

#### Fuel Cycle ($23M):
- **Script mentions**: "$15-25M/yr target" (per CLAUDE.md)
- **Chosen value**: $23M

**⚠️ ISSUE**: These targets are NOT shown to be derived from client counts, pricing, or market sizing. They appear to be **arbitrary targets within stated ranges**.

---

## SLIDE 7: Market Opportunity Funnel
### Numbers Presented:
- **$6.2B** - Global TAM (Total Addressable Market)
- **$1.9B** - U.S. Serviceable Market
- **$570M** - Our Target (30% market share)

### Calculation Source:

#### $6.2B Global TAM:
**Implied formula:**
```
80 startups × Average lifetime licensing spend = $6.2B
$6.2B ÷ 80 = $77.5M per startup over their lifetime
```

**Question**: Where does $77.5M/startup come from?
- Slide 4 says "$50M+ in regulatory costs"
- But $6.2B ÷ 80 = $77.5M (higher than $50M)
- **Possible**: Includes consulting beyond just regulatory (safety, fuel cycle)

#### $1.9B U.S. Market:
```
$1.9B ÷ $6.2B = 30.6% of global market
```
**Assumption**: ~30% of startups are U.S.-based or in allied nations

#### $570M Target:
```
$570M ÷ $1.9B = 30%
```
**Stated explicitly**: "30% market share by 2030"

**⚠️ CRITICAL ISSUE**: The formula assumes:
- All 80 startups will spend their full licensing budgets
- All will hire consultants (not do it in-house)
- Oklo can capture 30% market share
- No competition from established nuclear consulting firms

---

## SLIDE 8: 5-Year Growth Chart
### Numbers Presented (Chart Data):

| Year | Licensing | Safety | Fuel Cycle | **Total** |
|------|-----------|--------|------------|-----------|
| 2026 | $3.0M     | $1.0M  | $0.5M      | **$4.5M** |
| 2027 | $15.0M    | $6.0M  | $2.0M      | **$23.0M** |
| 2028 | $38.0M    | $20.0M | $9.0M      | **$67.0M** |
| 2029 | $65.0M    | $35.0M | $18.0M     | **$118.0M** |
| 2030 | $75.0M    | $42.0M | $23.0M     | **$140.0M** |

### Calculation Check:
```
2026: $3.0 + $1.0 + $0.5 = $4.5M ✓
2027: $15.0 + $6.0 + $2.0 = $23.0M ✓
2028: $38.0 + $20.0 + $9.0 = $67.0M ✓
2029: $65.0 + $35.0 + $18.0 = $118.0M ✓
2030: $75.0 + $42.0 + $23.0 = $140.0M ✓
```

### Growth Rates:
```
2026→2027: $4.5M → $23M = 411% growth
2027→2028: $23M → $67M = 191% growth
2028→2029: $67M → $118M = 76% growth
2029→2030: $118M → $140M = 19% growth
```

### Calculation Source:
**HOW WERE THESE YEAR-BY-YEAR NUMBERS CALCULATED?**

Looking at Slide 10 client counts:
- 2026: 3 clients → $4.5M revenue
- 2027: 20 clients → $23M revenue
- 2028: 40 clients → $67M revenue
- 2030: 100+ clients → $140M revenue

**Implied revenue per client:**
```
2026: $4.5M ÷ 3 = $1.5M per client
2027: $23M ÷ 20 = $1.15M per client
2028: $67M ÷ 40 = $1.675M per client
2030: $140M ÷ 100 = $1.4M per client
```

**⚠️ ISSUE**: Revenue per client is INCONSISTENT:
- Should increase over time as clients buy more services
- Or decrease as you add smaller clients
- But it bounces around: $1.5M → $1.15M → $1.675M → $1.4M

**CONCLUSION**: These numbers appear to be **WORKED BACKWARDS** from the $140M target, not calculated from bottom-up client/pricing assumptions.

---

## SLIDE 9: Profitability
### Numbers Presented:
- **$42M EBITDA** by 2030
- **35-40% margin**

### Calculation Check:
```
If Revenue = $140M and EBITDA = $42M:
Margin = $42M ÷ $140M = 30%

But slide claims 35-40% margin!
```

**⚠️ DISCREPANCY**:
- Claimed margin: 35-40%
- Calculated margin: 30%
- **At 35% margin**: $140M × 35% = $49M EBITDA (not $42M)
- **At 40% margin**: $140M × 40% = $56M EBITDA (not $42M)
- **Actual margin**: $42M ÷ $140M = **30%**

**CONTRADICTION FOUND**: The math doesn't match the claim.

### Calculation Source:
From speaker script (create_team_script.py):
- Claims "35-40% margin—exceptional for professional services"
- But shows $42M EBITDA on $140M revenue = 30% margin

**⚠️ MAJOR ERROR**: Either the EBITDA is wrong or the margin % is wrong.

---

## SLIDE 10: Client Roadmap
### Numbers Presented:
- **2026**: 3 clients (Launch)
- **2027**: 20 clients (Scale)
- **2028**: 40 clients (Expand)
- **2030**: 100+ clients (Lead)

### Calculation Source:
**Missing**: 2029 client count (needed to calculate 2029 revenue on Slide 8)

**Growth pattern:**
```
2026→2027: 3 → 20 = 567% growth
2027→2028: 20 → 40 = 100% growth
2028→2030: 40 → 100 = 150% growth (over 2 years)
```

These appear to be **ASPIRATIONAL TARGETS**, not calculated from:
- Sales pipeline
- Market share math
- Conversion rates
- Sales capacity

**⚠️ MISSING LOGIC**: No explanation of HOW Oklo will acquire these clients.

---

## SLIDE 11: The Investment
### Numbers Presented:
- **$2M** initial investment
- **$140M** by 2030
- **70x return** in 4 years

### Calculation Check:
```
Return = $140M ÷ $2M = 70x ✓ (CORRECT)
```

**But wait...**
- $140M is ANNUAL REVENUE, not profit
- $42M is EBITDA (closer to actual return)
- **Actual return on EBITDA**: $42M ÷ $2M = **21x** (not 70x)

**⚠️ MISLEADING**: 70x return uses revenue, not profit. Investors care about profit/EBITDA multiple.

### Calculation Source:
From speaker script:
- $2M covers hiring 3-5 consultants, software, marketing, legal setup
- Breakeven in Year 2 (2027)

**Question**: If $2M investment gets you to $4.5M revenue in 2026, how do you reach $23M in 2027?
- **Implied**: Need to reinvest profits or raise more capital (not mentioned)

---

## SUMMARY: WHERE THE NUMBERS REALLY COME FROM

### Hard Data (Verifiable):
1. **80+ startups**: Market research data
2. **$4B funding**: Sum of known funding rounds (TerraPower, X-energy, etc.)
3. **10+ years licensing**: NRC historical timelines
4. **Oklo 2020/2022 dates**: Public record

### Calculated (Internally Consistent):
1. **$140M total revenue**: $75M + $42M + $23M ✓
2. **70x return**: $140M ÷ $2M ✓
3. **30% market share**: $570M ÷ $1.9B ✓

### Assumptions (NOT Derived from Data):
1. **$75M, $42M, $23M revenue targets**: Chosen within stated ranges, no bottom-up calculation shown
2. **$6.2B global TAM**: Assumes $77.5M per startup lifetime spend (not explained)
3. **Client counts (3, 20, 40, 100)**: Aspirational targets, no acquisition model shown
4. **Year-by-year revenue**: Appears worked backwards from $140M target

### Errors Found:
1. **Margin miscalculation**: Claims 35-40% but shows 30% ($42M ÷ $140M)
2. **ROI framing**: Uses revenue multiple (70x) instead of profit multiple (21x)
3. **$140M as "asset"**: Revenue potential mislabeled as asset valuation on Slide 5

---

## WHAT'S MISSING: The Real Calculations Should Be:

### Bottom-Up Revenue Model:
```
Revenue = (# of clients) × (avg contract value) × (services per client)

Where:
- Avg contract value = $X per engagement
- Services per client = Y engagements/year
- Retention rate = Z%
```

**None of this is shown.**

### Market Share Calculation:
```
Market share % = (Oklo client count ÷ Total startup count) × (Oklo avg deal ÷ Market avg deal)
```

**Not provided.**

### Pricing Strategy:
```
Hourly rate: $250-500/hour (mentioned in script)
Annual contract size: ?
Licensing project: ?
Safety analysis: ?
```

**Not broken down.**

---

## CONCLUSION

### The presentation uses THREE types of numbers:

1. **Real market data** (80 startups, $4B funding, NRC timelines)
2. **Target-based assumptions** ($140M goal broken into $75M/$42M/$23M)
3. **Reverse-engineered projections** (year-by-year growth designed to hit the target)

### The core issue:
**The $140M target appears to be chosen first, then all other numbers are derived to support it.**

The presentation does NOT show:
- ✗ How to price services
- ✗ How to acquire clients
- ✗ Why 30% market share is achievable
- ✗ What competitors charge
- ✗ Bottom-up revenue build from pricing × volume
- ✗ Customer acquisition cost
- ✗ Sales cycle length
- ✗ Win rate assumptions

### What you'd need to validate these numbers:
1. **Pricing research**: What do nuclear consulting firms charge?
2. **Competitive analysis**: Who else offers these services?
3. **Customer interviews**: Would startups pay these amounts?
4. **Sales model**: CAC, LTV, conversion rates, sales cycle
5. **Capacity model**: How many clients can Oklo's team handle?
6. **Market share justification**: Why would Oklo win 30%?

**Bottom line**: The numbers are internally consistent but lack bottom-up justification from market data, pricing research, or customer validation.
