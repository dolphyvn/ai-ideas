# BillSlayer Validation Plan

**7-Day Sprint to MVP Validation**

---

## Objective

Validate core assumptions with minimal build:
1. Will people connect their bank account to see subscriptions?
2. Will they share their savings on social media?
3. Will they pay for the service after seeing savings?
4. Can we actually cancel subscriptions automatically?

---

## Day 1-2: Landing Page + Waitlist

### Monday-Tuesday

**Build:**
```bash
# Tech Stack: Vercel + Framer Motion (rapid deployment)
- Single landing page
- Email capture (Waitlist)
- Value prop A/B testing
- Social proof placeholders
```

**Copy Variants to Test:**

| Variant | Headline | CTA |
|---------|----------|-----|
| A (Fear) | "You're paying $400/mo in subscriptions you forgot about" | "Find Out How Much" |
| B (Greed) | "Our AI just saved Jane $1,247/year. See what you can save" | "Get My Free Scan" |
| C (Curiosity) | "Connect your bank. We'll find every subscription in 30 seconds." | "Scan My Subscriptions" |

**Metrics to Track:**
- Email capture rate
- Click-through by traffic source
- Time on page
- Referral sources

**Target:**
- 20%+ email capture from visitors
- 1,000 waitlist signups by Day 7

---

## Day 3-4: Concierge MVP

### Wednesday-Thursday

**Build:**
```bash
# Manual backend, automated frontend
- Stripe/Plaid sandbox integration
- Manual transaction analysis (founder does it)
- Email/Slack delivery of results
- Shareable card generator
```

**Concierge Process Flow:**

```
1. User connects bank (Plaid link)
2. Transactions pulled automatically
3. Founder manually reviews transactions
4. AI (GPT-4) categorizes subscriptions
5. Results emailed to user within 2 hours
6. Shareable card included in email
```

**User Script (First 50 users):**

```javascript
// Email Sequence
Email 1 (Immediate): "Analyzing your subscriptions..."
Email 2 (2 hours later): "Found 12 subscriptions. You're paying $347/mo."
Email 3 (48 hours later): "Want us to cancel the 4 you don't use?"
Email 4 (Day 7): "How much have you saved? Share your story"
```

**Data Capture:**
- Total subscriptions found
- Dollar amount of potential savings
- User's reaction to savings amount
- Willingness to share on social media

**Target:**
- 50 users complete concierge onboarding
- 80%+ surprised by subscription count
- 40%+ share their results

---

## Day 5-6: Social Sharing Test

### Friday-Saturday

**Test Viral Mechanics:**

**Shareable Card Formats:**

1. **Instagram Story Size (1080x1920)**
```
┌─────────────────────────────┐
│                             │
│     I just found out        │
│     I'm paying $427/mo      │
│     in subscriptions        │
│                             │
│     📱 14 total             │
│     💀 8 I forgot about     │
│     💸 $2,400/year wasted   │
│                             │
│     Scan yours:             │
│     billslayer.ai           │
│                             │
└─────────────────────────────┘
```

2. **Twitter/X Card**
```
BillSlayer just scanned my subscriptions:

🔍 Found: 12 subscriptions
😳 I knew about: 4 of them
💰 Monthly cost: $347
🎯 Savings potential: $1,800/year

This is painful but necessary. Get your free scan →
```

3. **TikTok Template**
- Background music: trending audio
- Text overlays with dramatic reveal
- Point-of-view: "watch me find out how much I'm wasting"

**Influencer Test:**
- 5 personal finance TikTok creators
- Pay $100 each for honest review
- Provide custom discount code
- Track conversion from each

**Target:**
- 30%+ of test users share their card
- 0.5+ K-factor from shares
- Identify most shareable format

---

## Day 7: Pricing Test

### Sunday

**Pricing Experiment:**

**A/B Test Offers:**

| Variant | Offer | Psychology |
|---------|-------|-------------|
| A | "Pay $49/year. We'll save you $500+" | Rational ROI |
| B | "Free scan. Pay only if we save you $200+" | Risk reversal |
| C | "$99/year. Cancel anytime. Full refund if you don't save $300+" | Guarantee |

**Email Script:**

```
Subject: We found $1,200/year in savings

Hi [Name],

Our AI found 12 subscriptions costing you $347/month:

✅ Keep: Netflix, Spotify, Amazon Prime (you use these)
❌ Cancel: Gym membership, 3 streaming services, beauty box
📉 Negotiate: Your insurance could be $40/mo less

We can cancel the unwanted ones and negotiate the rest for you.

Plan options:
• Free DIY (we'll send instructions)
• Pro ($79/year): We do everything automatically
• Lifetime ($199): Everything, forever, including future subscriptions

Which would you prefer?

[Reply with your choice]
```

**Target:**
- 20%+ convert to paid from concierge users
- Identify price sensitivity
- Validate willingness to pay for automation

---

## Validation Criteria

### Go/No-Go Decision Matrix

| Metric | Green Light | Yellow Light | Red Light |
|--------|-------------|--------------|-----------|
| Bank connection rate | 60%+ | 40-60% | <40% |
| Savings surprise (reaction) | 80%+ | 60-80% | <60% |
| Social share rate | 30%+ | 20-30% | <20% |
| Paid conversion | 15%+ | 10-15% | <10% |
| Referral rate | 25%+ | 15-25% | <15% |

**Go decision:** 3+ Green metrics
**Build decision:** 2+ Yellow metrics + 1+ Green

### Kill Criteria

If ANY of these occur:
- <20% connect bank account → Trust issue, reconsider approach
- <10% share results → Not viral, not B2C-scalable
- <$100 average savings potential → Not enough value
- Users refuse to pay for automation → Product-market fit issue

---

## Build Checklist (Post-Validation)

### Week 2: MVP Development

**Core Features:**
- [ ] Plaid/Yodlee bank integration
- [ ] Transaction classification model
- [ ] Subscription database (merchants, cancellation methods)
- [ ] One-click cancellation flow
- [ ] Shareable card generator (all formats)
- [ ] Email notification system
- [ ] Stripe payment integration

**Compliance:**
- [ ] Privacy policy
- [ ] Terms of service
- [ ] SOC 2 Type II initiation
- [ ] Bank-level security audit
- [ ] Data encryption at rest and transit

**Analytics:**
- [ ] Mixpanel event tracking
- [ ] Stripe analytics
- [ ] Viral loop tracking
- [ ] Churn prediction setup

---

## Risk Mitigation

### What Could Go Wrong

| Risk | Signal | Pivot |
|------|--------|-------|
| Trust issues (won't connect bank) | <30% connection rate | Email upload alternative, manual entry |
| Can't cancel subscriptions | <50% cancellation success | Negotiation scripts instead of automation |
| Not viral | K-factor <0.5 | B2B pivot (HR benefits, employee perk) |
| High churn after first use | 50%+ churn month 2 | Ongoing monitoring value |

### Backup Plan: B2B Pivot

If B2C validation fails:

**Value Proposition:**
"BillSlayer for Teams - Company subscription management"

**Target:**
- SMBs with 10-100 employees
- expense reimbursement chaos
- Multiple SaaS subscriptions

**Pricing:**
- $99/month for companies
- Employee perk (free for individuals)
- Corporate card integration

---

## Success Metrics (End of Day 7)

### Quantitative Targets

| Metric | Target | Actual |
|--------|--------|--------|
| Email waitlist | 1,000 | ___ |
| Bank connections | 100 | ___ |
| Concierge completions | 50 | ___ |
| Social shares | 15 | ___ |
| Paid conversions | 8 | ___ |
| NPS score | 40+ | ___ |

### Qualitative Signals

- [ ] Users express excitement about savings
- [ ] Unsolicited social media mentions
- [ ] Users ask for features (product-market fit signal)
- [ ] Repeat usage (come back to check)
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
- Bootstrap if possible (<$50K)
- Pre-seed if needed ($500K, 20% equity)

### If Yellow Light:

**Actions:**
1. Run another validation cycle (7 more days)
2. Test different messaging/positioning
3. Consider alternative monetization
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
- Onboarding flows
- Shareable formats
- Cancellation methods

**Monthly Deep Dives:**
- User interviews (10+ users)
- Cohort analysis by acquisition channel
- Churn analysis by user segment
- Viral coefficient by social platform

**Quarterly Reviews:**
- Unit economics revisited
- Market size recalibration
- Competitive landscape refresh
- Moat strengthening assessment

---

*Document Version: 1.0*
*Last Updated: 2026-03-06*
