# Validation Plan: OfferOptimizer

## Objective
Validate that job seekers will use AI to negotiate salary and that it results in higher compensation.

## Week 1: Manual Concierge MVP

### Target: 20 offer analyses, 5 negotiation attempts

**Days 1-2: Setup**
- Create simple landing page (Typeform + basic site)
- Offer: "Free AI-powered salary negotiation - first 20 people"
- Post in: r/jobs, r/recruiting, r/careerguidance, r/jobsbit
- LinkedIn: Post in job search groups

**Days 3-4: Manual Analysis**
- For each submitted offer:
  - Use Claude to analyze components
  - Research salary data manually
  - Generate 3 negotiation scripts
  - Email back within 4 hours

**Days 5-7: Follow-up**
- Email users 3 days later: "Did you negotiate?"
- Track outcomes (attempted, succeeded, failed)
- Collect testimonials for those who got more money

## Week 2: Automated MVP

**If validation successful (5+ negotiation attempts):**

**Days 8-10: Build Automation**
- PDF parser (pypdf + OCR)
- Salary scraping (Levels.fyi, Glassdoor)
- Script generation templates
- Simple dashboard

**Days 11-14: Beta Launch**
- 50 beta users
- Charge $29 (discounted from $49)
- Measure: conversion rate, usage, outcomes

## Success Criteria

**Minimum Viable Signal:**
- [ ] 20+ offers analyzed
- [ ] 5+ users attempt negotiations
- [ ] 2+ users report higher compensation
- [ ] 50%+ say they would pay $49

**Strong Signal:**
- [ ] 50+ offers analyzed
- [ ] 10+ users report higher comp
- [ ] Average increase >$5K
- [ ] 1+ LinkedIn viral post about success

**Kill Criteria:**
- < 3 negotiation attempts after 20 analyses
- Users refuse to negotiate despite scripts
- Salary data is insufficient/incorrect

## Channels to Test

1. **Reddit**: r/jobs, r/recruiting, r/careerguidance, r/jobsbit
2. **LinkedIn**: Job search groups, "Open to Work" posts
3. **TikTok**: Career creators, job search tips
4. **Twitter/X**: #opentowork, #careeradvice
5. **Hacker News**: "Show HN: AI negotiated my salary"

## Data to Collect

- Conversion: landing page visitors → submit offer
- Engagement: open rate of analysis emails
- Action: % who attempt negotiations
- Outcome: $ amount of increases
- NPS: would they recommend?
- Pricing: what would they pay?

## Go/No-Go Decision

**GO if:**
- 5+ negotiation attempts AND 2+ successful outcomes
- 40%+ say they'd pay $49+
- Average increase >$3K

**NO-GO if:**
- < 3 negotiation attempts
- 0 successful negotiations
- Users say scripts don't feel authentic

**PIVOT if:**
- High engagement but low willingness to pay → freemium with career services
- High willingness to practice but not negotiate → focus on interview prep
