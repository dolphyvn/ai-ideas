# AI Venture Spec

## Name:
**Physical Therapy Billing AI**

## Core Concept:
AI-powered denial prevention and billing optimization for physical therapy clinics. Handles Medicare's complex 8-minute rule, G-code reporting, therapy caps, and documentation requirements to maximize reimbursement and minimize audit risk.

## Problem:
- **Medicare 8-minute rule**: Complex billing logic causes 30%+ denial rates
- **G-code hell**: Functional reporting requirements are error-prone
- **Therapy caps**: Automated tracking needed to avoid claim denials
- **Audit risk**: Medicare audits target PT billing aggressively
- **Staff burden**: Small clinics can't afford billing specialists

## Target Vertical:
**Primary**: Independent and small-chain PT clinics
- Solo practitioners (1-5 therapists)
- Small practices (5-20 therapists)
- Underserved by enterprise billing solutions

**Secondary**: Occupational therapy, speech therapy practices

## Why Now:
1. **Medicare complexity**: Billing rules increasingly complex
2. **Audit pressure**: Medicare recovery audit contractors targeting PT
3. **Staff shortage**: Billing specialists scarce/expensive
4. **EHR fragmentation**: Many PTs use basic EMRs without billing logic
5. **AI capability**: Long-context models can parse session notes accurately

## AI Advantage:
- **Session note analysis**: Extracts billable activities from documentation
- **8-minute rule engine**: Automatically calculates correct billing units
- **G-code generation**: Creates compliant functional reporting
- **Cap tracking**: Monitors therapy cap utilization across patients
- **Denial prediction**: Flags high-risk claims before submission
- **Audit protection**: Documentation review for compliance

## Viral Mechanism:
- **PT community networks**: High referral rates
- **Association channels**: APTA, state chapters
- **Revenue recovery stories**: "Saved my practice $50K in denials"
- **Audit survival**: "Passed Medicare audit thanks to AI"

## Revenue Model:
**Per-Clinic Subscription:**
- **Solo**: $499/month - 1-3 therapists
- **Practice**: $1,299/month - 4-15 therapists
- **Multi-location**: $2,999/month - 16+ therapists

**Implementation:**
- $1,500 one-time (workflow setup, EMR integration)

**Unit Economics:**
- CAC: $300 (PT conferences, referrals)
- LTV: $18,000 (36-month avg)
- Gross Margin: 85%

## Moat:
1. **Medicare billing expertise**: 8-minute rule logic is complex
2. **PT-specific codes**: G-codes, modifiers, therapy caps
3. **Audit track record**: Proven protection = valuable
4. **EMR integration depth**: WebPT, TheraOffice integrations
5. **Outcome data**: Denied claims database improves prediction

## MVP in 7 Days:
**Days 1-2:**
- Manual process: PT sends session notes
- Manual analysis of billable units

**Days 3-4:**
- Claude 4.6 for note analysis
- Build 8-minute rule calculator
- G-code suggestion engine

**Days 5-7:**
- Beta with 1 solo PT practice
- Compare AI billing vs. actual billing
- Measure: Additional units captured, denials prevented

**Validation Metric:**
- 1 solo PT willing to pay
- 10%+ revenue increase identified
- Zero compliance issues flagged

## Tech Stack:
- **Backend**: Python/FastAPI
- **AI**: Claude 4.6 (note analysis), GPT-4o (code generation)
- **Integrations**: WebPT API, TheraOffice
- **Database**: PostgreSQL (claims data), Qdrant (denial patterns)
- **Infrastructure**: AWS ECS

## Monthly Revenue Potential (Year 1–3):
- **Year 1**: $30K MRR (50 clinics × $600 ARPU)
- **Year 2**: $150K MRR (250 clinics)
- **Year 3**: $500K MRR (1,000 clinics + enterprise)

## Risk Factors:
1. **Medicare regulation changes**: Rules could simplify (unlikely)
2. **EMR competition**: WebPT could build this
3. **Low ARPU**: Small clinics have budget constraints
4. **Compliance risk**: Wrong advice = audit liability
5. **Market size**: Limited PT clinics nationally (~20K)

## Competitive Threat:
- BetterPT (scheduling, not billing)
- WebPT (EMR with basic billing, not AI-optimized)
- DrChrono (general medical, not PT-specific)

**Differentiation**: PT billing is a specialty - generalists miss nuances

---

## Agent Evaluation Summary

**Score: 8.75/10 - PURSUE** ✅

**Strengths:**
- Extreme specificity (PT only, not "healthcare billing")
- Medicare complexity creates moat
- Underserved solo/small practice market
- Audit risk creates urgency
- Higher complexity than dental = stronger moat

**Weaknesses:**
- Limited TAM (~20K PT clinics)
- Low ARPU (small practices)
- EMR competition risk

**Why this meets threshold:**
- True vertical (PT-specific billing rules)
- Regulatory complexity (Medicare 8-minute rule)
- Underserved market segment
- High retention (billing is mission-critical)

## Go/No-Go Decision: **GO** ✅

**Path forward:**
1. Solo PT practice wedge (underserved)
2. Medicare focus (highest complexity)
3. Prove 10%+ revenue lift
4. Expand to OT/Speech after PMF

**Note**: This is the right type of vertical AI - highly specialized, regulatory complexity, underserved niche.
