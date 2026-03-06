# AI Venture Spec

## Name:
CPA Shield

## Core Concept:
AI-powered multi-state CPA license compliance platform that tracks CPE requirements, license renewals, and state board regulations across 50 jurisdictions for 600,000 CPAs and accounting firms.

## Problem:
- **License lapse = practice-blocking**: Expired CPA cannot sign audit opinions, tax returns, or attestation reports
- **50 state boards, 50 different rules**: Each state has unique CPE requirements, renewal cycles, ethics course mandates
- **Firms face massive liability**: Signing with expired license = malpractice, client lawsuits, board sanctions
- **CPE tracking is a nightmare**: CPAs complete courses across platforms, state boards have different acceptance rules
- **Firms spend $5,000+/year per CPA on compliance**: Existing solutions are spreadsheets and manual tracking

## Target Vertical:
- **Primary**: Mid-market accounting firms (20-500 employees) - ~12,000 firms in US
- **Secondary**: Big 4 firms (Deloitte, PwC, EY, KPMG) - enterprise sales to compliance departments
- **Tertiary**: Individual CPAs (600K total, 200K in public accounting)

## Why Now:
- **CPE requirements expanding**: States adding ethics, diversity, cybersecurity requirements (new complexity)
- **Remote work trend**: CPAs licensed in multiple states, working across state lines
- **Board enforcement increasing**: State boards auditing CPE compliance more aggressively post-pandemic
- **AI capability frontier**: LLMs can parse 50 different state board rule documents, extract requirements
- **Firm pain point**: Partners personally liable for firm compliance, urgent problem for firm leadership

## AI Advantage:
- **State rule interpretation**: LLMs parse 50 state board websites, PDF rulebooks, extract unique requirements
- **CPE matching**: AI matches completed courses to state-specific requirements (some states reject certain providers)
- **Predictive compliance**: Identifies CPAs at risk of non-compliance 90 days before license renewal
- **Document extraction**: Vision models extract CPE completion from varied certificate formats (PDFs, images, emails)
- **Requirement mapping**: Maps one course to multiple state requirements (e.g., "404 A&A Auditing" counts differently per state)

## Viral Mechanism:
- **Firm partner fear**: "Our firm was nearly sanctioned because a senior manager's license expired"
- **Accounting industry tight-knit**: Partners talk at AICPA conferences, state CPA society events
- **Compliance horror stories**: "Firm X lost 3 audit clients because a partner signed with expired license"
- **State board newsletter mentions**: Boards publish enforcement actions publicly (PR nightmare for firms)
- **Network effects**: More firms using = more CPE provider data = better matching accuracy

## Revenue Model:
**Tier 1: Firm Subscription (Primary Revenue)**
- Small firms (2-20 CPAs): $299/month
- Mid-market (20-100 CPAs): $799/month
- Large firms (100-500 CPAs): $2,499/month
- Enterprise (500+ CPAs): Custom pricing, typically $50,000-200,000/year

**Tier 2: Individual CPA (Secondary)**
- $19/month or $159/year
- Free for CPAs whose firm subscribes (firm-sponsored)
- Includes: all-state tracking, CPE gap analysis, renewal alerts

**Tier 3: CPE Provider Partnerships**
- CPE providers pay for placement recommendation (CPA needs ethics course -> recommend approved provider)
- Revenue share on course completions

**Add-on: Audit Defense**
- $0/month monitoring, $10,000 one-time for emergency board response coordination

## Moat:
- **Data moat**: Aggregated CPE requirements across 50 states, course provider acceptance data
- **Integration moat**: Deep integrations with firm practice management systems (Caseware, Thomson Reuters, CCH)
- **Regulatory moat**: 50-state board rule interpretation (rules change frequently, must stay current)
- **Network effects**: More firms = more CPE completion data = better matching accuracy
- **Switching costs**: Once integrated into firm compliance workflow, painful to extract

## MVP in 7 Days:
**Day 1-2: Data Pipeline**
- Python scrapers for 10 highest-volume state boards (CA, NY, TX, FL, IL, PA, OH, GA, NC, MI)
- Store license lookup URLs, renewal deadlines, CPE requirements in Postgres

**Day 3-4: Core Feature**
- Simple dashboard: bulk upload CPA list + license numbers
- Display: license status, expiration date, CPE progress
- Alert system: email when license expires in 90 days

**Day 5-6: AI Layer**
- Claude API for extracting CPE requirements from board PDFs
- Simple CPE tracker: upload CPE certificates, parse course hours, categorize by type

**Day 7: Landing Page + Test**
- Launch landing page with demo video
- Cold email 50 mid-market firms with personalized "your CPAs at risk" report
- Manual onboarding for first 2 firms

## Tech Stack:
- **Backend**: Python (FastAPI), Postgres, Redis (caching)
- **AI**: Claude API (board rule parsing), GPT-4 Vision (certificate extraction)
- **Scraping**: Playwright (JavaScript-heavy board sites), proxies for rate limiting
- **Frontend**: Next.js 14, shadcn/ui components
- **Infrastructure**: AWS (ECS for containers, RDS Postgres, S3 for document storage)
- **Integrations**: API connections to Caseware, Thomson Reuters (planned)

## Monthly Revenue Potential (Year 1-3):

**Year 1 (Conservative):**
- 20 small firms @ $299/mo = $5,980 MRR
- 10 mid-market firms @ $799/mo = $7,990 MRR
- 1 large firm @ $2,499/mo = $2,499 MRR
- 500 individual CPAs @ $19/mo = $9,500 MRR
- **Total Year 1 MRR: ~$26,000 → $312K ARR**

**Year 2 (Moderate Growth):**
- 100 small firms @ $299/mo = $29,900 MRR
- 40 mid-market firms @ $799/mo = $31,960 MRR
- 10 large firms @ $2,499/mo = $24,990 MRR
- 5,000 individual CPAs = $95,000 MRR
- CPE provider rev share: $20,000 MRR
- **Total Year 2 MRR: ~$200,000 → $2.4M ARR**

**Year 3 (Market Penetration):**
- 300 small firms (10% of market) = $89,700 MRR
- 150 mid-market firms (12% of market) = $119,850 MRR
- 50 large firms = $124,950 MRR
- 30,000 CPAs = $570,000 MRR
- CPE provider rev share: $100,000 MRR
- **Total Year 3 MRR: ~$1,000,000 → $12M ARR**

## Risk Factors:
- **State board website changes**: Scraping breakage, 50 separate parsers to maintain
- **Competitive threat**: Existing CPE trackers (CPE Link, Surgent), but none do multi-state license compliance
- **Data accuracy**: Wrong CPE calculation = compliance liability for firm
- **Firm adoption speed**: Accounting industry conservative, multi-month sales cycles
- **Big 4 competition**: Large firms may build in-house solutions
- **State rule complexity**: Some states have highly specific CPE requirements (e.g., "must include taxation of pass-through entities")

## Competitive Threat:
- **CPE Link / Surgent / Becker**: CPE platforms with tracking, but license renewal is secondary feature
- **State board portals**: Each state has online lookup, but no cross-state tracking or proactive alerts
- **Firm homegrown**: Most firms use spreadsheets today (fragile, error-prone)
- **Accounting software integrations**: Thomson Reuters, CCH have compliance modules but are clunky and expensive

**Differentiation:**
- **AI-powered rule interpretation**: Only product that understands 50-state regulatory nuances
- **Multi-state focus**: Purpose-built for CPAs licensed in multiple states (growing segment)
- **CPE matching**: Only product that matches completed courses to specific state requirements
- **Firm-first design**: Built for firm compliance workflows, not individual CPAs
- **Price advantage**: 10x cheaper than enterprise compliance suites

## Go-to-Market Strategy:
**Phase 1 (Months 1-3): Firm Direct Sales**
- Target mid-market regional firms ($5-50M revenue)
- Cold outreach with personalized "at-risk CPA" reports
- Offer free pilot: "We'll track your top 50 staff for 30 days, show you compliance gaps"
- Case study from each success

**Phase 2 (Months 4-6): Association Partnerships**
- Partner with state CPA societies (50 state societies)
- Offer member discount through society
- Conference presence: AICPA ENGAGE, state society annual meetings
- CPE provider partnerships (placement recommendations)

**Phase 3 (Months 7-12): Enterprise Expansion**
- Target Big 4 firms with enterprise offering
- API launch for integration with practice management systems
- Individual CPA launch (firm-sponsored accounts)
- Viral content: "CPA License Horror Stories" LinkedIn series
