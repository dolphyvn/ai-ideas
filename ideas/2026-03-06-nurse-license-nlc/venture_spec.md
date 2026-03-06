# AI Venture Spec

## Name:
NurseLC NLC Tracker

## Core Concept:
AI-powered multistate nurse license compliance platform that tracks NLC (Nurse Licensure Compact) requirements across 39 participating states, predicts license lapses 30 days in advance, and automates renewal workflows for 3 million nurses and staffing agencies.

## Problem:
- **License lapse = immediate income loss**: Nurses cannot work without active license
- **NLC complexity explosion**: 39 states participate, each with different renewal dates, CNE requirements, background check rules
- **Staffing agencies lose $10,000+ per missed placement**: Travel nurse arrives on assignment, license expired -> placement cancelled
- **Manual tracking is impossible**: Staffing agencies manage 500-5,000 nurses each across multiple states
- **3M nurses, 40% travel/per-diem**: Highest urgency segment

## Target Vertical:
- **Primary**: Travel nurse staffing agencies (500+ agencies, $15B market)
- **Secondary**: Per-diem nursing platforms (shift-based marketplaces)
- **Tertiary**: Individual nurses (3M total, 1.2M travel/per-diem)

## Why Now:
- **NLC expansion**: 39 states now participate (was 25 in 2020), more nurses working multistate
- **Post-COVID travel nurse boom**: 40% increase in travel nursing, 2021-2024 growth permanent
- **State enforcement increasing**: Boards tightening audit rules, expired license = practice-blocking
- **Staffing agency pain**: Agency margins squeezed, can't afford $10K+ placement failures
- **AI capability frontier**: Vision models can extract requirements from board PDFs, LLMs can interpret state-specific rules

## AI Advantage:
- **Board PDF extraction**: Vision models parse 50 state board websites, PDF renewal notices, CNE requirements
- **Predictive lapse detection**: ML models identify at-risk nurses 30 days before expiration based on historical patterns
- **State rule interpretation**: LLMs translate 50 different regulatory frameworks into unified "renewal checklist"
- **CNE matching**: AI matches completed courses to state-specific requirements, auto-identifies gaps
- **Reminder personalization**: Optimal timing for renewal reminders (nurse schedules vary wildly)

## Viral Mechanism:
- **Staffing agency FOMO**: "Agency X didn't lose a single placement this year due to license lapses"
- **Nurse word-of-mouth**: "My agency proactively fixed my license before I knew it was expiring"
- **Travel nurse Facebook groups**: 200K+ members, license issues discussed daily
- **Placement crisis stories**: Every agency has horror stories of $50K losses from license lapses
- **Network effect**: More agencies using = more real-time lapse data = better predictions

## Revenue Model:
**Tier 1: Staffing Agency SaaS**
- $500/month for up to 200 nurses tracked
- $2,500/month for 200-1,000 nurses
- $10,000/month enterprise (1,000+ nurses)
- Includes: dashboard, automated alerts, renewal workflow tracking

**Tier 2: Per-Diem Platform API**
- $0.50 per nurse per month (volume-based)
- API integration into platform scheduling systems
- Real-time license verification before shift assignment

**Tier 3: Individual Nurse (B2C)**
- $15/month or $120/year
- Free for nurses whose agency subscribes (agency-sponsored)
- Includes: all-state tracking, CNE gap analysis, renewal document storage

**Crisis Insurance Add-on:**
- $0/month monitoring, $5,000 one-time when lapse detected and 48-hour expedited service needed

## Moat:
- **Data moat**: Aggregated license lapse patterns across 50 states (proprietary)
- **Integration moat**: Deep integrations with agency ATS/CRM systems (Bullhorn, Akken)
- **Network effects**: More agencies = more real-time lapse data = better predictions
- **Regulatory moat**: 50-state board API integrations (each state requires separate build)
- **Switching costs**: Once integrated into agency workflow, painful to extract

## MVP in 7 Days:
**Day 1-2: Data Pipeline**
- Python scrapers for 5 highest-volume state boards (CA, TX, FL, NY, TX BON)
- Store license lookup URLs, renewal deadlines in Postgres

**Day 3-4: Core Feature**
- Simple dashboard: bulk upload nurse list + license numbers
- Display: license status, expiration date, days-until-expiration
- Alert system: email when license expires in 30 days

**Day 5-6: AI Layer**
- Claude API for extracting renewal requirements from board PDFs
- Simple CNE tracker: upload CNE certificates, parse completion dates

**Day 7: Landing Page + Test**
- Launch landing page with demo video
- Cold email 10 travel nurse agencies with personalized "your nurses at risk" report
- Manual onboarding for first 2 agencies

## Tech Stack:
- **Backend**: Python (FastAPI), Postgres, Redis (caching)
- **AI**: Claude API (board PDF parsing), OpenAI (classification)
- **Scraping**: Playwright (JavaScript-heavy board sites), proxies for rate limiting
- **Frontend**: Next.js 14, shadcn/ui components
- **Infrastructure**: AWS (ECS for containers, RDS Postgres, S3 for document storage)
- **Monitoring**: Sentry (errors), Mixpanel (analytics)

## Monthly Revenue Potential (Year 1-3):

**Year 1 (Conservative):**
- 20 agencies @ $500/mo = $10,000 MRR
- 5 agencies @ $2,500/mo = $12,500 MRR
- 1,000 individual nurses @ $15/mo = $15,000 MRR
- **Total Year 1 MRR: ~$37,500 → $450K ARR**

**Year 2 (Moderate Growth):**
- 100 agencies @ avg $1,500/mo = $150,000 MRR
- 20,000 individual nurses = $300,000 MRR
- 2 per-diem platforms @ volume pricing = $50,000 MRR
- **Total Year 2 MRR: ~$500,000 → $6M ARR**

**Year 3 (Market Penetration):**
- 300 agencies (15% of market) @ avg $2,000/mo = $600,000 MRR
- 100,000 nurses = $1,500,000 MRR
- 10 platforms integrated = $250,000 MRR
- **Total Year 3 MRR: ~$2,350,000 → $28M ARR**

## Risk Factors:
- **State board website changes**: Scraping breakage, need to maintain 50 separate parsers
- **Competitive threat**: Nursegrid, Nursys (existing but clunky), Verity (nurse-focused background checks)
- **Data accuracy**: Wrong expiration dates = misplaced liability
- **Agency adoption speed**: Staffing industry is slow to adopt new tech, multi-month sales cycles
- **NLC rule changes**: Compact rules evolve, requiring ongoing platform updates
- **HIPAA concerns**: Handling nurse personal information requires compliance

## Competitive Threat:
- **Nursys (NCSBN)**: Official database but read-only, no proactive tracking, poor UX
- **Nursegrid**: Career-focused platform, license tracking is secondary feature
- **CEBroker**: CNE tracking only, no license expiration focus
- **Agency homegrown**: Most agencies use spreadsheets today (fragile, error-prone)
- **New entrants**: Low barrier to basic scraping, but high barrier to 50-state coverage + AI rules

**Differentiation:**
- **AI-powered rule interpretation**: Only product that understands 50-state regulatory nuances
- **Predictive vs reactive**: 30-day advance notice vs "your license expired yesterday"
- **Agency-first design**: Built for staffing agency workflows, not individual nurses
- **CNE gap analysis**: Only product matching completed courses to state requirements

## Go-to-Market Strategy:
**Phase 1 (Months 1-3): Agency Direct Sales**
- Target top 50 travel nurse agencies by revenue
- Cold outreach with personalized "at-risk nurse" reports
- Offer free pilot: "We'll track your top 100 travelers for 30 days, show you lapses prevented"
- Case study from each success

**Phase 2 (Months 4-6): Partnerships**
- Partner with ATS vendors (Bullhorn, Akken) for marketplace listing
- Partner with nursing associations (Travel Nurses Unlimited) for member discount
- Conference presence: Staffing World, Healthcare Staffing Summit

**Phase 3 (Months 7-12): Platform Expansion**
- API launch for per-diem platforms (CareRev, ShiftKey)
- Individual nurse launch (agency-sponsored accounts)
- Viral content: "License Lapse Horror Stories" podcast/LinkedIn series
