# AI Venture Spec

## Name:
**AI DNA Prevention & Smart Scheduling Engine**

## Core Concept:
Predictive appointment scheduling for NHS trusts that integrates with EMIS/SystmOne to identify high-risk DNAs (Did Not Attend), optimize slot allocation, and automate personalized reminder sequences. Reduces the £1.9B annual cost of missed appointments.

## Problem:
- **£1.9B annually** in missed appointments (11.8M missed appointments/year)
- **Guy's & St Thomas' alone loses £51.4M** to DNAs annually
- **8 million missed elective care appointments** (2023/24)
- **1 in 3 people miss screening appointments**
- **Current reminder systems are generic** (SMS blasts, no personalization)

## Target Vertical:
**Primary**: NHS Trusts (144 acute trusts)
- High-DNA specialties: dermatology, ophthalmology, orthopaedics
- Outpatient departments (highest DNA volume)
- Screening programs (breast, bowel, cervical)

**Secondary**: NHS Integrated Care Boards (42 ICBs)
- Commissioning groups with DNA reduction targets
- Regional coordination of scheduling

## Why Now:
1. **2026 AI capability**: Long-context models can predict DNA risk from patient history
2. **NHS APIs mature**: EMIS/SystmOne appointment booking APIs established
3. **Budget pressure**: Trusts desperate for cost savings
4. **Procurement frameworks**: NHS AI Lab funding, Digital Capability for Health 2
5. **Proven ROI**: 73% waiting time reduction where AI deployed (Chelsea & Westminster)

## AI Advantage:
- **DNA risk prediction**: Analyzes patient history (age, deprivation, past DNA, weather, transport)
- **Smart scheduling**: Optimizes slot allocation (high-risk patients get prime slots)
- **Personalized reminders**: Multi-channel (SMS, email, NHS App, phone) based on patient preference
- **Real-time optimization**: Fills cancelled slots with high-priority waitlist patients
- **Learning system**: Improves predictions with each appointment

## Viral Mechanism:
- **NHS case studies**: "Saved £8M annually" spreads via NHS networks
- **ICB referrals**: Integrated Care Boards share results regionally
- **NHS conferences": NHS Confed, Health Innovation Conference
- **Government validation**: NHS AI Lab endorsement = trust signal

## Revenue Model:
**Per-Trust Subscription:**
- **Standard**: £75K/year - Single hospital, basic predictions
- **Trust**: £150K/year - Multiple hospitals, full optimization
- **ICB**: £400K/year - Region-wide, across all GP practices

**Implementation:**
- £25K one-time (EMIS/SystmOne integration, model training)

**Unit Economics:**
- CAC: £75K (NHS conferences, ICB outreach, case studies)
- LTV: £450K (36-month retention, multi-year contracts)
- Gross Margin: 75%

## Moat:
1. **Patient data**: Historical appointment data improves predictions
2. **Integration depth**: Deep hooks into EMIS/SystmOne booking systems
3. **NHS procurement**: Framework approval = barrier to entry
4. **Learning system**: More trusts = better models
5. **Switching costs**: Re-training models on new data is expensive

## MVP in 16 Weeks:
**Weeks 1-4:**
- Focus: ONE high-DNA specialty (dermatology outpatient)
- Partner with Guy's & St Thomas' (already measuring DNA cost)
- Manual DNA risk prediction from historical data

**Weeks 5-8:**
- Build prediction model (age, deprivation, past DNA, weather)
- Integrate EMIS appointment booking API
- Deploy reminder automation (SMS, NHS App)

**Weeks 9-12:**
- Pilot with Guy's dermatology department
- Measure: DNA rate reduction target 15%
- ROI calculation: £ saved vs. system cost

**Weeks 13-16:**
- Expand to 2 more departments
- Add real-time slot optimization
- Prepare ICB regional rollout

**Validation Metrics:**
- 15%+ DNA reduction (industry target is 10%)
- £8M+ annual savings for Guy's
- Payback period <3 months
- 2+ additional trusts commit after pilot

## Tech Stack:
- **Backend**: Python/FastAPI
- **AI**: XGBoost (DNA risk prediction), Claude 4.6 (personalization)
- **Integrations**: EMIS Web API, SystmOne GP Connect
- **Messaging**: NHS App API, SMS gateway, email
- **Infrastructure**: AWS London Region (data residency)

## Monthly Revenue Potential (Year 1–3):
- **Year 1**: £125K MRR (10 trusts × £12.5K ARPU/month)
- **Year 2**: £625K MRR (50 trusts + 3 ICBs)
- **Year 3**: £1.75M MRR (140 trusts + 20 ICBs)

## Risk Factors:
1. **EMIS/SystmOne dependency**: Both could shut off API access
2. **NHS procurement complexity**: 12-24 month sales cycles
3. **Data governance**: NHS data protection requirements
4. **Political risk**: NHS England may build nationally
5. **Clinical adoption**: Staff may resist algorithmic scheduling

## Competitive Threat:
- **EMIS/SystmOne**: Building AI features, but focused on clinical (not scheduling)
- **Accurx**: Patient messaging, not prediction/optimization
- **NHS Federated Data Platform**: Palantir vendor, analytics-focused
- **Current reminder systems**: Generic SMS blasts, no intelligence

**Differentiation**: Predictive + optimization + personalization, not just reminders

## NHS Integration Strategy:
- **GP Connect API**: Standardised access to appointment data
- **NHS AI Lab**: Pre-commercial procurement funding available
- **Digital Capability for Health 2**: National procurement framework
- **Local pilots**: Trust-level procurement (faster than national)

---

## Agent Evaluation Summary

**Score: 8.8/10 - PURSUE** ⭐ **TIES FOR #1 ACROSS ALL CYCLES**

**Strengths:**
- **Massive validated pain**: £1.9B annually, 11.8M missed appointments
- **Clear ROI**: 10% DNA reduction = £8M savings for Guy's, payback <3 months
- **Integration feasible**: EMIS/SystmOne APIs established
- **Procurement-friendly**: Budget-neutral via savings, frameworks available
- **Low clinical risk**: Administrative (not diagnostic) = faster regulatory path
- **No incumbent threat**: EMIS/SystmOne focused on clinical features

**Weaknesses:**
- EMIS/SystmOne dependency (could build competing features)
- NHS procurement complexity (12-24 month cycles)
- Data governance requirements

**Why this ties for #1:**
- **Massive TAM**: £190-380M/year (10-20% of DNA cost)
- **Budget-neutral**: Pays for itself in savings
- **NHS-specific**: Deep integration knowledge required
- **Urgent**: Trusts desperate for cost savings
- **Proven**: Chelsea & Westminster showed 73% improvement with admin AI

## Go/No-Go Decision: **GO** ✅

**Critical success factors:**
1. Start with high-DNA specialties (dermatology, ophthalmology)
2. Pilot with innovation-friendly trusts (Guy's, Manchester, Barts)
3. Leverage NHS AI Lab funding for pre-commercial procurement
4. Build integration with BOTH EMIS and SystmOne (don't pick sides)

**This is the top NHS AI opportunity and ties for #1 overall across all cycles.**

---

## Sources:
- [NHS Missed Appointments Statistics](https://www.england.nhs.uk/2024/12/millions-of-people-receiving-screening-and-appointment-reminders-on-mobile-phones/)
- [NHS AI Automation Admin Tasks](https://www.bma.org.uk/news/the-nhs-is-tackling-admin-burden-by-trialling-ai-driven-discharge-summary-tool/)
- [NHS Winter Crisis AI Tools](https://www.telegraph.co.uk/news/2025/12/16/ai-used-across-nhs-predict-emergency-department-demand/)
- [NHS AI Implementation Study](https://www.ucl.ac.uk/health-informatics/news/2025/jan/nhs-ai-implementation-takes-10-months-longer)
