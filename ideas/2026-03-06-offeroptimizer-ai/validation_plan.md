# OfferOptimizer Validation Plan

**7-Day Sprint to MVP Validation**

---

## Objective

Validate core assumptions with minimal build:
1. Will people share their job offers for analysis?
2. Will they practice negotiation with AI?
3. Will they share their salary wins on LinkedIn?
4. Will they pay $49-99 for a successful negotiation?

---

## Day 1-2: Landing Page + Waitlist

### Monday-Tuesday

**Build:**
```bash
# Tech Stack: Vercel + Framer Motion (rapid deployment)
- Single landing page
- Email capture (Waitlist)
- Value prop A/B testing
- Interactive "offer analyzer" teaser
```

**Copy Variants to Test:**

| Variant | Headline | CTA |
|---------|----------|-----|
| A (Greed) | "Last user got $43,000 more using our AI. Upload your offer." | "Analyze My Offer" |
| B (Fear) | "90% of people leave money on the table. Don't be one of them." | "Get What You Deserve" |
| C (Curiosity) | "Is your offer fair? AI compares your offer to 1M+ salaries." | "Check My Offer" |

**Interactive Teaser:**

```javascript
// Fake offer analyzer (no AI yet)
- User inputs: Salary, Role, Location
- Returns: "Based on our data, you might be leaving $15-40K on the table"
- CTA: "Get full analysis + negotiation script" (captures email)
```

**Metrics to Track:**
- Email capture rate
- Offer submission rate (even fake)
- Time on page
- Referral sources
- Role/location distribution (market research)

**Target:**
- 25%+ email capture from visitors
- 500 waitlist signups by Day 7
- 50+ fake offer submissions (interest signal)

---

## Day 3-4: Concierge MVP

### Wednesday-Thursday

**Build:**
```bash
# Manual backend, automated frontend
- Simple offer upload form
- Manual analysis (founder does it)
- Email/Slack delivery of results
- Shareable LinkedIn card generator
```

**Concierge Process Flow:**

```
1. User uploads/pastes offer
2. Founder manually analyzes:
   - Compares to Levels.fyi, Glassdoor, Blind data
   - Identifies negotiation potential
   - Drafts personalized script
3. Results emailed within 4 hours
4. Shareable card included in email
```

**User Script (First 30 users):**

```javascript
// Email Sequence
Email 1 (Immediate): "Analyzing your offer..."
Email 2 (4 hours later): "Your offer analysis:
  Market value: $170-195K (your offer: $145K)
  Negotiation potential: +$25-50K
  Personalized script attached"

Email 3 (48 hours later): "How did the negotiation go?
  Reply with your result, get $20 off future use"

Email 4 (After success): "Share your story?
  Here's a LinkedIn template if you got an increase"
```

**Data Capture:**
- Offer components (salary, bonus, equity)
- Gap to market (how underpriced are offers?)
- User reaction to gap (surprise? validation?)
- Willingness to negotiate
- Actual negotiation outcomes

**Target:**
- 30 users complete concierge analysis
- 80%+ surprised by market gap
- 20%+ attempt negotiation
- 10%+ share results (after success)

---

## Day 5-6: LinkedIn Sharing Test

### Friday-Saturday

**Test Viral Mechanics on LinkedIn**

**Shareable Card Formats:**

1. **LinkedIn Post Template**
```
I just used OfferOptimizer to analyze my job offer:

Original Offer: $145,000
Market Value: $175,000 - $195,000
Gap: $30,000 - $50,000 below market

The AI generated a personalized negotiation script that
helped me understand my leverage and practice the conversation.

Final result: $178,000 (+$33,000/year)

If you're navigating offers, happy to share the tool.
#career #negotiation #salary
```

2. **Visual Card (1200x627 for LinkedIn)**
```
┌─────────────────────────────────────────────────────┐
│                                                     │
│    How I Got 23% More Using AI                     │
│                                                     │
│    Original Offer: $145,000                         │
│    Final Offer: $178,000                            │
│                                                     │
│    +$33,000/year                                    │
│    +$550,000 lifetime earnings (20 years)          │
│                                                     │
│    [OfferOptimizer logo]                            │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Influencer Test:**
- 5 LinkedIn career creators
- Provide free concierge analysis
- Ask for honest LinkedIn post about experience
- Track engagement and conversions

**Anonymous Community Test:**
- Post to r/careerguidance, r/jobs
- "Tested this AI offer analyzer - here's my result"
- Track upvotes and comments

**Target:**
- 40%+ of successful users post to LinkedIn
- 0.3+ K-factor from posts (lower than BillSlayer, less viral)
- Identify most compelling format

---

## Day 7: Pricing Test

### Sunday

**Pricing Experiment:**

**A/B Test Offers:**

| Variant | Offer | Psychology |
|---------|-------|-------------|
| A | "$49 one-time. We help you get $10K+ more" | Rational ROI |
| B | "Free analysis. Pay $49 only if you negotiate" | Risk reversal |
| C | "$99 for 3 offers (career bundle). Average user gets $25K" | Value bundling |
| D | "$199 unlimited for 6 months. Get the job you deserve" | Power user |

**Email Script:**

```
Subject: Your offer analysis: $30K gap to market

Hi [Name],

I analyzed your offer for [Role] at [Company]:

📊 Your Offer: $145,000
💰 Market Range: $170,000 - $195,000
🎯 Gap: $25,000 - $50,000 below market

The good news: You have room to negotiate.

I've prepared:
✅ Market analysis with data sources
✅ Personalized negotiation script (3 scenarios)
✅ Objection handling guide
✅ AI roleplay practice partner

Get everything:
• Single Offer: $49 (one-time)
• Career Bundle: $99 (3 offers, 6 months)
• Unlimited: $199 (6 months, unlimited offers)

Which would you prefer?

[Reply with your choice]
```

**Target:**
- 15%+ convert to paid from concierge users
- Identify price sensitivity
- Validate willingness to pay for one-time use

---

## Validation Criteria

### Go/No-Go Decision Matrix

| Metric | Green Light | Yellow Light | Red Light |
|--------|-------------|--------------|-----------|
| Offer submission rate | 15%+ | 10-15% | <10% |
| Market gap surprise | 80%+ | 60-80% | <60% |
| LinkedIn share rate (after success) | 30%+ | 20-30% | <20% |
| Paid conversion | 12%+ | 8-12% | <8% |
| Negotiation attempt rate | 25%+ | 15-25% | <15% |

**Go decision:** 3+ Green metrics
**Build decision:** 2+ Yellow metrics + 1+ Green

### Kill Criteria

If ANY of these occur:
- <10% submit offers (even fake) → Not compelling enough
- <5% share on LinkedIn → Not viral enough for B2C
- <$10K average gap → Not enough value to charge for
- Users won't negotiate even with scripts → Product-market fit issue

---

## Build Checklist (Post-Validation)

### Week 2: MVP Development

**Core Features:**
- [ ] Offer parser (email, PDF, paste)
- [ ] Salary database API (Levels.fyi, Glassdoor, etc.)
- [ ] Market comparison engine
- [ ] Script generator (LLM-powered)
- [ ] AI roleplay chat interface
- [ ] LinkedIn share generator
- [ ] Stripe payment integration
- [ ] Email notification system

**Compliance:**
- [ ] Privacy policy (salary data is sensitive)
- [ ] Terms of service
- [ ] Data anonymization
- [ ] SOC 2 Type II initiation
- [ ] GDPR compliance (EU expansion)

**Analytics:**
- [ ] Mixpanel event tracking
- [ ] Offer outcome tracking
- [ ] Negotiation success rate
- [ ] LinkedIn share tracking
- [ ] Viral loop measurement

---

## Risk Mitigation

### What Could Go Wrong

| Risk | Signal | Pivot |
|------|--------|-------|
| Won't share salary data (privacy) | <20% submission rate | Anonymous option, data aggregation framing |
| Companies blacklist AI negotiators | Reports of candidates rejected | Position as "research + practice", not automation |
| Not viral enough | K-factor <0.3 | B2B pivot (HR tool, outplacement) |
| One-time use, no repeat business | 80%+ never return | Add career tracking, ongoing market monitoring |
| Salary data access blocked | APIs revoked | Crowd-sourced data, community model |

### Backup Plan: B2B Pivot

If B2C validation fails:

**Value Proposition:**
"OfferOptimizer for Teams - Career advancement for your employees"

**Target:**
- HR departments (retention tool)
- Outplacement firms (layoff benefits)
- Bootcamps (career services add-on)

**Pricing:**
- $25/employee/year (B2B)
- $150/candidate (outplacement)
- Revenue share with bootcamps

---

## Success Metrics (End of Day 7)

### Quantitative Targets

| Metric | Target | Actual |
|--------|--------|--------|
| Email waitlist | 500 | ___ |
| Offer submissions (real) | 30 | ___ |
| Concierge completions | 30 | ___ |
| Negotiation attempts | 8 | ___ |
| LinkedIn shares | 3 | ___ |
| Paid conversions | 5 | ___ |
| NPS score | 50+ | ___ |

### Qualitative Signals

- [ ] Users express excitement about salary gap
- [ ] Unsolicited LinkedIn posts
- [ ] Users ask for roleplay feature (product-market fit signal)
- [ ] Repeat usage (multiple offers)
- [ ] Referrals without incentives

---

## Post-Validation: Build Decision

### If Green Light:

**Immediate Actions:**
1. Hire 2 engineers (funding dependent)
2. Begin 6-week MVP build sprint
3. Launch private beta to waitlist
4. Continue concierge for new users

**Funding:**
- Bootstrap if possible (<$40K)
- Pre-seed if needed ($500K, 15-20% equity)

### If Yellow Light:

**Actions:**
1. Run another validation cycle (7 more days)
2. Test different messaging/positioning
3. Consider lower pricing ($29-39)
4. Gather deeper user interviews

### If Red Light:

**Actions:**
1. Document learnings
2. Kill with pride (not every idea works)
3. Apply insights to next venture
4. Consider B2B pivot if data suggests viability

---

## Continuous Validation

Even after launch, keep testing:

**Weekly Experiments:**
- Messaging variants
- Pricing tiers
- Script styles (aggressive vs. collaborative)
- Shareable formats
- Roleplay difficulty levels

**Monthly Deep Dives:**
- User interviews (10+ users)
- Negotiation outcome analysis
- Cohort analysis by industry
- LinkedIn engagement by post type

**Quarterly Reviews:**
- Unit economics revisited
- Market size recalibration
- Competitive landscape refresh
- Salary data moat assessment

---

## Pre-Launch: Community Building

**Pre-launch channels to build:**

1. **LinkedIn**
   - Founder's account (regular salary content)
   - Company page (company-specific negotiation guides)
   - Engage with #career #salary #negotiation posts

2. **Reddit**
   - r/careerguidance (success stories, AMAs)
   - r/jobs (offer review threads)
   - r/recruitinghell (anti-patterns to avoid)

3. **Discord/Slack**
   - Y Combinator career channel
   - Indie hackers (founder hires)
   - Industry-specific communities

**Content Strategy:**
- "Salary teardowns" (anonymized real offers)
- "Negotiation playbooks" by industry
- "Day in the life" of successful negotiation
- "Market watch" salary trend reports

---

*Document Version: 1.0*
*Last Updated: 2026-03-06*
