# ZAP — Financial Model: Stablecoin Retail Payment Savings

## Retailer Fee Savings Calculator

### Assumptions (Verified March 2026)
- Current card interchange rate: 2.35% average (Visa+MC credit); 1.75% blended effective rate
- USDC processing rate: 0.5-1.0% (NowPayments); using 0.75% average
- Net savings per dollar: 1.0-1.35% (conservative to full)
- Customer USDC adoption ramp: 10% → 30% → 50% over 3 years
- Chain: Solana (gas $0.00025-$0.005 per tx)

---

## Target Corporation (Verified: ~$106B revenue FY2025)

| Metric | Year 1 (10%) | Year 2 (30%) | Year 3 (50%) |
|--------|-------------|-------------|-------------|
| Annual card volume | $106B | $106B | $106B |
| USDC payment volume | $10B | $30B | $50B |
| Card fees avoided (2.5%) | $250M | $750M | $1.25B |
| USDC processing cost (0.75%) | $75M | $225M | $375M |
| **Net savings** | **$175M** | **$525M** | **$875M** |
| Float income (4% APY on avg balance) | $20M | $60M | $100M |
| **Total annual benefit** | **$195M** | **$585M** | **$975M** |
| **Cumulative 3-year savings** | | | **$1.755B** |

---

## Costco (Verified: $275.2B revenue FY2025)

| Metric | Year 1 (10%) | Year 2 (30%) | Year 3 (50%) |
|--------|-------------|-------------|-------------|
| Annual card volume | $275B | $275B | $275B |
| USDC payment volume | $24B | $72B | $120B |
| Card fees avoided (2.5%) | $600M | $1.8B | $3.0B |
| USDC processing cost (0.75%) | $180M | $540M | $900M |
| **Net savings** | **$420M** | **$1.26B** | **$2.1B** |
| Float income (4% APY) | $48M | $144M | $240M |
| **Total annual benefit** | **$468M** | **$1.404B** | **$2.34B** |
| **Cumulative 3-year savings** | | | **$4.212B** |

---

## Home Depot (Verified: $164.7B revenue FY2025)

| Metric | Year 1 (10%) | Year 2 (30%) | Year 3 (50%) |
|--------|-------------|-------------|-------------|
| Annual card volume | $165B | $165B | $165B |
| USDC payment volume | $15B | $45B | $75B |
| Card fees avoided (2.5%) | $375M | $1.125B | $1.875B |
| USDC processing cost (0.75%) | $112.5M | $337.5M | $562.5M |
| **Net savings** | **$262.5M** | **$787.5M** | **$1.3125B** |
| Float income (4% APY) | $30M | $90M | $150M |
| **Total annual benefit** | **$292.5M** | **$877.5M** | **$1.4625B** |
| **Cumulative 3-year savings** | | | **$2.6325B** |

---

## Walmart (Verified: $706.4B revenue FY2026 — reference, already has OnePay/Zerohash)

| Metric | Year 1 (10%) | Year 2 (30%) | Year 3 (50%) |
|--------|-------------|-------------|-------------|
| Annual card volume | $706B | $706B | $706B |
| USDC payment volume | $40B | $120B | $200B |
| Card fees avoided (2.5%) | $1.0B | $3.0B | $5.0B |
| USDC processing cost (0.75%) | $300M | $900M | $1.5B |
| **Net savings** | **$700M** | **$2.1B** | **$3.5B** |
| Float income (4% APY) | $80M | $240M | $400M |
| **Total annual benefit** | **$780M** | **$2.34B** | **$3.9B** |
| **Cumulative 3-year savings** | | | **$7.02B** |

---

## Your Revenue as Deal Closer

### Per-Account Revenue Model

| Revenue Stream | Per Account (Year 1) | Per Account (Year 2+) |
|---------------|---------------------|----------------------|
| Implementation/consulting fee | $500K - $2M | $0 (one-time) |
| Rev-share (15% of net savings) | $0 (pilot year) | $26M - $130M |
| SaaS platform fee | $100K | $200K |
| Circle partner referral | $50K - $200K | $100K - $500K |
| **Total per account** | **$650K - $2.4M** | **$26.3M - $130.7M** |

### Portfolio Revenue (Multiple Accounts)

| Scenario | Year 1 | Year 2 | Year 3 |
|----------|--------|--------|--------|
| **Conservative** (2 pilots) | $1.3M | $10M | $30M |
| **Base case** (5 accounts) | $5M | $25M | $75M |
| **Aggressive** (10 accounts) | $12M | $60M | $200M |

---

## Restaurant Pilot Economics

### Monthly comparison (your restaurant)

| Metric | Card Payments | USDC Payments | Savings |
|--------|--------------|---------------|---------|
| Monthly card volume | $50,000 | — | — |
| Card processing fee (2.5%) | $1,250 | — | — |
| USDC processing fee (0.5%) | — | $250 | — |
| **Monthly savings** | | | **$1,000** |
| **Annual savings** | | | **$12,000** |

Assumes 100% of volume shifts to USDC. At realistic 20-30% adoption:

| Adoption Rate | Monthly USDC Volume | Monthly Savings | Annual Savings |
|--------------|--------------------:|----------------:|---------------:|
| 10% | $5,000 | $100 | $1,200 |
| 20% | $10,000 | $200 | $2,400 |
| 30% | $15,000 | $300 | $3,600 |
| 50% | $25,000 | $500 | $6,000 |
| 100% | $50,000 | $1,000 | $12,000 |

---

## Customer Economics

### What it costs a customer to use USDC

| Action | Cost | Notes |
|--------|------|-------|
| Download wallet app | $0 | Trust Wallet, Coinbase, etc. |
| Load USDC via ACH | $0 | Free bank transfer |
| Load USDC via debit card | 1-1.5% | ~$1 on $100 load |
| Send USDC to pay bill | $0.00025-$0.005 | Solana gas (cheapest); Tron $0.81-$3.86; Ethereum L2 $0.05-$0.30 |
| **Total customer cost (ACH + Solana)** | **< $0.01** | Essentially free |
| **Total customer cost (card load)** | **$1.01-$1.50** | Still cheaper than retailer's card fees |

### Customer incentive math

If retailer offers 2% discount for USDC payments:
- Customer saves $2 on $100 purchase
- Retailer still saves $0.75 net (2.5% card fee - 0.75% USDC fee - 1% discount = 0.75%)
- Both sides win

---

## Break-Even Analysis

### Your startup costs vs. revenue

| Investment | Amount |
|-----------|--------|
| Restaurant pilot setup | $1,000 |
| Circle partner certification | $2,000 |
| Legal (LLC + contracts) | $10,000 |
| Website + pitch materials | $5,000 |
| Travel (first 6 months) | $10,000 |
| Contract developer | $20,000 |
| **Total investment** | **$48,000** |

**Break-even:** First enterprise pilot contract ($500K+) covers all startup costs 10x over.

**Time to break-even:** 6-12 months (time to close first enterprise deal).
