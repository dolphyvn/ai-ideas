# AI Venture Spec

## Name:
**OncologyPriorAuthAI - Oncology Prior Authorization Platform**

## Core Concept:
AI-powered platform for oncology practices that automates cancer drug prior authorizations, step therapy navigation, appeals, and genomic testing authorization.

## Problem:
- **2,000+ oncology practices** in US
- **30+ cancer drugs** require prior authorization (growing)
- **Step therapy**: Fail-first protocols delay treatment (life-or-death for cancer)
- **Genomic testing**: FoundationOne, Guardant360 require prior auth ($3K-$8K tests)
- **Appeal burden**: 40%+ denials require appeals (manual process)
- **Treatment delays**: Prior auth delays = 2-4 weeks (cancer progression risk)

## Target Vertical:
**Primary:** Oncology Practices
- Community oncology practices (independent, mid-size)
- Hospital-based oncology departments
- Oncology networks (US Oncology, The US Oncology Network)

**Secondary:** Cancer centers, infusion centers, oncology pharmacists

## Why Now:
1. **Prior auth explosion**: 70%+ of cancer drugs require prior auth (up from 40% in 2020)
2. **Step therapy**: Payers requiring fail-first for cancer drugs (ethical controversy)
3. **Genomic testing boom**: Companion diagnostics required for targeted therapies
4. **Appeal automation**: Payers automating denials, practices must automate appeals
5. **Cancer drug cost**: $10K-$100K+ per course = payer scrutiny

## AI Advantage:
- **Prior auth automation**: AI completes payer-specific prior auth forms (clinical documentation)
- **Step therapy navigation**: AI identifies step therapy exceptions, generates appeal letters
- **Genomic testing auth**: AI justifies molecular testing (NCCN guidelines, biomarker evidence)
- **Appeal generation**: Auto-generates appeal letters (peer-to-peer talking points)
- **Clinical guideline matching**: AI matches patient to NCCN/ASCO guidelines (prior auth support)
- **Payer rule tracking**: AI tracks changing payer policies (prior auth requirements)

## Viral Mechanism:
- **ASCO conferences**: American Society of Clinical Oncology annual meeting
- **Oncology community**: Tight-knit, word-of-mouth
- **Case studies**: "Reduced prior auth time 70%, got patient treatment 2 weeks faster"
- **Patient outcomes**: "Treatment not delayed by prior auth" = powerful

## Revenue Model:
**Per-Practice Subscription:**
- **Community**: $2,000/month - 1-10 oncologists, prior auth automation
- **Network**: $5,000/month - 11+ oncologists, unlimited + genomic testing + appeal module
- **Enterprise**: $10,000/month - Multi-location + white-label + EMR integration + payer rule feed

**Per-Prior-Auth add-on:**
- $50 per complex prior auth (beyond included tiers)

**Implementation:**
- $10,000 one-time (payer rule setup, EMR integration, training)

**Unit Economics:**
- CAC: $300 (ASCO conferences, oncology society partnerships)
- LTV: $72,000 (36-month retention - switching costs extreme)
- Gross Margin: 80%

## Moat:
1. **Oncology drug complexity**: 30+ cancer drugs, combination therapies, clinical trials
2. **Payer rules**: Each payer has different prior auth criteria (changing)
3. **Step therapy exceptions**: Cancer-specific exceptions, clinical trial enrollment
4. **Genomic testing**: Molecular biomarkers, companion diagnostics, NCCN guidelines
5. **Appeal expertise**: Peer-to-peer talking points, medical literature citations

## MVP in 12 Weeks:
**Weeks 1-3:**
- Focus: Top 10 cancer drugs only (Keytruda, Opdivo, etc.)
- ONE payer (UnitedHealthcare - largest)
- Manual prior auth workflow

**Weeks 4-6:**
- Build AI prior auth completer (UHC criteria)
- Step therapy exception identifier
- Appeal letter generator

**Weeks 7-9:**
- Partner with 3 community oncology practices
- Deploy pilot for top 10 drugs + UHC
- Validate: Prior auth approval rate, time reduction

**Weeks 10-12:**
- Add 5 more payers (Aetna, Cigna, Humana, BCBS, Medicare Advantage)
- Genomic testing prior auth
- Prepare ASCO conference demo

**Validation Metrics:**
- 70%+ reduction in prior auth time
- 95%+ prior auth approval rate (vs. 80% baseline)
- 2+ practices commit after pilot
- One step therapy exception granted using AI appeal

## Tech Stack:
- **Backend**: Python/FastAPI
- **AI**: GPT-4 (prior auth completion, appeal letters), Custom ML (payer rule tracking)
- **Integrations**: Oncology EMRs (Flatiron, Elekta), payer portals, NCCN/ASCO guidelines
- **Infrastructure**: AWS (US regions, HIPAA compliant)

## Monthly Revenue Potential (Year 1–3):
- **Year 1**: $24K MRR (12 practices × $2K ARPU)
- **Year 2**: $120K MRR (60 practices + networks)
- **Year 3**: $360K MRR (180 practices + enterprise)

## Risk Factors:
1. **Payer rules**: Prior auth requirements change frequently
2. **Payer resistance**: Payers may tighten step therapy, deny appeals
3. **Clinical trials**: Clinical trial enrollment adds complexity
4. **Oncology consolidation**: Practices selling to hospitals/US Oncology
5. **Liability risk**: Wrong prior auth = delayed treatment

## Competitive Threat:
- **Prior auth platforms**: SamaCare (prior auth for oncology), CoverMyMeds (general)
- **Oncology EMRs**: Flatiron Health (prior auth features), Elekta (not focused)
- **Prior auth services**: SamaCare = competitor

**Differentiation**: Only AI platform for oncology prior auth with step therapy exception handling, genomic testing authorization, and appeal automation.

---

## Agent Evaluation Summary

**Score: 8.6/10 - PURSUE** ⭐ **TOP CYCLE 24, TOP 15 ALL-TIME**

**Strengths:**
- **Life-or-death urgency**: Cancer treatment delays = progression risk
- **Prior auth explosion**: 70%+ of cancer drugs require prior auth
- **Step therapy pain**: Fail-first for cancer = ethical controversy + delays
- **Genomic testing**: $3K-$8K tests require prior auth
- **High revenue per practice**: Oncology = high-revenue specialty
- **Tight community**: ASCO conferences, word-of-mouth

**Weaknesses:**
- Payer rules change frequently
- Oncology consolidation (practices selling)
- Competition exists (SamaCare)

**Why this scores 8.6:**
- **Cancer = life-or-death** = extreme urgency
- **Prior auth explosion** = growing pain (70%+ require auth)
- **Step therapy** = ethical controversy + media attention
- **Genomic testing** = new complexity (companion diagnostics)
- **$10K-$100K drugs** = high stakes

**Top 15 All-Time opportunity.**

## Go/No-Go Decision: **GO** ✅

**Critical success factors:**
1. Hire oncologists/oncology practice managers as co-founders/advisors
2. Start with top 10 cancer drugs (Keytruda, Opdivo, etc.)
3. Partner with ASCO for distribution
4. Build step therapy exception module (key differentiator)
5. Add genomic testing auth (emerging complexity)

**Outstanding oncology prior authorization opportunity.**
