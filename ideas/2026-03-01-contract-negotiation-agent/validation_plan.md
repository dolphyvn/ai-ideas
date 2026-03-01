# Validation Plan - Contract Negotiation Agent

## Phase 1: Problem Validation (Days 1-3)

### Goal:
Confirm procurement teams actually care about contract negotiation.

### Method:
**LinkedIn Outreach**
- Target: CFOs, VPs of Procurement, Heads of Finance
- Companies: $10M-$100M ARR, heavy SaaS spend
- Outreach: 50 cold messages

**Message Template:**
```
Hi [Name],

We're building AI that autonomously negotiates SaaS contracts.

Early testing shows companies are overpaying 20-30% on standard SaaS agreements.

Quick question: Would you be interested in seeing what unfavorable clauses are hiding in your current contracts? No cost, just send us a redacted agreement.

If we find 3+ issues worth addressing, would a demo be valuable?

Thanks,
[Your Name]
```

### Success Criteria:
- 10+ replies with "yes, send more info"
- 5+ companies volunteer contracts for analysis
- 3+ agree to demo

### Kill Criteria:
- <5 responses total
- "We already use [Vendr/SaaS Spend]" >50% of responses
- "Not a priority right now" >70% of responses

---

## Phase 2: Solution Validation (Days 4-7)

### Goal:
Test if AI can actually find valuable contract issues.

### Method:
1. Build manual version (no AI needed yet)
2. Use legal checklist for top 20 SaaS vendors (Salesforce, Oracle, Microsoft, etc.)
3. Manually review 5 volunteered contracts
4. Deliver findings with dollar value estimates

**Deliverable to Prospects:**
- PDF report: 5 issues found
- Estimated annual savings: $X
- Recommended redlines

### Success Criteria:
- 3+ prospects say "this is valuable"
- At least 1 says "how much to automate this?"
- Identified savings >$50K annually per company

### Kill Criteria:
- All prospects say "we already knew this"
- Savings estimates <$10K (not worth paying for)
- Procurement says "we need human review anyway"

---

## Phase 3: Pricing Validation (Days 8-10)

### Goal:
Test willingness-to-pay.

### Method:
**Offer Tiers:**
- $499/month - Self-service
- $1,999/month - Full service
- 10% of savings - Performance model

**Ask:**
"Which of these would you choose if we automated this tomorrow?"

### Success Criteria:
- 2+ choose $1,999/month tier
- At least 1 chooses 10% of savings (validates ROI)
- No one says "this should be free"

### Kill Criteria:
- Everyone wants <$200/month
- "Our legal team handles this" (no budget)
- Request for one-time fee instead of subscription

---

## Phase 4: MVP Build (Days 11-17)

### Build:
1. **Contract Upload** → PDF parsing
2. **Claude 4.6 API** → Clause extraction
3. **Playbook Engine** → Redline suggestions
4. **Email Draft** → Negotiation email generation

### Test:
- Process 3 real contracts from Phase 2
- Human review each output
- Measure accuracy (target: 90%+ clause detection)

### Success Criteria:
- AI finds >80% of issues found manually
- Zero hallucinations (no fake clauses)
- <5 minute processing time per contract

---

## Phase 5: Commit Validation (Days 18-21)

### Goal:
Get pre-launch commitments.

### Method:
- Return to Phase 2-3 prospects
- "MVP is ready. Want to be first?"
- Offer: 50% off for first 3 months
- Request: 12-month commitment

### Success Criteria:
- 3+ pre-launch commitments
- At least 1 pays setup fee upfront
- 1+ agrees to case study

---

## Total Validation Timeline: 21 Days

## Go/No-Go Decision Criteria:

### GO if:
- 3+ paying commitments
- Identified savings >$100K across prospects
- 90%+ AI accuracy
- No legal blockers identified

### NO-GO if:
- <2 paying commitments
- AI accuracy <70%
- Legal liability exposure unmanageable
- Competitors already dominating (free product from incumbents)

---

## Fallback Plan:
If B2B validation fails, pivot to:
1. **Consumer focus**: Help individuals negotiate apartment leases, car purchases
2. **Vendor focus**: Sell to SaaS companies as "make your contracts negotiation-friendly"
3. **Agency model**: White-glove negotiation service, automate later
