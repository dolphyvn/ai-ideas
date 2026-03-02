# MammoAI - Breast Cancer Screening & Detection Platform

## Executive Summary

MammoAI is an AI-powered platform designed specifically for breast imaging radiologists that automates mammogram interpretation, calcification detection, mass detection, breast density assessment, and BI-RADS scoring. Breast cancer is the second most common cancer in women with over 300,000 new cases annually in the US, and 40+ million mammograms are performed each year. The platform targets breast imaging specialists with a suite of AI tools that improve detection accuracy, reduce interpretation time, and provide consistency in BI-RADS scoring.

**Go/No-Go Decision: GO (Score: 8.50/10)**

---

## 1. Core Concept

AI-powered platform for breast imaging radiologists that automates:

- **Calcification Detection:** Automated identification of microcalcifications (early sign of DCIS)
- **Mass Detection:** Tumor and mass identification with malignancy probability
- **Breast Density Assessment:** Automated BI-RADS density categorization (a, b, c, d)
- **BI-RADS Scoring:** Standardized assessment category recommendation
- **Prior Exam Comparison:** Temporal analysis for change detection
- **Workflow Integration:** PACS integration for seamless radiologist workflow

---

## 2. Problem Statement

### Market Scale
- **15,000+** radiologists specializing in breast imaging in the US
- **40M+** mammograms performed annually in the United States
- **300K+** new breast cancer cases per year (2nd leading cancer in women)
- **50K+** breast cancer deaths annually

### Core Pain Points

#### For Radiologists
- **Calcification detection is extremely time-consuming:** Microcalcifications are tiny (0.1-1mm) and easy to miss, requiring painstaking zoom inspection
- **Breast density masks cancer:** Dense breast tissue (BI-RADS c/d) obscures ~50% of cancers in mammography
- **High cognitive load:** Hours of screening with constant attention to detail
- **Prior exam comparison:** Manual comparison with prior studies is tedious but critical

#### For Breast Centers
- **Breast imaging specialist shortage:** Fewer radiologists specializing in breast imaging
- **Turnaround time pressure:** Patients expect quick results (anxiety reduction)
- **Quality assurance:** MQSA requires rigorous quality standards
- **Malpractice risk:** Missed diagnosis = litigation (breast cancer = high-stakes malpractice)

#### For Patients
- **Dense breast notification laws:** 38 states require density notification (patient anxiety)
- **Recall anxiety:** False positives cause unnecessary recall and biopsy
- **Early detection matters:** Stage 0 detection = 98% survival vs Stage IV = 27%

---

## 3. Target Vertical

### Primary Customer: Breast Imaging Radiologists

**Segment 1: Breast Imaging Specialists (High Priority)**
- Fellowship-trained breast radiologists
- Dedicated breast imaging practice
- High-volume mammography readers (100+ studies/day)
- **Pain:** Maximizing throughput without missing cancers

**Segment 2: General Radiologists (Medium Priority)**
- General diagnostic radiologists who read mammograms
- Rural/underserved areas without breast specialists
- **Pain:** Lack of specialized training, higher miss rates

**Segment 3: Breast Center Directors (Decision Makers)**
- Medical directors of breast centers
- Chiefs of breast imaging
- **Pain:** Quality metrics, throughput, liability management

### Secondary Customer: Breast Centers & Hospitals

- Hospital breast imaging departments
- Freestanding breast centers
- Women's imaging centers
- Academic breast imaging programs

---

## 4. Why Now

### Market Timing Factors

#### 1. Universal Screening Demand
- Breast cancer screening is universally recommended for women 40-75
- USPSTF guidelines: biennial screening for women 50-74
- American College of Radiology: annual screening starting at 40
- **Result:** 40M+ annual mammograms = massive, stable market

#### 2. Regulatory Landscape
- **MQSA (Mammography Quality Standards Act):** Federal accreditation requirements
- **Breast Density Notification Laws:** 38 states mandate density disclosure
- **FDA oversight:** Breast imaging AI = Class II/III medical device (regulatory moat)
- **Result:** Regulatory moat protects validated solutions

#### 3. Technology Maturity
- **Calcification detection CNN:** Proven capability for microcalcification identification
- **Breast density ML:** Automated density assessment is mature
- **2D/3D mammography AI:** Tomosynthesis (3D) analysis is advancing
- **GPU compute:** Affordable inference for mammography models
- **Result:** AI technology is ready for clinical deployment

#### 4. Specialist Shortage
- Breast imaging fellowship positions are limited
- Aging radiologist workforce
- Breast burnout from high-volume screening
- **Result:** Demand for efficiency tools

#### 5. Malpractice Pressure
- Breast cancer = highest malpractice payouts in radiology
- Missed diagnosis = $1M+ settlements
- **Result:** Radiologists need AI "second reader" for liability protection

---

## 5. AI Advantage

### Core AI Capabilities

#### 1. Calcification Detection CNN
- **Input:** Full-field digital mammography (FFDM) or tomosynthesis
- **Output:** Microcalcification cluster localization + malignancy probability
- **Architecture:** ResNet-50/DenseNet backbone with feature pyramid
- **Training:** Labeled microcalcification datasets (CBIS-DDSM, VinDr-Mammo)
- **Advantage:** Human eye fatigue = missed microcalcifications; AI never fatigues

#### 2. Mass Detection & Classification
- **Input:** Mammogram images (2D or 3D)
- **Output:** Mass localization + shape/margin analysis + BI-RADS features
- **Architecture:** Mask R-CNN for segmentation + classifier
- **Features:** Spiculation, circumscription, calcification within mass
- **Advantage:** Quantitative morphology features

#### 3. Breast Density Assessment
- **Input:** Bilateral mammogram views (CC, MLO)
- **Output:** BI-RADS density category (a, b, c, d) + percent density
- **Architecture:** CNN regression model trained on density-labeled datasets
- **Advantage:** Eliminates inter-rater variability in density assessment

#### 4. BI-RADS Scoring Automation
- **Input:** All detected features + density + comparison with priors
- **Output:** Recommended BI-RADS category (0-6) with confidence
- **Architecture:** Multi-modal fusion of detection outputs
- **Advantage:** Consistency in assessment categories

#### 5. Prior Exam Temporal Comparison
- **Input:** Current exam + prior exams (1+ years ago)
- **Output:** Change detection (new, stable, regressing)
- **Architecture:** Siamese networks for temporal analysis
- **Advantage:** Detects subtle changes over time (early cancer sign)

### Data Requirements
- **Training Data:** 50,000+ annotated mammograms (calcification, mass, density)
- **Validation Data:** 10,000+ independent test set
- **Sources:** Public datasets (CBIS-DDSM, VinDr-Mammo) + partner breast center data

---

## 6. Viral Mechanism

### Professional Network Virality

#### 1. Society of Breast Imaging (SBI) Conferences
- Annual SBI meeting (1,500+ breast imaging specialists)
- "This AI detected DCIS I missed" = VIRAL storytelling
- Case study presentations: AI-detected microcalcifications = curative DCIS
- **Result:** Peer-to-peer referral within tight specialist community

#### 2. RSNA Radiological Society of North America
- Annual RSNA meeting (50K+ radiologists)
- Breast imaging scientific sessions
- AI showcase demonstrations
- **Result:** Exposure to general radiologists who read mammograms

#### 3. Breast Center Referral Networks
- Breast center directors share best practices
- "How do you handle density assessment?" = "We use MammoAI"
- Quality improvement collaboratives
- **Result:** Multi-center adoption within health systems

### Case Study Virality
- **"Early detection = breast-conserving surgery"** (mastectomy avoided)
- **"AI-detected calcifications = DCIS cure"** (life-saving detection)
- **"50% reduction in interpretation time"** (efficiency story)
- **"Zero missed cancers in 10K pilot"** (quality story)

### Academic Publication Strategy
- SBI/ACR journal publications (validation studies)
- RSNA Radiology journal (impact factor ~12)
- **Result:** Clinical validation = adoption trigger

---

## 7. Revenue Model

### Per-Breast Center Subscription

#### Tier 1: Starter ($2,000/month)
- Calcification detection AI
- Breast density assessment (BI-RADS categories)
- Basic reporting integration
- Email support
- **Target:** Small breast centers, solo practices

#### Tier 2: Professional ($3,000/month)
- All Starter features
- Mass detection + classification
- BI-RADS scoring recommendation
- Prior exam comparison (temporal analysis)
- PACS integration (standard)
- Priority support
- **Target:** Medium-sized breast centers, hospital departments

#### Tier 3: Enterprise ($6,000/month)
- All Professional features
- Multi-center deployment (unlimited sites)
- Advanced analytics dashboard
- Research/quality improvement tools
- API access for custom workflows
- Dedicated account manager
- On-site training
- **Target:** Large health systems, academic centers, multi-state breast center networks

### Per-Mammogram Add-On
- **Price:** $5 per AI-analyzed mammogram (beyond included tiers)
- **Usage:** High-volume centers exceeding monthly quotas
- **Tier allocations:**
  - Starter: 500 mammograms/month included
  - Professional: 2,000 mammograms/month included
  - Enterprise: 5,000 mammograms/month included

### Unit Economics

#### Customer Acquisition Cost (CAC)
- **SBI/RSNA conference presence:** $20K/year ÷ 100 leads = $200/lead
- **Conversion rate:** 20% = $1,000 CAC per customer
- **Breast center direct sales:** Site visits + demos = $400 CAC
- **Weighted average CAC:** $400

#### Customer Lifetime Value (LTV)
- **Average contract value:** $3,000/month (Professional tier)
- **Retention:** 36 months (switching costs very high - workflow integration)
- **Expansion:** 30% upsell to Enterprise over lifetime
- **LTV:** $3,000 × 36 × 1.3 = $140,400
- **Conservative LTV:** $108,000 (no upsell)

#### LTV:CAC Ratio
- **Ratio:** $108,000 ÷ $400 = **270:1** (exceptional)

#### Gross Margin
- **Infrastructure costs:** 10% (AWS GPU inference, storage)
- **Support costs:** 5% (account management, technical support)
- **Gross margin:** **85%**

### Monthly Revenue Potential

#### Year 1: Launch Phase
- **Target:** 12 breast centers
- **Mix:** 8 Starter ($2K) + 3 Professional ($3K) + 1 Enterprise ($6K)
- **MRR:** (8 × $2K) + (3 × $3K) + (1 × $6K) = $16K + $9K + $6K = **$31K MRR**
- **ARR:** **$372K**

#### Year 2: Growth Phase
- **Target:** 60 breast centers
- **Mix:** 20 Starter + 30 Professional + 10 Enterprise
- **MRR:** (20 × $2K) + (30 × $3K) + (10 × $6K) = $40K + $90K + $60K = **$190K MRR**
- **ARR:** **$2.28M**

#### Year 3: Scale Phase
- **Target:** 180 breast centers
- **Mix:** 40 Starter + 100 Professional + 40 Enterprise
- **MRR:** (40 × $2K) + (100 × $3K) + (40 × $6K) = $80K + $300K + $240K = **$620K MRR**
- **ARR:** **$7.44M**

---

## 8. MVP in 8 Weeks

### Weeks 1-2: Data Collection & Partnership
**Goal:** Secure mammogram dataset + one breast center partnership

**Activities:**
- Identify and outreach to 20 breast centers
- Negotiate data sharing agreement (de-identified mammograms)
- Collect 5,000+ mammograms with calcification/mass annotations
- Set up secure, HIPAA-compliant data storage
- IRB approval for retrospective data analysis

**Deliverables:**
- One breast center partnership agreement
- 5,000+ annotated mammogram dataset
- Data pipeline for image ingestion

### Weeks 3-5: Calcification Detection CNN
**Goal:** Build and validate calcification detection model

**Activities:**
- Train CNN on CBIS-DDSM + partner data
- Implement microcalcification detection (0.1-1mm clusters)
- Validate on held-out test set
- Compare to radiologist ground truth

**Technical Approach:**
- Backbone: ResNet-50 pre-trained on ImageNet
- Detection: Feature Pyramid Network (FPN) for small objects
- Training: Transfer learning from mammography datasets
- Inference optimization: TensorRT for GPU acceleration

**Deliverables:**
- Calcification detection CNN model
- Validation report: sensitivity, specificity, AUC
- REST API for model inference

### Weeks 6-7: Breast Center Pilot
**Goal:** Validate detection accuracy + time savings in clinical setting

**Activities:**
- Deploy model to breast center PACS integration
- Radiologists use AI for calcification detection (parallel read)
- Collect metrics: detection accuracy, interpretation time, user satisfaction
- Iterate based on feedback

**Validation Metrics:**
- **>90% sensitivity** for calcification detection (vs radiologist)
- **>85% specificity** (avoid false recalls)
- **50%+ reduction** in interpretation time
- **Net Promoter Score >50** from radiologists

**Deliverables:**
- Pilot deployment at one breast center
- Validation report with clinical metrics
- User feedback + iteration plan

### Week 8: Refinement & Demo Prep
**Goal:** Finalize model + prepare for SBI conference demo

**Activities:**
- Refine model based on pilot feedback
- Optimize inference speed (<3 seconds per mammogram)
- Build interactive demo for SBI conference
- Prepare case studies: "AI-detected DCIS"

**Deliverables:**
- Production-ready calcification detection model
- SBI conference demo
- Case study deck for customer presentations

### MVP Go/No-Go Criteria
- [ ] >90% sensitivity for calcification detection
- [ ] >85% specificity (avoid false recalls)
- [ ] 50%+ reduction in interpretation time
- [ ] One breast center commits to paid pilot after MVP
- [ ] HIPAA compliance validated

---

## 9. Tech Stack

### Backend & API
- **Language:** Python 3.11+
- **Framework:** FastAPI (async,高性能)
- **Authentication:** OAuth2 + JWT
- **Database:** PostgreSQL (customer data) + Redis (caching)

### AI/Machine Learning
- **Framework:** PyTorch 2.0+
- **Medical Imaging:** MONAI (Medical Open Network for AI)
- **Pre-trained Models:** MedicalNet for transfer learning
- **Inference Optimization:** ONNX Runtime, TensorRT
- **Training:** AWS SageMaker (GPU instances)

### Computer Vision
- **Image Processing:** OpenCV, scikit-image
- **Visualization:** matplotlib, Plotly (for heatmaps)
- **DICOM Handling:** pydicom, HighDICOM

### Integrations
- **PACS:** DICOM protocol (DIMSE), DICOMweb
- **Mammography Systems:** Hologic, GE Healthcare, Siemens
- **EHR:** HL7 FHIR API for patient data
- **Reporting:** Integration with RadReport, PowerScribe

### Infrastructure
- **Cloud:** AWS (US regions)
- **Compute:** EC2 G5 instances (GPU inference)
- **Storage:** S3 (mammogram storage, encrypted)
- **Compliance:** HIPAA BAA, SOC 2 Type II
- **Monitoring:** Datadog, Sentry

### Security
- **Encryption:** AES-256 at rest, TLS 1.3 in transit
- **Access Control:** Role-based access control (RBAC)
- **Audit Logging:** All access logged
- **De-identification:** DICOM anonymization (patient privacy)

---

## 10. Risk Factors

### 1. FDA Regulatory Pathway (HIGH RISK)
- **Risk:** Breast imaging AI = FDA Class II or III medical device
- **Impact:** 510(k) clearance or de novo approval = 12-24 months, $1-5M
- **Mitigation:**
  - Start with "Software as Medical Device" (SaMD) pathway
  - Use FDA-cleared components where possible
  - Partner with regulatory consultant from day 1
  - Target 510(k) with predicate device (e.g., iCAD's cleared AI)
  - Publish clinical validation studies

### 2. Mammogram Data Quality (MEDIUM RISK)
- **Risk:** Variability in compression, positioning, artifacts
- **Impact:** Poor data = model fails to generalize
- **Mitigation:**
  - Strict data quality criteria during collection
  - Data augmentation (rotation, noise, artifacts)
  - Multi-center data (diverse equipment, protocols)
  - Active learning for edge cases

### 3. High Liability (HIGH RISK)
- **Risk:** AI misses breast cancer = malpractice exposure
- **Impact:** Company liability + reputation damage
- **Mitigation:**
  - AI positioned as "decision support" not diagnostic
  - Radiologist always makes final diagnosis
  - Comprehensive validation studies
  - Malpractice insurance coverage
  - Clear product disclaimers

### 4. Competition (MEDIUM RISK)
- **Risk:** Established mammography AI vendors (iCAD, Kheiron, Hologic)
- **Impact:** Market share battle
- **Mitigation:**
  - Focus on breast-specific suite (not just detection)
  - Prior exam comparison (unique feature)
  - Workflow integration advantage
  - SBI conference presence (specialist relationships)

### 5. Clinical Workflow Integration (MEDIUM RISK)
- **Risk:** PACS integration complexity, radiologist workflow disruption
- **Impact:** Poor adoption if workflow is disrupted
- **Mitigation:**
  - Seamless PACS integration (DICOM standard)
  - Radiologist co-designers
  - "No-click" integration (AI auto-runs)
  - Pilot testing before full rollout

### 6. Reimbursement (LOW-MEDIUM RISK)
- **Risk:** No CPT code for AI-assisted mammography
- **Impact:** Centers must pay out of pocket
- **Mitigation:**
  - Position as efficiency tool (time savings justify cost)
  - Advocacy for AI CPT codes (long-term)
  - ROI calculator for breast centers

---

## 11. Competitive Landscape

### Direct Competitors

#### iCAD (Public Company)
- **Product:** ProFound AI for 2D/3D mammography
- **Focus:** Detection + case prioritization
- **Strength:** FDA-cleared, established customer base
- **Weakness:** Limited density assessment, no prior comparison
- **Market Cap:** ~$100M

#### Kheiron Medical (Startup)
- **Product:** Mia (mammography AI)
- **Focus:** Breast cancer detection
- **Strength:** CE marked, UK-based validation
- **Weakness:** Limited US presence, early-stage
- **Funding:** ~$20M

#### Hologic (Equipment Vendor)
- **Product:** AI integrated into 3D mammography systems
- **Focus:** Detection + workflow
- **Strength:** Installed base advantage
- **Weakness:** Hardware lock-in, limited breast-specific features

#### GE Healthcare
- **Product:** mammography AI on GE systems
- **Focus:** Quality + detection
- **Strength:** GE equipment integration
- **Weakness:** Hardware-focused, not platform-agnostic

#### Hospital-Built AI
- **Products:** Academic centers building custom AI
- **Focus:** Research + clinical validation
- **Strength:** Strong clinical validation
- **Weakness:** Not commercialized, limited availability

### MammoAI Differentiation

| Feature | MammoAI | iCAD | Kheiron | Hologic | GE |
|---------|---------|------|---------|---------|-----|
| Calcification Detection | YES | YES | YES | YES | YES |
| Mass Detection | YES | YES | YES | YES | YES |
| Breast Density Assessment | YES | Limited | NO | Limited | Limited |
| BI-RADS Scoring | YES | Limited | NO | NO | NO |
| Prior Exam Comparison | YES | NO | NO | Limited | NO |
| PACS-Agnostic | YES | YES | YES | NO (Hologic) | NO (GE) |
| Breast-Specific Suite | YES | NO | NO | NO | NO |

**Competitive Advantage:** Only platform combining calcification detection + density assessment + BI-RADS + prior exam comparison in one breast-specific suite. Platform-agnostic (works with any PACS/mammography system).

---

## 12. Go/No-Go Decision: GO

### Score: 8.50/10 - PURSUE

#### Strengths (Why GO)
1. **High-Stakes Problem:** 2nd leading cancer (300K+ cases) = massive impact
2. **Massive Market:** 40M+ mammograms annually = 15K+ radiologist customers
3. **Proven AI:** Calcification detection CNN = mature technology
4. **Strong Monetization:** $3K/month × 180 centers = $7.44M ARR potential
5. **Regulatory Moat:** FDA + MQSA = credential barrier to entry
6. **High Switching Costs:** Workflow integration = 36-month retention
7. **Viral Mechanism:** "This AI detected DCIS I missed" = powerful storytelling
8. **Density Laws:** 38 states mandate notification = mandatory feature

#### Weaknesses (Risks to Manage)
1. **FDA Pathway:** Class II/III clearance = 12-24 months, $1-5M
2. **Competition:** iCAD, Kheiron, Hologic already in market
3. **Specialist Shortage:** Fewer breast imaging specialists
4. **High Liability:** Missed cancer = malpractice exposure
5. **Data Dependence:** Need breast center partnership for training data

### Critical Success Factors

#### MUST Have (Non-Negotiable)
1. **Breast Imaging Radiologist Co-Founder/Advisor:** Clinical credibility is essential
2. **Breast Center Data Partnership:** Cannot build without real mammograms
3. **FDA Strategy from Day 1:** Regulatory pathway drives product design
4. **Calcification Detection First:** Early sign of DCIS = highest clinical value
5. **Density Assessment:** Mandatory in 38 states = compliance sell

#### SHOULD Have (Important)
1. **SBI/RSNA Presence:** Conference relationships drive adoption
2. **Prior Exam Comparison:** Unique vs competition
3. **PACS-Agnostic Platform:** Works with any system
4. **Malpractice Insurance:** Risk mitigation
5. **Clinical Validation Studies:** Publication strategy

#### NICE to Have (Advantageous)
1. **Multi-Center Pilot:** Validation across diverse settings
2. **EHR Integration:** Seamless workflow
3. **Research Tools:** Academic breast center appeal
4. **API Access:** Custom workflow enablement
5. **International Expansion:** CE mark for Europe

### Final Recommendation: GO

**Reasoning:**

1. **Credential + Regulatory Pattern:** Breast imaging + MQSA + FDA = defensible moat. The regulatory barrier protects against low-effort competition.

2. **High-Volume Screening:** 40M+ annual mammograms = stable, recurring demand. Screening is universal for women 40-75.

3. **Calcification Detection = Proven AI:** Microcalcification detection CNN is technically feasible with public datasets (CBIS-DDSM, VinDr-Mammo).

4. **Strong Monetization:** $3K/month pricing × 36-month retention = $108K LTV per customer with 85% gross margins.

5. **Viral Potential:** "AI-detected DCIS" storytelling creates powerful peer-to-peer virality within the tight breast imaging community.

6. **Density Laws = Tailwind:** 38 states mandate breast density notification = compliance-driven feature adoption.

**High-volume screening + calcification detection + regulatory moat = breast cancer impact.**

---

## 13. Next Steps

### Immediate Actions (Week 1)
1. **Recruit Breast Imaging Radiologist Co-Founder/Advisor**
   - Target: SBI member, academic breast center
   - Equity stake + clinical leadership role

2. **Secure Breast Center Data Partnership**
   - Outreach to 20 breast centers
   - Pitch: Research collaboration, early access to AI
   - Deliverable: 5,000+ annotated mammograms

3. **Engage FDA Regulatory Consultant**
   - Classify device: Class II vs III
   - Identify predicate device for 510(k)
   - Design validation study

### MVP Build (Weeks 2-8)
4. **Build Calcification Detection CNN**
   - Train on CBIS-DDSM + partner data
   - Target: >90% sensitivity, >85% specificity

5. **Deploy Breast Center Pilot**
   - One breast center pilot
   - Validate: accuracy + time savings + NPS

### Go-to-Market (Post-MVP)
6. **SBI Conference Launch**
   - Demo calcification detection
   - Present case studies: "AI-detected DCIS"
   - Collect 50+ qualified leads

7. **FDA 510(k) Submission**
   - Submit with predicate device
   - Target 12-month clearance timeline

8. **Scale to 12 Centers**
   - 5 Starter + 5 Professional + 2 Enterprise
   - $31K MRR = $372K ARR

---

## Appendix A: Market Sizing

### TAM (Total Addressable Market)
- **US Breast Centers:** ~2,500 facilities
- **US Mammograms:** 40M annually
- **Market Value:** $3B+ (assuming $75/mammogram for screening)

### SAM (Serviceable Addressable Market)
- **Breast Centers with Digital Mammography:** ~2,000
- **Adoptable for AI (modern PACS):** ~1,500
- **Target Market Value:** $1.8B+

### SOM (Serviceable Obtainable Market)
- **3-Year Target:** 180 breast centers (12% of adoptable market)
- **3-Year Revenue:** $7.44M ARR
- **Market Share:** <1% of total market

## Appendix B: Regulatory Pathway

### FDA Classification
- **Likely Class II:** Mammography CAD (Computer-Aided Detection)
- **Predicate Device:** iCAD ProFound AI (510(k) cleared)
- **Pathway:** 510(k) substantial equivalence

### 510(k) Requirements
1. **Predicate Device:** Identify cleared mammography AI
2. **Substantial Equivalence:** Demonstrate safety/effectiveness
3. **Clinical Validation:** Reader study + retrospective validation
4. **Software Documentation:** Architecture, testing, risk analysis
5. **Manufacturing:** QSR (Quality System Regulation)

### Timeline
- **Preparation:** 3 months (documentation, validation study)
- **Submission:** 1 month
- **FDA Review:** 8-12 months
- **Total:** 12-16 months

### Cost
- **Regulatory Consultant:** $200K
- **Clinical Validation Study:** $500K
- **Documentation & Testing:** $300K
- **Total:** ~$1M

## Appendix C: Clinical Validation Design

### Reader Study Design
- **Participants:** 10 breast imaging radiologists
- **Cases:** 200 mammograms (100 cancer, 100 normal)
- **Conditions:** Unassisted vs AI-assisted
- **Metrics:** Sensitivity, specificity, AUC, reading time

### Retrospective Validation
- **Dataset:** 10,000 mammograms with pathology correlation
- **Comparison:** AI vs radiologist ground truth
- **Subgroup Analysis:** Density categories, cancer types

### Endpoints
- **Primary:** Non-inferior sensitivity vs radiologist
- **Secondary:** Reduction in interpretation time
- **Safety:** No increase in false positives

## Appendix D: Key Datasets

### Public Datasets
1. **CBIS-DDSM:** Curated Breast Imaging Subset of DDSM (2,620 scans)
2. **VinDr-Mammo:** 5,000 mammograms with annotations
3. **MIAS:** Mammographic Image Analysis Society (322 scans)
4. **BCDR:** Breast Cancer Digital Repository (1,500+ cases)

### Private Data (Partnership)
- **Target:** 5,000+ annotated mammograms from breast center
- **Annotations:** Calcification, mass, density, pathology
- **De-identified:** HIPAA compliant

---

**Document Version:** 1.0
**Created:** March 2, 2026
**Last Updated:** March 2, 2026
**Status:** GO - Pursue
