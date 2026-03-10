# ZAP — Proof of Concept Test Plan

## Why You Need This Before Pitching Enterprise

No Fortune 500 company will hand you a pilot based on a pitch deck alone. You need to walk in with:

1. **A working product** they can see and touch
2. **Real transaction data** from a live environment
3. **Measured fee savings** with actual numbers
4. **Customer feedback** showing people will use it

This document is your roadmap to build that proof before you ever pitch Costco or Target.

---

## PHASE 1: YOUR RESTAURANT (Weeks 1-4)

You already own a restaurant. This is your testing lab. No permission needed, no contracts, no gatekeepers.

### Step 1: Set Up USDC Payment Acceptance

**What to do:**
- Create a business account on NowPayments (nowpayments.io) — 0.5% fee
- Generate a USDC payment QR code for your restaurant
- Set up auto-conversion to USD → direct deposit to your bank
- Alternative: Set up a Circle account (circle.com) for direct USDC acceptance

**What you'll have:** A working payment endpoint that accepts USDC and deposits dollars in your bank.

**Time:** 1-2 days

### Step 2: Create the Customer Experience

**What to build:**
- A simple one-page "How to Pay with [Restaurant Name] Pay" guide
- Step-by-step: Download wallet (Phantom or Coinbase Wallet) → Link bank → Buy USDC → Scan QR to pay
- Print QR code table tents or counter signs
- Train your staff to explain it in 30 seconds

**The pitch to customers:**
"Pay with [Restaurant Name] Pay and get 5% off your order today."

**Time:** 2-3 days

### Step 3: Run It Live for 30 Days

**What to track (this is your data for the pitch):**

| Metric | How to Measure |
|--------|---------------|
| Total USDC transactions | NowPayments or Circle dashboard |
| Total USD value processed | Dashboard |
| Processing fees paid | Dashboard (should be ~0.5%) |
| Card transactions same period | Your existing POS/processor statement |
| Card processing fees paid | Your processor statement |
| Fee savings (USDC vs card) | Card fee % minus USDC fee % |
| Customer adoption rate | USDC transactions ÷ total transactions |
| Customer setup time | Time it yourself with 5 customers |
| Customer satisfaction | Ask them — simple 1-5 rating |
| Settlement speed | Time from payment to bank deposit |

**What you'll have after 30 days:**
- "We processed $X,XXX in USDC payments over 30 days"
- "Our processing fee was 0.5% vs 2.35% on cards — an 80% reduction"
- "X% of customers who were offered the option used it"
- "Average customer setup time was X minutes"
- "Settlement was instant vs 2-3 business days with cards"

**This is the data that gets you in the door at Costco.**

### Step 4: Document Everything

- Screenshot the NowPayments/Circle dashboard showing transactions
- Screenshot your bank showing instant deposits
- Screenshot your card processor statement showing the fees you normally pay
- Record a 60-second video of a customer paying with USDC at your restaurant
- Get 3-5 customer testimonials (even short quotes work)
- Calculate total fees saved over the 30-day period

---

## PHASE 2: EXPAND TO 2-3 LOCAL BUSINESSES (Weeks 5-8)

Your restaurant proves it works for you. Now prove it works for someone else.

### Find 2-3 Local Businesses to Pilot

**Who to approach:**
- Other restaurant owners you know
- A local coffee shop or cafe
- A local retail store (clothing, electronics, etc.)
- A food truck (high volume, small tickets — good test case)
- A barber shop or salon

**Your pitch to them:**
"I'm testing a new payment system that cuts credit card fees from 2.35% to 0.5%. I'll set it up for free, manage everything, and you keep the savings. All I need is 30 days."

**What you handle for them:**
- Set up their NowPayments/Circle account
- Create their QR codes and signage
- Train their staff (10 minutes)
- Create customer-facing "How to Pay" guide
- Track all metrics for them
- Give them a weekly savings report

### What This Proves

- ZAP can onboard a merchant in hours, not months
- The system works across different business types
- You have implementation experience beyond your own business
- You can create a repeatable process

### Data You'll Collect

- 3 businesses × 30 days = 90 days of real-world data
- Transaction volume across different business types
- Adoption rates in different customer demographics
- Fee savings across different average ticket sizes
- Implementation time per merchant
- Staff training time per merchant

---

## PHASE 3: BUILD THE DASHBOARD (Weeks 5-12, parallel with Phase 2)

While running the local pilots, build a basic version of the ZAP Dashboard. This is what you demo to enterprise.

### Minimum Viable Dashboard

**What it needs to show:**
1. Total transactions processed (count and dollar value)
2. Total fees saved vs card processing
3. Adoption rate over time (graph)
4. Settlement status (instant vs pending)
5. Fee comparison: ZAP rate vs card rate

**How to build it:**
- Simple web app (React or even a static page with charts)
- Pull data from NowPayments/Circle API
- Compare against average card fees (2.35%)
- Show savings in real-time

**You don't need it to be production-grade.** You need it to look professional enough that a payments VP can see it on a screen and understand the value.

### What This Proves to Enterprise

"This isn't a PowerPoint. This is a working dashboard showing real transactions, real fee savings, and real settlement data from live businesses."

---

## PHASE 4: CASE STUDY & PITCH PACKAGE (Week 12)

### Compile the Case Study

**Title:** "ZAP Pilot Results: 80% Fee Reduction Across 3 Local Businesses"

**Structure:**
1. Problem: Card processing fees at 2.35%
2. Solution: USDC payments via ZAP at 0.5%
3. Results:
   - Total volume processed: $XX,XXX
   - Fee savings: XX%
   - Customer adoption rate: X%
   - Average setup time per merchant: X hours
   - Average customer onboarding time: X minutes
   - Settlement speed: instant vs 2-3 days
4. Customer quotes
5. Dashboard screenshots
6. Video of live payment

### Your Complete Pitch Package for Enterprise

When you walk into a meeting with Costco or Target, you bring:

1. **Pitch Deck** (10 slides — see PITCH_DECK.md)
2. **Case Study** (2-3 pages with real data from your pilots)
3. **Live Dashboard Demo** (show real transactions on screen)
4. **60-Second Payment Video** (customer paying at your restaurant)
5. **Executive Summary** (1-page leave-behind — see EXECUTIVE_SUMMARY.md)
6. **The Site** (cashnowzap.com — they'll Google you after the meeting)

---

## BUDGET FOR THE ENTIRE TEST

| Item | Cost |
|------|------|
| NowPayments account | Free to create |
| QR code signage (your restaurant) | $20-50 (printed signs) |
| Customer discount (5% off for USDC payers) | ~$200-500 over 30 days depending on volume |
| Signage for 2-3 local businesses | $60-150 |
| Dashboard hosting (Vercel free tier) | $0 |
| Domain (already have cashnowzap.com) | $0 |
| Your time | ~10-15 hours/week for 12 weeks |
| **Total cash outlay** | **~$300-700** |

You can prove this entire business model for under $1,000.

---

## TIMELINE SUMMARY

| Week | Activity | Deliverable |
|------|----------|-------------|
| 1 | Set up USDC payments at your restaurant | Working payment system |
| 2 | Create signage, train staff, start accepting | First USDC transactions |
| 3-4 | Run 30-day pilot, track all metrics | Transaction data |
| 5-6 | Onboard 2-3 local businesses | Multi-merchant pilot |
| 5-8 | Build basic ZAP Dashboard | Working demo |
| 8-10 | Complete local business pilots | 90 days of data |
| 10-12 | Compile case study, finalize pitch package | Complete pitch kit |
| 12+ | Begin enterprise outreach | Meetings with targets |

---

## WHAT MAKES THIS APPROACH UNBEATABLE

Most startups pitch enterprise with nothing but a slide deck and a promise. You'll walk in with:

- **Live transaction data** — not projections
- **Multiple business types** — not just your own
- **A working dashboard** — not a mockup
- **Video proof** — not a description
- **Customer testimonials** — not assumptions
- **Measured fee savings** — not estimates

When the VP of Payments at Costco asks "Has anyone actually used this?", you pull up the dashboard and show them live data. That's the difference between getting a "we'll think about it" and getting a pilot.

---

## THE WALMART/ZEROHASH DISTINCTION

When someone says "Walmart already has crypto" — here's your response:

"Walmart partnered with Zerohash to add crypto trading to their OnePay app. Customers can buy and sell Bitcoin and Ethereum as investments. That's a brokerage feature, like Robinhood inside the Walmart app.

What ZAP does is completely different. We replace the card payment at the register with a stablecoin payment. The customer pays with USDC — a digital dollar — and the merchant saves 80% on processing fees. Nobody at Walmart is paying for groceries with USDC today. The point-of-sale payment opportunity is completely untouched.

In fact, Walmart having Zerohash actually helps us. It means their customers are already getting comfortable with crypto inside the Walmart ecosystem. When we propose USDC payments at checkout, those customers are pre-educated."
