# Validation Plan: 7-Day MVP Sprint

**Venture:** CA SB 1383 Food Waste Tracker
**Duration:** 7 days
**Goal:** Validate demand before writing code
**Success Criteria:** 3 letters of intent OR 10 pre-registrations

---

## Day 1: Customer Discovery Interviews

### Objective
Validate problem urgency and willingness to pay

### Target: 10 Conversations

**Who to interview:**
1. Multi-location restaurant franchisees (3)
2. Independent restaurant owners (3)
3. Grocery store managers (2)
4. Food processing facility managers (2)

**Interview Script:**

#### Opening (2 min)
> "Thanks for taking the time. I'm researching how California businesses handle SB 1383 compliance. Your feedback will help me understand if there's a better way to manage this. This is research, not a sales pitch. Everything we discuss is confidential."

#### Questions (20 min)

**Problem Validation:**
1. "How are you currently tracking organic waste diversion for SB 1383?"
2. "Who owns compliance at your organization?"
3. "What's your biggest frustration with current compliance process?"
4. "Have you or anyone you know received fines for non-compliance?"

**Solution Validation:**
5. "If I showed you a photo of your waste, could you tell me what percentage is organic?"
6. "How do you track exemption thresholds for each city you operate in?"
7. "What would you pay to never worry about SB 1383 fines again?"
8. "Would you use a mobile app to document waste disposal? Why/why not?"

**Closing:**
> "This has been incredibly helpful. I'm building a solution based on these insights. Would you be open to seeing a demo when it's ready? Also, do you know 2-3 other business owners dealing with this?"

### Red Flags
- "We don't track this at all" AND don't care
- "My hauler handles it" (follow up: how do they prove diversion?)
- "We're exempt" (ask: have you verified with the city?)

### Green Flags
- "I'm worried about the $10K/day fines"
- "My spreadsheet is a mess"
- "I have locations in 5 different cities with different rules"
- "How much? I'd pay $X/month"

### Day 1 Deliverable
- Interview notes in shared doc
- Pattern analysis (what surprised you?)
- Update customer profile based on learnings

---

## Day 2: Municipal Data Deep Dive

### Objective
Assess feasibility of ordinance aggregation

### Tasks

#### Morning: Public Data Collection
1. **Identify top 20 target cities** (by restaurant density):
   - Los Angeles, San Francisco, San Diego, San Jose, Sacramento
   - Oakland, Fresno, Long Beach, Bakersfield, Anaheim
   - Santa Ana, Riverside, Stockton, Irvine, Fremont
   - San Bernardino, Modesto, Fontana, Oxnard, Moreno Valley

2. **For each city, find:**
   - [ ] SB 1383 implementation page
   - [ ] Exemption application form
   - [ ] Exemption eligibility criteria
   - [ ] Enforcement contact
   - [ ] Annual reporting requirements
   - [ ] Hauler partners

3. **Document in spreadsheet:**
   ```
   City | Population | Exemption Threshold | Application Link | Contact | Notes
   ```

#### Afternoon: Outreach
1. **Call 5 municipal sustainability offices:**
   - "Hi, I'm a small business owner trying to understand SB 1383 exemption requirements in [CITY]. Can you walk me through the process?"
   - Document: responsiveness, clarity, additional resources mentioned

2. **Identify data sources:**
   - CalRecycle municipal resources page
   - League of California Cities resources
   - Third-party compliance consultants

### Success Criteria
- 80% of cities have public exemption info
- At least one city has a clear, structured exemption process
- Clear path to aggregate remaining cities

### Failure Criteria
- < 50% of cities have public info
- All cities say "contact your hauler" (no direct municipal oversight)
- No enforcement happening yet

### Day 2 Deliverable
- Municipal ordinance database (MVP version)
- Map of data gaps
- Feasibility assessment

---

## Day 3: Competitive Audit

### Objective
Understand existing solutions and gaps

### Tasks

#### Morning: Product Research
1. **Test competitor products:**
   - [Leanpath](https://leanpath.com): Request demo, note pricing
   - [Winnow](https://winnowsolutions.com): Request demo, note pricing
   - [Copely](https://copely.com): Research waste management features
   - [Local municipal tools]: Test 3 city-provided compliance portals

2. **For each competitor, document:**
   - Core features
   - Pricing model
   - SB 1383 specific features?
   - Municipal exemption handling?
   - Hauler integrations?
   - Target customer

#### Afternoon: Gap Analysis
1. **Feature matrix:**
   ```
   Feature | Leanpath | Winnow | Municipal Tools | Our Solution
   Waste Tracking | ✓ | ✓ | Partial | ✓
   Photo Classification | ✓ | ✓ | ✗ | ✓
   Exemption Finder | ✗ | ✗ | Partial | ✓
   Hauler Integration | Partial | Partial | ✗ | ✓
   Multi-Language | ✗ | ✗ | ✗ | ✓
   Price | $5K+ | £3K+ | Free | $99-299
   ```

2. **Identify our wedge:**
   - What are competitors NOT doing?
   - What do customers complain about?
   - What's too expensive for small businesses?

### Day 3 Deliverable
- Competitive analysis document
- Differentiation statement
- Feature prioritization for MVP

---

## Day 4: Pre-Product Landing Page

### Objective
Test value proposition and collect leads

### Landing Page Elements

#### Headline Options (A/B test)
1. "Never Pay a $10,000 SB 1383 Fine Again"
2. "California Food Waste Compliance in 5 Minutes/Day"
3. "Automated SB 1383 Compliance for Restaurants"
4. "The Only SB 1383 Tool That Files Exemptions For You"

#### Page Sections
1. **Hero:** Headline + subheadline + email capture
2. **Problem:** "$10K/day fines, 500K+ businesses at risk"
3. **Solution:** "Photo tracking, exemption automation, municipal database"
4. **Social Proof:** Logos (placeholder) + early adopter count
5. **Pricing:** Transparent ($99-299/mo)
6. **CTA:** "Get Early Access - 50% Off First Year"

#### Copy Framework
```
[Headline]

[Subhead: Automated compliance for California's SB 1383 organic waste law]

[3-bullet value prop]:
- Snap photos of waste → AI tracks your diversion rate
- We find exemptions you qualify for (city-specific)
- Alerts before you risk a $10K/day fine

[CTA button]

[Social proof]: "Already helping 50+ businesses stay compliant"

[Trust badges]: Compliant with CalRecycle standards | Secure data | Cancel anytime
```

### Traffic Sources
1. **LinkedIn:** Post in California Restaurant Association groups
2. **Twitter/X:** Tag CalRecycle, restaurant associations
3. **Reddit:** r/restaurant, r/CaliforniaBusiness
4. **Local chambers:** Email blast (offer affiliate commission)
5. **Facebook ads:** Target restaurant owners in CA (geo-fenced)

### Day 4 Deliverable
- Live landing page (Carrd/Webflow/Linear - no code)
- Email capture connected (Mailchimp/ConvertKit)
- Analytics installed (Google Analytics)

---

## Day 5-6: Traffic + Conversion

### Objective
Drive 500 visitors, capture 50 emails

#### Day 5: Launch
1. **Morning:**
   - Final landing page QA
   - Set up analytics goals
   - Prepare social posts

2. **Afternoon:**
   - Launch to LinkedIn (personal + company)
   - Post to Reddit (r/restaurant, r/restaurantindustry)
   - Tweet with handles (@CalRecycle, @CRArestaurants)

3. **Evening:**
   - Check first 4 hours of traffic
   - Respond to comments/DMs
   - Note which channels convert

#### Day 6: Follow-Up
1. **Outreach to signups:**
   - Email template:
     ```
     Subject: Quick question about your SB 1383 setup

     Thanks for signing up! Quick question - what's your biggest
     pain point with current compliance tracking?

     Hit reply - I read every response.

     - [Your Name]
     ```

2. **Sales outreach:**
   - Call back high-intent leads (provided phone number)
   - Offer: 30-min consultation + $99/mo lifetime discount

3. **Content push:**
   - Post LinkedIn article: "SB 1383 Compliance: 5 Mistakes That Cost $10K/Day"
   - Share in 5 more subreddits
   - Email 20 restaurant associations

### Day 6 Deliverable
- Traffic analysis (which channels worked?)
- Lead list with qualification notes
- 3-5 sales calls scheduled

---

## Day 7: Decision + Commit

### Objective
Go/No-Go decision based on validation data

### Decision Framework

#### GO if:
- [ ] 3+ letters of intent signed OR 10+ pre-registrations
- [ ] Clear pain point validated (6+ interviews mentioned fines)
- [ ] Municipal data path clear (80%+ cities have public info)
- [ ] 2+ competitor gaps identified
- [ ] Landing page conversion > 3%

#### NO-GO if:
- [ ] < 5 qualified leads
- [ ] Municipal data unavailable or inconsistent
- [ ] Competitors already doing this well
- [ ] Customers say "my hauler handles it" (no urgency)
- [ ] Conversion < 1%

#### PROCEED WITH CAUTION if:
- [ ] Mixed signals (some urgency, some indifference)
- [ ] Municipal data available but scattered
- [ ] Strong leads but low volume

### Next Steps (if GO)

#### Week 2: Technical Setup
- Next.js project scaffold
- Supabase database schema
- Authentication (Clerk)
- Stripe integration

#### Week 3-4: MVP Build
- Manual waste tracking (no AI yet)
- Municipal exemption database (50 cities)
- Basic dashboard
- Exemption calculator

#### Week 5: Beta Launch
- Onboard first 10 customers
- Weekly feedback calls
- Rapid iteration

#### Week 6-8: AI Integration
- Build waste classification model
- Photo capture feature
- Launch v1.0

### Day 7 Deliverable
- Go/No-Go decision document
- Customer testimonials (if available)
- Updated venture score based on findings

---

## Success Metrics Summary

| Metric | Target | Actual | Pass/Fail |
|--------|--------|--------|-----------|
| Interviews completed | 10 | ___ | ___ |
| Pain point validated | 8/10 | ___ | ___ |
| Municipal data accessible | 80% cities | ___ | ___ |
| Landing page visitors | 500 | ___ | ___ |
| Email captures | 50 | ___ | ___ |
| Letters of intent | 3 | ___ | ___ |
| Sales calls booked | 5 | ___ | ___ |
| Competitor gaps identified | 2+ | ___ | ___ |

---

## Resources

### Tools
- **Landing page:** Carrd ($19/yr), Webflow, or Linear.app
- **Email capture:** ConvertKit, Mailchimp, or Substack
- **Scheduling:** Calendly (free tier)
- **Survey:** Typeform or Google Forms
- **Notes:** Notion or Obsidian

### Templates
- Interview script (provided above)
- Cold email templates
- Letter of intent template
- Sales pitch deck outline

### Outreach Lists
- **Restaurant Associations:**
  - California Restaurant Association
  - Golden State Restaurant Association
  - National Restaurant Association (CA chapters)

- **Municipal Contacts:**
  - City sustainability offices (top 20 cities)
  - CalRecycle SB 1383 team
  - County environmental health departments

---

## Week 2 Preview (If GO)

### Build Sprint: Manual MVP

**Day 1-2:** Tech scaffold
- Next.js 14 + shadcn/ui
- Supabase setup + schema design
- Clerk authentication
- Stripe payment flow

**Day 3-4:** Core features
- Waste tracking form (manual entry)
- Municipal database (50 cities, manual data entry)
- Compliance dashboard
- User profile management

**Day 5:** Testing
- End-to-end user flow
- Payment test
- Deploy to Vercel

**Day 6-7:** Customer onboarding
- First 10 customers from validation
- Onboarding calls
- Feedback loops

### MVP Feature Checklist
- [ ] User registration/login
- [ ] Business profile setup (location, waste tier)
- [ ] Manual waste entry (type, pounds, date)
- [ ] Compliance dashboard (current vs. threshold)
- [ ] Municipal exemption lookup
- [ ] Exemption eligibility calculator
- [ ] Subscription payment
- [ ] Basic reporting (CSV export)

---

## Risk Mitigation

### If Traffic Is Low
- **Pivot to direct outreach:** Cold email 500 restaurants
- **Paid ads:** $100 Facebook ads test
- **Partner outreach:** Contact waste haulers directly

### If Signups Don't Convert
- **Pricing test:** Offer lower price ($49/mo) for first 6 months
- **Feature adjustment:** Add high-demand feature based on feedback
- **Target change:** Pivot to larger enterprises (higher urgency)

### If Municipal Data Is Unavailable
- **Focus on top cities:** Launch with 10 cities first
- **Partner with consultants:** Revenue share for exemption filing
- **Change model:** Compliance consulting + light software

---

## Post-Sprint Actions

### Success Path
1. Incorporate entity (LLC)
2. Open bank account
3. Set up accounting (Stripe Atlas)
4. Apply to Y Combinator or other accelerators
5. Begin fundraising conversations (optional)

### Failure Path
1. Document lessons learned
2. Archive customer research
3. Identify pivot opportunities
4. Update venture score with real data
5. Share findings with community (blog post)

---

## Appendix: Interview Scripts

### Script 1: Restaurant Franchisee
> "Hi [Name], I'm researching how multi-location restaurants handle SB 1383 compliance across different cities. You operate in [CITIES] - have you had to deal with different exemption rules in each location? How do you track compliance today?"

### Script 2: Waste Hauler Rep
> "Hi [Name], I'm building a tool to help your customers stay compliant with SB 1383. What are the most common compliance questions you get from restaurants? Would you be interested in a white-label solution for your customers?"

### Script 3: Municipal Compliance Officer
> "Hi [Name], I'm trying to understand the exemption process for [CITY]. Can you walk me through how a small business would apply for an SB 1383 exemption? What documentation do they need?"

### Script 4: Restaurant Association Director
> "Hi [Name], I'm building a compliance tool for SB 1383. Are your members asking about this? What resources do you currently provide? Would you be open to an exclusive discount for your members?"

---

## Validation Tracker

Use this table to track daily progress:

| Day | Focus | Target | Actual | Notes |
|-----|-------|--------|--------|-------|
| 1 | Interviews | 10 | ___ | Pattern: ___ |
| 2 | Municipal data | 20 cities | ___ | Gap: ___ |
| 3 | Competitor audit | 4 products | ___ | Wedge: ___ |
| 4 | Landing page | Live | ___ | Headline: ___ |
| 5 | Traffic | 300 visitors | ___ | Channel: ___ |
| 6 | Leads | 50 emails | ___ | Qualified: ___ |
| 7 | Decision | Go/No-Go | ___ | Score: ___/10 |
