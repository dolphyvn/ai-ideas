# AI Venture Spec

## Name:
**OfferOptimizer - Salary Negotiation AI**

## Core Concept:
AI that analyzes job offers and generates personalized negotiation scripts. Users upload offer letters (PDF or text), and the AI benchmarks salary against market data, identifies negotiable elements beyond base salary, generates negotiation email/call scripts, practices negotiations via voice AI, and provides counter-offer simulations.

## Problem:
- **Money left on table**: 70% of negotiators don't negotiate their first offer
- **Average loss**: $5K-$20K+ in first-year compensation
- **Negotiation anxiety**: People don't know what to say or ask for
- **Information asymmetry**: Don't know market value or what's negotiable
- **Coaching is expensive**: Career coaches charge $300+/hour

## Target Vertical:
**Primary**: Active job seekers in knowledge worker roles
- Tech workers (software engineers, product managers, data scientists)
- Consultants, finance professionals, marketing leaders
- Recent graduates, career switchers, people in high COL areas

**Secondary**: Internal offer reviews, promotion negotiations, contractor rate setting

## Why Now:
1. **Salary transparency laws**: More states requiring salary ranges in postings
2. **AI voice capability**: Realistic conversation practice is now feasible
3. **Job market volatility**: More frequent job changes = more negotiations
4. **Compensation complexity**: Equity, RSUs, sign-on bonuses are more common
5. **Remote work arbitrage**: Location-based pay creates negotiation opportunities

## AI Advantage:
- **Market data synthesis**: Aggregates salary data from multiple sources (Levels.fyi, Glassdoor, Blind, LinkedIn)
- **Pattern recognition**: Identifies negotiable elements humans miss
- **Personalization**: Tailors scripts to user's experience, leverage, industry
- **Real-time practice**: Voice AI can roleplay negotiations with infinite variations
- **Counter-offer simulation**: Models employer responses and suggests countermoves

## Viral Mechanism:
- **Direct ROI sharing**: "I got $15K more using AI" posts are extremely shareable
- **Salary screenshots**: Before/after offer comparisons (anonymized)
- **LinkedIn testimonials**: Users share when they land better offers
- **TikTok breakdowns**: "Watch me negotiate my salary using AI"
- **Recruiter responses**: "This candidate negotiated professionally"
- **Annual savings**: "This $49 app made me $50K over 3 years"

## Revenue Model:
**Consumer Pay-Per-Use:**
- **Free analysis**: Market benchmarking only
- **Single offer**: $49 one-time - full analysis + scripts + practice
- **Job search bundle**: $99/month - unlimited offers for 3 months

**Premium Features:**
- **Voice practice**: +$20 per offer (unlimited AI conversations)
- **Equity analysis**: +$30 for RSU/option modeling
- **Success fee model**: 10% of additional salary negotiated (optional, capped at $2K)

**Unit Economics:**
- CAC: $60 (LinkedIn content, Reddit communities, TikTok)
- LTV: $150 (average 2-3 offers during job search)
- Gross Margin: 85%

**B2B2C Partnerships:**
- **Career centers**: $10K/year site license (universities)
- **Outplacement firms**: $25K/year (for laid-off worker services)

## Moat:
1. **Offer database**: Aggregate negotiation outcomes (what worked)
2. **Compensation models**: Accurate total comp modeling (equity, benefits)
3. **Company-specific patterns**: Learn each company's negotiation flexibility
4. **Voice AI training data**: Realistic negotiation conversations
5. **Market data partnerships**: Exclusive access to salary benchmarks

## MVP in 7 Days:
**Days 1-2:**
- PDF/OCR parser for offer letters
- Base salary benchmarking (scrape public data)
- Basic script generation via Claude API

**Days 3-4:**
- Negotiable element detection (sign-on, equity, benefits, PTO)
- Script templates (email, phone, in-person)
- Counter-offer response simulation

**Days 5-7:**
- Simple web app for offer upload
- Voice practice using ElevenLabs/OpenAI voice
- Beta testing with 10 active job seekers
- TikTok content: "I got $10K more" stories

**Validation Metrics:**
- 20+ offers analyzed
- 5+ users attempt negotiations
- 2+ users report higher compensation (any amount)
- 1+ viral LinkedIn/TikTok post

## Tech Stack:
- **Backend**: Python/FastAPI
- **AI**: Claude 4.6 for analysis, GPT-4 for scripts
- **Voice**: ElevenLabs API or OpenAI Voice
- **Data Scraping**: BeautifulSoup, Selenium for salary data
- **Frontend**: Next.js (web-first, mobile responsive)
- **Infrastructure**: AWS ECS, Postgres, Redis

## Monthly Revenue Potential (Year 1-3):
- **Year 1**: $30K MRR (600 offers/month × $50 ARPU)
- **Year 2**: $150K MRR (3,000 offers/month × $50 ARPU)
- **Year 3**: $500K MRR (10,000 offers/month × $50 ARPU)
- **Enterprise**: Additional $50K MRR in Year 2

## Risk Factors:
1. **One-time use**: High churn after job landed (mitigate with career-long tools)
2. **Legal sensitivity**: AI advice could be seen as legal/financial counsel
3. **Platform risk**: LinkedIn could restrict API access
4. **Competition**: Some free tools exist, Salary.com has data
5. **Cultural resistance**: Some demographics won't negotiate

## Competitive Threat:
- **Levels.fyi**: Data but no coaching
- **Glassdoor**: Market data but no personalization
- **Career coaches**: Better but expensive ($300+/hour)
- **Free negotiation scripts**: Generic, not personalized

**Differentiation**: Personalized scripts + voice practice + market data in one product

---

## Go/No-Go Decision: **GO** (9/10)

**Rationale:**
- Highest viral potential in B2C category (money results are shareable)
- Clear ROI demonstration ($49 to make $5K+ is obvious)
- Large TAM with consistent demand (job changes are constant)
- Low technical risk (straightforward AI implementation)
- High willingness to pay during high-stress life event

**Conditional factors:**
- Must validate that users actually negotiate (not just analyze)
- Need to ensure market data is accurate enough for trust
- Voice practice must feel realistic or users won't use it

**Next steps**: 7-day MVP sprint with 10 beta testers
