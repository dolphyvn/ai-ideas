# CathLabAI - Interventional Cardiology Platform

**Venture Spec Created:** 2026-03-02

---

## Executive Summary

CathLabAI is an AI-powered platform for interventional cardiologists that automates cardiac catheterization interpretation, coronary anatomy analysis from angiograms, PCI planning, stent sizing, FFR prediction, and structural heart procedure guidance. With 15,000+ interventional cardiologists in the US and 1M+ cardiac catheterization procedures annually, this represents one of the largest AI opportunities in credentialized medicine.

**Go/No-Go Decision: GO**

**Agent Evaluation Score: 8.00/10**

---

## 1. Core Concept

AI-powered platform for interventional cardiologists that provides:

- **Automated Angiogram Interpretation:** Computer vision analysis of coronary anatomy with stenosis percentage estimation
- **Stent Sizing Optimization:** AI-recommended stent diameter and length based on vessel measurements
- **PCI Planning:** Procedural guidance including access site selection, device selection, and step-by-step guidance
- **FFR Prediction:** Non-invasive fractional flow reserve estimation from angiogram data
- **Structural Heart Guidance:** TAVR sizing, MitraClip planning, and other structural heart procedure support
- **Outcomes Prediction:** Risk stratification for procedural success and complications

---

## 2. Problem Statement

### Market Pain Points

| Problem | Impact | Current Solution |
|---------|--------|------------------|
| **Subjective Angiogram Interpretation** | Visual estimation leads to 30%+ variability in stenosis assessment | QCA (quantitative coronary angiography) - time-consuming, not universally used |
| **Stent Sizing Errors** | Underexpansion = 15% restenosis rate; Malapposition = stent thrombosis risk | Operator experience + visual estimation |
| **Variable PCI Outcomes** | 30-day MACE rates vary 2-3x by operator | Experience-dependent, no standardization |
| **FFR Underutilization** | Only 20-30% of lesions get FFR assessment (cost, time, wire) | Invasive FFR = additional cost, time, risk |
| **Structural Heart Complexity** | TAVR sizing errors = paravalvular leak, migration | CT angiography + operator judgment |
| **Cath Lab Efficiency** | 15-20% of procedures have delays for additional imaging | N/A |

### Market Statistics

- **15,000+** interventional cardiologists in the US (largest specialty cohort)
- **1,000,000+** cardiac catheterization procedures annually in the US
- **600,000+** PCI (stent) procedures annually in the US
- **200,000+** structural heart procedures annually (TAVR, MitraClip, etc.)
- **$20B+** annual US market for interventional cardiology procedures
- **CAD is the #1 killer worldwide** (17.9M deaths/year)

---

## 3. Target Vertical

### Primary Users: Interventional Cardiologists

| Segment | Size | Priority | Needs |
|---------|------|----------|-------|
| **Cath Lab Directors** | 2,000+ | High | Lab efficiency, outcomes tracking, ROI justification |
| **Interventional Cardiologists** | 13,000+ | High | Stent sizing accuracy, PCI planning, efficiency |
| **Structural Heart Specialists** | 1,500+ | Medium | TAVR sizing, complex procedure planning |
| **Fellows in Training** | 800+ | Medium | Education, case review, skill development |

### Secondary Users: Institutions

| Segment | Decision Maker | Priority |
|---------|----------------|----------|
| **Hospital Cath Labs** | Cath Lab Director, Cardiology Chair | High |
| **Structural Heart Programs** | Program Director | Medium |
| **Academic Medical Centers** | Department Chair, Research Director | Medium |
| **Private Practice Groups** | Managing Partner | High |

---

## 4. Why Now

### Market Timing Factors

1. **Increasing CAD Prevalence**
   - Diabetes, obesity, aging population driving growth
   - 38% of US adults have metabolic syndrome
   - 10,000 Baby Boomers turn 65 daily

2. **PCI Expansion**
   - High-risk PCI becoming more common (cath lab-based support)
   - Complex lesion treatment increasing (CTO, bifurcation, left main)
   - "Leave nothing behind" trend (DCB, IVUS/OCT guidance)

3. **Structural Heart Growth**
   - TAVR volume growing 15-20% annually
   - MitraClip, tricuspid, mitral valve devices expanding
   - Congenital/structural interventions increasing

4. **AI/Computer Vision Breakthroughs**
   - CNN architectures proven for medical imaging
   - 3D reconstruction from 2D angiography now feasible
   - Real-time inference possible with modern GPUs

5. **Cath Lab Modernization**
   - Philips, GE, Siemens investing in AI integration
   - PACS interoperability improving
   - Cloud-based imaging adoption accelerating

---

## 5. AI Advantage

### Core AI Capabilities

#### 1. Angiogram Computer Vision
- **Input:** Standard 2D angiography images (DICOM)
- **Processing:** CNN-based vessel segmentation, stenosis detection
- **Output:** Coronary anatomy map, stenosis percentages, vessel diameters
- **Accuracy Target:** <10% error vs. QCA (quantitative coronary angiography)

#### 2. Stent Sizing ML
- **Input:** Vessel measurements, lesion characteristics, patient factors
- **Processing:** Ensemble models for diameter and length prediction
- **Output:** Optimal stent selection (size, length, type)
- **Validation:** vs. IVUS/OCT measurements

#### 3. FFR Prediction
- **Input:** Angiogram-derived vessel geometry, flow estimates
- **Processing:** Physics-informed neural networks
- **Output:** Lesion-specific FFR estimate
- **Target:** 0.85 ROC AUC vs. invasive FFR

#### 4. PCI Outcome Prediction
- **Input:** Patient comorbidities, lesion complexity, operator experience
- **Processing:** Gradient boosting on structured + imaging data
- **Output:** Success probability, complication risk
- **Use Case:** Pre-procedure risk stratification

#### 5. Structural Heart Planning
- **Input:** CT angiography, angiograms, echo data
- **Processing:** 3D model generation, device simulation
- **Output:** TAVR valve size, MitraClip sizing, access planning
- **Integration:** Pre-procedure planning workflows

---

## 6. Viral Mechanism

### Professional Networks

| Channel | Reach | Strategy |
|---------|-------|----------|
| **SCAI (Society for Cardiovascular Angiography and Interventions)** | 4,000+ members | Annual conference demos, sponsored research, abstract submissions |
| **TCT (Transcatheter Cardiovascular Therapeutics)** | 10,000+ attendees | Late-breaking clinical trials, AI showcase, hands-on demos |
| **ACC (American College of Cardiology)** | 50,000+ members | Innovation showcase, scientific sessions |
| **EuroPCR** | 12,000+ European attendees | International expansion, European clinical data |

### Referral Networks

- **Cath Lab Director Network:** 2,000 influencers, high referral value
- **Fellowship Programs:** 180+ programs, training next generation
- **Key Opinion Leaders (KOLs):** Top 100 ICs drive adoption
- **Case Study Diffusion:** "This AI caught an under-expanded stent"
- **Social Proof:** Published outcomes data

### Content Marketing

- **Case Studies:** Real-world angiogram analyses
- **Webinars:** "AI in the Cath Lab" series
- **Podcasts:** IC thought leader interviews
- **Journal Publications:** JACC: Cardiovascular Interventions, Circulation: Cardiovascular Interventions

---

## 7. Revenue Model

### Per-Cath Lab Subscription (B2B SaaS)

| Tier | Monthly Price | Features | Target |
|------|---------------|----------|--------|
| **Starter** | $1,500/month | Angiogram AI, stent sizing, basic reporting | Small community hospitals |
| **Professional** | $2,500/month | Full suite + PCI planning + outcomes tracking | Mid-size hospitals, academic centers |
| **Enterprise** | $5,000/month | Multi-lab + structural heart + research + API access | Large systems, research hospitals |

### Per-Procedure Add-on

- **AI-Assisted PCI:** $25 per procedure (beyond included tiers)
- **Structural Heart Case:** $50 per TAVR/MitraClip planning
- **FFR Prediction:** $15 per non-invasive assessment

### Unit Economics

| Metric | Value |
|--------|-------|
| **CAC** | $200 (SCAI/TCT conferences, demos) |
| **LTV** | $90,000 (36-month avg retention, high switching costs) |
| **LTV:CAC** | 450:1 |
| **Gross Margin** | 85% (software, low variable cost) |
| **ARPU** | $2,500/month (Professional tier weighted avg) |
| **Payback Period** | <1 month |

### Monthly Revenue Potential

| Year | Labs | ARPU | MRR | ARR |
|------|------|------|-----|-----|
| **Year 1** | 12 | $2,500 | $30,000 | $360,000 |
| **Year 2** | 60 | $2,750 | $165,000 | $1,980,000 |
| **Year 3** | 180 | $3,000 | $540,000 | $6,480,000 |
| **Year 5** | 450 | $3,250 | $1,462,500 | $17,550,000 |

---

## 8. MVP in 8 Weeks

### Week 1-2: Data Collection & Partnerships

**Goals:**
- Secure one cath lab partnership
- Establish data use agreements
- Collect 500+ angiograms with QCA ground truth
- Set up annotation pipeline

**Deliverables:**
- Data partnership agreement signed
- DICOM ingestion pipeline operational
- Annotation schema finalized
- IRB approval (if needed for research use)

### Week 3-5: Core AI Model Development

**Goals:**
- Build coronary anatomy segmentation CNN
- Develop stenosis percentage estimation
- Create vessel diameter measurement
- Train on initial dataset

**Technical Stack:**
- PyTorch + torchvision
- U-Net architecture for segmentation
- ResNet backbone for feature extraction
- DICOM processing: pydicom, HighDicom

**Deliverables:**
- Segmentation model (vessel detection)
- Stenosis estimation model
- Initial validation metrics

### Week 6-7: Pilot & Validation

**Goals:**
- Deploy to partner cath lab
- Validate stenosis accuracy vs. QCA
- Measure interpretation time savings
- Collect user feedback

**Deployment:**
- Web-based interface for angiogram upload
- Real-time inference (<30 seconds per case)
- Side-by-side comparison with QCA

**Deliverables:**
- Pilot completed with 100+ cases
- Validation report
- User feedback summary

### Week 8: Refinement & Demo Prep

**Goals:**
- Refine model based on feedback
- Optimize for real-time performance
- Prepare TCT conference demo
- Create marketing materials

**Deliverables:**
- Production-ready MVP
- TCT demo presentation
- Marketing one-pager
- Pilot case study

### Validation Metrics

| Metric | Target | Status |
|--------|--------|--------|
| Stenosis error vs. QCA | <10% | Measured |
| Interpretation time | 50%+ faster | Measured |
| User satisfaction | 4+ / 5 | Survey |
| Pilot conversion | 1 commitment | Signed |

---

## 9. Tech Stack

### Backend

- **Language:** Python 3.11+
- **Framework:** FastAPI (async, type-safe)
- **Task Queue:** Celery + Redis (background processing)
- **Database:** PostgreSQL (relational data), Redis (cache)

### AI/ML

- **Framework:** PyTorch 2.0+
- **Computer Vision:**
  - torchvision (pre-trained models)
  - monai (medical imaging)
  - SimpleITK (DICOM processing)
- **3D Reconstruction:**
  - VTK (visualization)
  - pyvista (3D rendering)
- **NLP:**
  - GPT-4 API (report generation)
  - spaCy (medical entity extraction)

### Integrations

- **Cath Lab Systems:**
  - Philips X-ray systems (DICOM)
  - GE Healthcare (DICOM, integration APIs)
  - Siemens Healthineers (syngo via DICOM)
- **PACS:** DICOM C-STORE, C-MOVE, C-FIND
- **EHR:** HL7 FHIR, Epic Interconnect, Cerner

### Infrastructure

- **Cloud:** AWS (us-east-1, us-west-2 for HIPAA)
- **Compute:**
  - EC2 G5 instances (GPU for inference)
  - SageMaker (training pipelines)
  - Lambda (serverless preprocessing)
- **Storage:**
  - S3 (DICOM storage, encrypted)
  - EBS (database volumes)
- **Security:**
  - VPC (network isolation)
  - KMS (encryption at rest)
  - ACM (TLS certificates)
  - AWS CloudHSM (optional, for key management)

### Frontend

- **Framework:** React 18 + TypeScript
- **Medical Imaging:**
  - OHIF Viewer (DICOM visualization)
  - Cornerstone.js (annotation tools)
- **UI Components:** shadcn/ui, Tailwind CSS
- **Charts:** Recharts, D3.js

### DevOps

- **CI/CD:** GitHub Actions
- **Containerization:** Docker, ECR
- **Orchestration:** Kubernetes (EKS)
- **Monitoring:**
  - DataDog (APM, logs)
  - Sentry (error tracking)
  - Prometheus (metrics)

---

## 10. Risk Factors

### 1. FDA Regulatory Pathway

| Factor | Impact | Mitigation |
|--------|--------|------------|
| **Class II Device Required** | 12-24 month timeline, $1-2M cost | Start with 510(k) predicate strategy |
| **Clinical Validation Needed** | 100+ patient study required | Partner with academic centers early |
| **Post-Market Surveillance** | Ongoing data collection required | Build MDSAP compliance from day 1 |

### 2. Angiogram Quality Variability

| Risk | Impact | Mitigation |
|------|--------|------------|
| Poor contrast opacification | Segmentation failures | Quality assessment AI, reject/capture workflow |
| Motion artifact | Measurement errors | Motion correction preprocessing |
| Different vendors/acquisition | Model generalization | Multi-vendor training data |

### 3. Clinical Liability

| Risk | Impact | Mitigation |
|------|--------|------------|
| Stent sizing errors = complications | Malpractice exposure | Clear "decision support" labeling, physician always decides |
| False negatives (missed disease) | Patient harm | Conservative thresholds, explicit uncertainty display |
| System failure during procedure | Care delay | High availability architecture, fail-fast design |

### 4. Sales Cycle Length

| Factor | Reality | Strategy |
|--------|---------|----------|
| Hospital procurement | 12-18 month cycles | Target private practices (6-9 months) first |
| Budget approval | Multiple stakeholders | ROI calculator with case volume data |
| IT security review | 3-6 month process | SOC 2 Type II, HITRUST from day 1 |

### 5. Operator Resistance

| Barrier | Counter |
|---------|---------|
| "I've done 10,000 cases" | Focus on fellows, younger ICs |
| "AI will replace me" | Position as "autopilot not autopilot" |
| "It's wrong" | Transparency, explainable AI, show errors |
| "It slows me down" | Real-time inference, <30 sec latency |

### 6. Competitive Landscape

| Competitor | Status | Differentiation |
|------------|--------|-----------------|
| **GE Healthcare** | Cath lab AI features | Full platform, not bolt-on |
| **Philips** | Azurion AI | Vendor-neutral advantage |
| **Siemens** | syngo AI | Structural heart focus |
| **Startups (CathAI, etc.)** | Early stage | First-mover, clinical validation |

---

## 11. Competitive Threat

### Existing Competitors

| Company | Product | Stage | Threat Level |
|---------|---------|-------|--------------|
| **CathWorks** | FFR prediction, PCI planning | FDA-approved, commercial | High |
| **HeartFlow** | CT-FFR (non-invasive) | FDA-approved, public company | Medium (different modality) |
| **OpSens** | FFR guidewire | Hardware + software | Low (hardware focus) |
| **Royal Philips** | Azurion with AI | Integrated into cath labs | High (incumbent) |
| **GE Healthcare** | REVOLUTION AI | Integrated systems | High (incumbent) |
| **Siemens Healthineers** | Corindus robotics + AI | Robotics-focused | Medium |

### Differentiation Strategy

1. **Vendor Neutral:** Works with Philips, GE, Siemens cath labs
2. **Structural Heart Focus:** First AI platform for TAVR/MitraClip
3. **Per-Procedure Pricing:** Aligns costs with volume
4. **Open Platform:** API for research integration
5. **Clinical Validation:** Publish outcomes data, not just algorithms

### Defensibility

| Moat | Strategy |
|------|----------|
| **Data Network Effects** | More angiograms = better models |
| **Integration Complexity** | Deep PACS/EHR integration = switching costs |
| **Regulatory Barrier** | FDA clearance = 12-24 mo moat |
| **Clinical Relationships** | KOL partnerships = trust barrier |
| **Workflow Optimization** | Built into existing cath lab flow |

---

## 12. Go-to-Market Strategy

### Phase 1: Seed (0-12 months)

**Target:** 12 cath labs, $30K MRR

- **Geography:** Focus on academic centers with research interest
- **KOL Strategy:** Partner with 3-5 thought leaders
- **Conferences:** TCT, SCAI, ACC (demo + poster sessions)
- **Pricing:** Pilot discounts, revenue share for research partners

### Phase 2: Growth (12-36 months)

**Target:** 60 cath labs, $165K MRR

- **Geography:** Expand to community hospitals
- **Sales:** Hire 2-3 cath lab experienced sales reps
- **Marketing:** Case studies, published outcomes
- **Partnerships:** GPO (Group Purchasing Organization) contracts

### Phase 3: Scale (36-60 months)

**Target:** 180+ cath labs, $540K+ MRR

- **Geography:** National expansion
- **Enterprise:** Health system contracts (10+ labs)
- **International:** Europe, then Asia-Pacific
- **Ancillary Products:** Fellowship training, research platform

### Sales Motion

1. **Identify Target:** Cath lab directors at high-volume centers
2. **Warm Intro:** KOL referral or conference demo
3. **Pilot:** 30-day free trial, 50+ cases
4. **Validation:** Outcomes report, ROI analysis
5. **Contract:** Annual subscription, implementation
6. **Expansion:** Additional labs, structural heart module

---

## 13. Team Composition

### Founding Team

| Role | Skills | Why Critical |
|------|--------|--------------|
| **CEO/Co-founder** | Healthcare SaaS, cath lab relationships | Sales, partnerships, fundraising |
| **CTO/Co-founder** | ML/CV, medical imaging, DICOM | AI model development, architecture |
| **Clinical Co-founder** | Interventional cardiologist, KOL | Clinical validation, trust, credibility |
| **Regulatory Lead** | FDA 510(k), medical devices | Regulatory strategy, submissions |

### Early Hires (Year 1)

| Role | Priority |
|------|----------|
| **ML Engineer** | Angiogram CV, model training |
| **Full-Stack Developer** | React, DICOM viewers |
| **Clinical Research Manager** | Data partnerships, validation studies |
| **Sales Director** | Cath lab sales experience |

### Advisor Network

- **Interventional Cardiologists** (3-5, diverse geographies)
- **Regulatory Counsel** (FDA device approval experience)
- **Healthcare VC** (Series A introduction)
- **Hospital Administrator** ( procurement, budget cycles)

---

## 14. Funding Strategy

### Pre-Seed: $500K (Already Committed)

**Use of Funds:**
- MVP development (8 weeks)
- Pilot validation (1 cath lab)
- Initial team (founders + 1 engineer)
- Conference presence (TCT, SCAI)

### Seed: $2-3M (Months 3-12)

**Use of Funds:**
- Team expansion (8-12 employees)
- FDA 510(k) initiation
- 10-20 pilot customers
- Clinical validation study

**Target Investors:**
- Healthcare-focused seed funds
- Medtech angels
- Strategic (cath lab vendors)

### Series A: $10-15M (Months 12-24)

**Use of Funds:**
- Commercial team (sales, marketing)
- FDA clearance completion
- 50-100 customers
- Product expansion (structural heart)

**Target Investors:**
- Healthcare growth equity
- Corporate VC (medtech)
- International expansion capital

---

## 15. Success Metrics

### Product Metrics

| Metric | Target (6 months) | Target (18 months) |
|--------|-------------------|-------------------|
| **Angiograms Processed** | 10,000 | 100,000 |
| **Active Cath Labs** | 12 | 60 |
| **Stenosis Accuracy** | <10% error | <5% error |
| **Interpretation Time** | 50% reduction | 70% reduction |
| **User Satisfaction** | 4.0/5.0 | 4.5/5.0 |

### Business Metrics

| Metric | Target (Year 1) | Target (Year 2) |
|--------|-----------------|-----------------|
| **MRR** | $30,000 | $165,000 |
| **ARR** | $360,000 | $1,980,000 |
| **Logo Count** | 12 cath labs | 60 cath labs |
| **NRR (Net Revenue Retention)** | 100% | 110%+ |
| **CAC Payback** | <12 months | <6 months |

### Clinical Metrics

| Metric | Target |
|--------|--------|
| **Stent Malapposition Reduction** | 20% vs. standard care |
| **FFR Utilization Increase** | 2x baseline (non-invasive) |
| **PCI Procedure Time** | 15% reduction |
| **Contrast Volume** | 20% reduction |

---

## 16. Validation Questions

### Critical Hypotheses to Test

1. **Stenosis Accuracy**
   - Question: Can AI estimate stenosis within 10% of QCA?
   - Validation: 100-case pilot, side-by-side comparison

2. **Workflow Integration**
   - Question: Can this fit into existing cath lab workflow without disruption?
   - Validation: Time-motion studies during pilot

3. **Economic Value**
   - Question: Do hospitals see ROI (contrast savings, efficiency)?
   - Validation: Economic analysis post-pilot

4. **Clinical Impact**
   - Question: Does AI improve outcomes (fewer complications)?
   - Validation: Longitudinal outcomes study (6+ months)

5. **Physician Acceptance**
   - Question: Will ICs trust and use AI recommendations?
   - Validation: Usage analytics, satisfaction surveys

### Kill Criteria

| Condition | Action |
|-----------|--------|
| Stenosis error >15% vs. QCA | Pivot or stop |
| <50% of pilots convert to customers | Pivot or stop |
| Physician satisfaction <3.0/5.0 | Pivot or stop |
| FDA pathway unclear/impossible | Stop |
| CAC >$500 | Pivot pricing or stop |

---

## 17. Long-Term Vision

### 5-Year Vision

**CathLabAI becomes the standard AI platform for interventional cardiology:**

- **Market Leader:** 450+ cath labs, $15M+ ARR
- **Product Expansion:**
  - Structural heart (TAVR, MitraClip, tricuspid)
  - Congenital interventions
  - Peripheral vascular interventions
  - Electrophysiology integration
- **Geographic Expansion:**
  - Europe (CE Mark), then Asia-Pacific
  - 30% of revenue international
- **Data Platform:**
  - Largest interventional cardiology dataset
  - Real-world evidence generation
  - Clinical trial acceleration

### Potential Exit Options

| Exit Type | Valuation Range | Timeline |
|-----------|-----------------|----------|
| **Strategic Acquisition** | $200-500M | 5-7 years |
| **IPO** | $500M-1B+ | 7-10 years |
| **Stay Private** | N/A | Indefinitely (bootstrapped profitability) |

### Likely Acquirers

- **Philips Healthcare** (cath lab systems)
- **GE Healthcare** (cardiology imaging)
- **Siemens Healthineers** (angiography)
- **Boston Scientific** (interventional devices)
- **Abbott** (cardiovascular devices)
- **Medtronic** (structural heart)

---

## 18. Decision Framework

### Go/No-Go Criteria: GO

| Factor | Assessment | Weight |
|--------|------------|--------|
| **Market Size** | 15,000 ICs, $20B procedures | 9/10 |
| **AI Fit** | Computer vision = native use case | 10/10 |
| **Clinical Need** | Stent sizing errors = real harm | 9/10 |
| **Revenue Potential** | $90K LTV, 450:1 LTV:CAC | 8/10 |
| **Competitive** | Incumbents + startups, but differentiated | 6/10 |
| **Regulatory** | FDA required, but clear path | 7/10 |
| **Team Feasibility** | Need clinical co-founder critical | 8/10 |

**Overall Score: 8.00/10**

### Critical Success Factors

1. **Hire interventional cardiologists** as co-founders/advisors (credibility)
2. **Partner with one cath lab** for data access and validation
3. **Start with stenosis estimation** (clear ROI, measurable)
4. **Differentiate vs. incumbents** (structural heart focus, vendor-neutral)
5. **Build TCT/SCAI relationships** early for distribution

---

## 19. Next Steps

### Immediate Actions (Week 1)

- [ ] Identify and reach out to 10 potential cath lab partners
- [ ] Draft data use agreement template
- [ ] Research FDA 510(k) predicate devices
- [ ] Scout clinical co-founder candidates
- [ ] Set up development environment and annotation pipeline

### Short-Term Actions (Month 1)

- [ ] Secure first data partnership
- [ ] Collect initial 500 angiograms
- [ ] Train first segmentation model
- [ ] Design validation study protocol
- [ ] Incorporate entity, setup legal

### Medium-Term Actions (Months 2-3)

- [ ] Complete MVP development
- [ ] Deploy pilot to partner cath lab
- [ ] Begin 510(k) preparation
- [ ] Present at TCT conference
- [ ] Raise seed round

---

## 20. Appendix

### Key References

1. **SCAI (Society for Cardiovascular Angiography and Interventions)** - https://scai.org
2. **TCT (Transcatheter Cardiovascular Therapeutics)** - https://www.crfdigitalevents.com/tct
3. **ACC.22 Interventional Cardiology Section** - https://www.acc.org
4. **FDA 510(k) Guidance for Cardiac Catheterization Devices**

### Clinical Papers

- "Computer-Assisted Coronary Intervention" - JACC: Cardiovascular Interventions
- "Deep Learning for Stenosis Quantification" - Circulation: AI
- "Non-invasive FFR from Coronary CTA" - HeartFlow validation studies

### Competitor Research

- **CathWorks:** https://www.cathworks.com
- **HeartFlow:** https://www.heartflow.com
- **Philips Azurion:** https://www.usa.philips.com/healthcare

---

**Venture Status:** PURSUE

**Last Updated:** 2026-03-02

**Decision:** Large market opportunity in high-volume cardiac procedures. AI-native use case with strong clinical and economic value. Proceed with MVP development and cath lab partnership.
