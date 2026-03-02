# CTTriageAI - Emergency CT Triage Platform
## Venture Specification

**Date:** 2026-03-02
**Category:** Healthcare AI / Medical Imaging
**Decision:** GO - 8.67/10

---

## Executive Summary

CTTriageAI is an AI-powered platform for radiologists that automates CT scan triage in emergency departments. By prioritizing critical findings first (pulmonary embolism, stroke, pneumonia, fractures), the platform reduces time-to-diagnosis for life-threatening conditions from hours to minutes.

**The Opportunity:** 100M+ CT exams annually in the US, with emergency cases representing the highest-stakes segment where minutes literally save lives.

**The Solution:** 3D CNN-based computer vision that detects critical findings, triages studies by urgency, and generates automated preliminary reports for emergency department radiologists.

---

## 1. Core Concept

AI-powered platform for radiologists that automates CT scan triage (prioritizing critical findings first), pulmonary embolism detection, pneumonia detection, fracture detection, and automated reporting for emergency department cases.

**Key Capabilities:**
- **Triage prioritization:** Queue reordering based on detected urgency
- **Critical finding detection:** PE, stroke, intracranial hemorrhage, fractures, pneumonia
- **Automated reporting:** Preliminary reports with measurements and findings
- **Incidental finding tracking:** Follow-up reminders for non-emergency findings

---

## 2. Problem Statement

### Market Pain Points

| Problem | Impact | Stakeholder |
|---------|--------|-------------|
| CT scan backlog | Delayed diagnoses, patient harm | Radiologists, Patients |
| FIFO queue processing | Critical studies wait behind routine | ED Physicians |
| Radiologist burnout | 35% reporting burnout | Radiologists |
| Incidental findings lost | Missed cancer diagnoses | Patients, Hospitals |
| Night/weekend coverage | Teleradiology latency | EDs, Patients |

### By The Numbers

- **35,000+** radiologists in the United States
- **100M+** CT examinations performed annually in the US
- **CT** = highest volume imaging modality (higher than MRI, ultrasound)
- **Emergency CT** = life-threatening findings (PE, stroke, trauma)
- **Time to diagnosis** = minutes matter for mortality outcomes
- **Pulmonary Embolism** = 100,000+ deaths annually when missed
- **Teleradiology** = growing due to radiologist shortages and 24/7 demand

### The "FIFO" Problem

Most PACS (Picture Archiving and Communication System) queues process studies in first-in, first-out order. A routine abdominal CT processed before a critical PE scan could delay life-saving treatment by 30+ minutes.

---

## 3. Target Vertical

### Primary Customer: Radiologists in Emergency Departments

**Emergency Radiologists**
- High-volume ED hospitals
- Academic medical centers
- Level I/II trauma centers
- Comprehensive stroke centers

**Teleradiologists**
- Night/weekend coverage services
- Outsourced ED reads
- Rural hospital coverage
- Subspecialty emergency reads

**Radiology Groups**
- Groups covering multiple EDs
- Hospital-based radiology practices
- Teleradiology firms

### Secondary Customers

**Emergency Physicians**
- Need faster radiology turnaround
- Benefit from triage notifications
- Make treatment decisions faster

**Hospital Administrators**
- Quality metrics (stroke/sepsis time-to-treatment)
- Length-of-stay reduction
- Malpractice risk reduction
- Radiologist recruitment/retention

---

## 4. Why Now

### Market Timing Factors

| Factor | Trend | Impact |
|--------|-------|--------|
| **CT Volume Growth** | Aging population, obesity, cancer screening | Increasing demand |
| **ED Overcrowding** | Boarding times, patient surge | Time pressure |
| **Teleradiology Growth** | Remote work, global coverage | Platform need |
| **AI Validation** | FDA approvals, clinical studies | Credibility |
| **Quality Metrics** | CMS metrics, reimbursement tied to outcomes | Hospital urgency |
| **Radiologist Shortage** | Burnout, retiring workforce | Automation need |

### Technology Readiness

1. **3D CNNs** proven for CT analysis (Nature Medicine papers, 2019-2025)
2. **MONAI framework** mature (Medical Open Network for AI)
3. **GPU infrastructure** accessible via cloud (AWS HIPAA regions)
4. **FDA pathways** clearer for AI/ML SaMD (Software as Medical Device)
5. **Hospital IT** more accepting of cloud integrations (post-COVID)

### Clinical Validation

- Aidoc (competitor) cleared by FDA for multiple findings
- Multiple published studies showing AI triage efficacy
- RSNA/AAPM AI initiatives building acceptance

---

## 5. AI Advantage

### Why AI Is The Right Solution

CT scans are **ideal for AI:**
1. **Structured 3D data** (unlike 2D X-ray)
2. **High contrast** (tissue differentiation)
3. **Standardized protocols** (consistent acquisition)
4. **Binary findings** (PE present/absent, fracture yes/no)
5. **Quantitative** (measurements, densities)

### Technical Approach

**3D Convolutional Neural Networks (CNNs)**
- Process CT volumes as 3D tensors
- Detect findings across contiguous slices
- Learn spatial relationships (vessel, organ anatomy)

**Key Architectures:**
- 3D ResNet / DenseNet variants
- Vision Transformers (ViT) for CT
- Multi-task learning (simultaneous finding detection)
- Attention mechanisms (localize findings)

**MONAI Framework**
- Medical imaging optimized
- DICOM native support
- 3D data pipelines
- Pre-trained models for transfer learning

### AI Capabilities

| Capability | AI Method | Clinical Value |
|------------|-----------|----------------|
| **PE Detection** | 3D CNN on pulmonary arteries | Life-saving triage |
| **Pneumonia Detection** | Segmentation + classification | Sepsis prevention |
| **Fracture Detection** | Bone segmentation + anomaly | Trauma prioritization |
| **Stroke Detection** | Intracranial hemorrhage detection | Thrombolytic window |
| **Triage Scoring** | Multi-finding urgency ML | Queue optimization |
| **Automated Measurements** | Segmentation + volumetrics | Report generation |

---

## 6. Viral Mechanism

### Organic Growth Channels

**Professional Conferences**
- RSNA (Radiological Society of North America) - 50K+ attendees
- ARRS (American Roentgen Ray Society)
- ACR (American College of Radiology) meetings
- ASER (American Society of Emergency Radiology)

**Case Study Virality**
- "This AI caught a PE I missed" = life-saving story
- Before/after time-to-diagnosis metrics
- Hospital-to-hospital referrals within networks

**Peer-to-Peer**
- Radiologist-to-radiologist referrals
- Teleradiology firm adoption
- Hospital system rollouts

### Thought Leadership

- Publication in radiology journals (Radiology, AJR)
- RSNA AI Showcase presentations
- Podcast appearances (Radiology podcasts, healthcare AI)
- Social proof from early adopters

---

## 7. Revenue Model

### Pricing Tiers

| Tier | Price | Features | Target |
|------|-------|----------|--------|
| **Starter** | $2,000/month | One finding (PE) + triage | Small EDs, rural hospitals |
| **Professional** | $2,500/month | Multiple findings + reporting + incidental tracking | Medium EDs, radiology groups |
| **Enterprise** | $5,000/month | Multi-hospital + white-label + API + EHR integration | Health systems, teleradiology |

### Additional Revenue Streams

**Per-Scan Add-on**
- $1 per AI-analyzed CT beyond included tiers
- Volume discounts for high-volume sites

**Implementation Fees**
- One-time $5,000 for PACS/EHR integration
- Custom workflow configuration

**Training & Support**
- Annual support contract: 20% of license
- On-site training: $2,000/day

### Unit Economics

| Metric | Value | Notes |
|--------|-------|-------|
| **CAC** | $400 | RSNA/ARRS conference booths, webinars |
| **LTV** | $90,000 | 36-month avg retention, high switching costs |
| **LTV:CAC** | 225:1 | Excellent |
| **Gross Margin** | 82% | Cloud compute, FDA compliance costs |
| **Sales Cycle** | 6-12 months | Hospital procurement timeline |
| **Churn** | <5% annually | High switching costs, workflow integration |

### Revenue Assumptions

- **Year 1:** 12 hospitals × $2,500 ARPU = $30K MRR = $360K ARR
- **Year 2:** 60 hospitals + enterprise accounts = $150K MRR = $1.8M ARR
- **Year 3:** 180 hospitals + health system contracts = $450K MRR = $5.4M ARR

---

## 8. MVP in 8 Weeks

### Development Timeline

**Weeks 1-2: Data Collection & Setup**
- Source PE (pulmonary embolism) CT datasets
- Establish data pipeline (DICOM → training format)
- Set up MONAI/PyTorch environment
- IRB/Data use agreements

**Deliverables:** 500+ annotated PE CT studies

**Weeks 3-5: PE Detection Model**
- Train 3D CNN for PE detection
- Target: >0.90 sensitivity (cannot miss PE)
- Target: >0.85 specificity (avoid false alarms)
- Validation on held-out test set

**Deliverables:** Trained model with performance benchmarks

**Weeks 6-7: ED Pilot Integration**
- Integrate with one ED radiology PACS
- Build triage notification system
- Deploy model in pilot environment
- Collect time-to-diagnosis metrics

**Deliverables:** Live pilot with one ED radiology group

**Week 8: Refinement & Demo Prep**
- Refine model based on pilot feedback
- Prepare RSNA conference demo
- Draft case study materials

**Deliverables:** Conference-ready demo, pilot results

### Validation Metrics

| Metric | Target | Why |
|--------|--------|-----|
| **Sensitivity** | >0.90 | Cannot miss PE (life-threatening) |
| **Specificity** | >0.85 | Avoid excessive false alarms |
| **Time Reduction** | 50%+ reduction in time-to-diagnosis | Measurable ROI |
| **Pilot Commitment** | One ED commits post-pilot | Commercial validation |

---

## 9. Tech Stack

### Backend & Infrastructure

| Component | Technology | Rationale |
|-----------|------------|-----------|
| **Backend** | Python/FastAPI | Async, fast development, medical imaging ecosystem |
| **AI Framework** | PyTorch + MONAI | Medical imaging optimized, 3D CNN support |
| **DICOM Processing** | pydicom, GDCM | Industry standard for medical imaging |
| **Task Queue** | Celery + Redis | Async scan processing |
| **Database** | PostgreSQL | Patient data, findings, audit logs |
| **Storage** | AWS S3 (HIPAA) | CT volume storage (100-500MB per scan) |
| **GPU Compute** | AWS p3/p4 instances | Model training and inference |

### Integrations

**PACS (Picture Archiving and Communication System)**
- DICOM listeners for incoming studies
- HL7 messages for study orders/results
- Modality worklist integration

**EHR (Electronic Health Records)**
- Epic (Interconnect, FHIR)
- Cerner ( millennium platform)
- Meditech

**RIS (Radiology Information Systems)**
- Study status updates
- Report generation
- Worklist prioritization

### Compliance & Security

- **HIPAA compliant** infrastructure (AWS BAA)
- **SOC 2 Type II** certification (planned Year 1)
- **FDA Class II** pathway (510(k) de novo or predicate)
- **Audit logging** for all patient data access
- **Encryption at rest and in transit**

---

## 10. Market Analysis

### Market Size

**TAM (Total Addressable Market):** $4.2B
- 6,000+ hospitals in the US
- 35,000+ radiologists
- 100M+ CT exams annually
- 30% of CTs are emergency/urgent = 30M exams
- At $1/exam potential = $30M annual software market
- Global expansion (Europe, Asia) = 3-4x US market

**SAM (Serviceable Addressable Market):** $800M
- US emergency departments (1,000+ hospitals with 24/7 ED)
- Teleradiology firms (major: vRad, RadNet, NightHawk)
- Target 20% penetration = 200 hospitals = $40M ARR potential

**SOM (Serviceable Obtainable Market):** $150M
- 3-year penetration target: 180 hospitals
- Average $2,500/month = $5.4M ARR
- At 20x revenue multiple = $108M valuation

### Competitive Landscape

| Competitor | Focus | Strength | Weakness vs. CTTriageAI |
|------------|-------|----------|-------------------------|
| **Aidoc** | General radiology AI | First mover, multiple findings | Not ED-focused, general radiology workflow |
| **Annalise.ai** | Triage + reporting | Comprehensive findings | Global (not US ED focus), expensive |
| **GE Healthcare** | CT AI features | Installed base (CT scanners) | Hardware-locked, not workflow-focused |
| **Siemens** | CT AI built-in | Scanner integration | Hardware vendor, not software-first |
| **Imalogix** | Radiology analytics | Practice analytics | Not diagnostic AI |
| **Gleamer** | X-ray AI | Strong X-ray | Not CT-focused |

### Differentiation

**Only platform focused on EMERGENCY triage:**
- Time-to-diagnosis as primary metric
- ED workflow optimization (not general radiology)
- Critical finding specialization (PE, stroke, trauma)
- Teleradiology optimization (night/weekend reads)

---

## 11. Risk Factors

### Regulatory Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| **FDA Class II pathway** | 12-24 month timeline, $1-2M cost | Start with 510(k) predicate, regulatory counsel |
| **Reimbursement unclear** | Hospital budget resistance | ROI on quality metrics, malpractice reduction |
| **State medical board rules** | Varying AI practice rules | Work as "decision support," not diagnosis |

### Technical Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| **CT data quality variability** | Model performance degrades | Data augmentation, domain adaptation |
| **False negatives** | Missed PE = patient harm | >0.90 sensitivity target, radiologist review |
| **False positives** | Alarm fatigue | >0.85 specificity target, learning from feedback |
| **PACS integration complexity** | Long deployment | Pre-built integrations for major vendors |

### Commercial Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| **ED sales cycles** | 6-12 month sales cycles | Target radiology groups (shorter cycles) |
| **Competition** | Aidoc, Annalise well-funded | ED focus = differentiation |
| **Radiologist resistance** | "AI will replace me" | Augmentation narrative, radiologist advisors |
| **Hospital IT barriers** | Security concerns, deployment | Cloud deployment, SOC 2, HIPAA compliance |

### Clinical Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| **Model drift** | Performance degrades over time | Continuous monitoring, retraining pipeline |
| **New CT protocols** | Model fails on new scanners | Ongoing data collection, domain adaptation |
| **Liability** | Misdiagnosis lawsuits | Clear product labeling, radiologist stays decision-maker |

---

## 12. Go/No-Go Decision: GO

**Score: 8.67/10 - PURSUE**

### Critical Success Factors

1. **Hire radiologists as co-founders/advisors**
   - Credibility with customer base
   - Clinical workflow understanding
   - FDA pathway navigation

2. **Partner with one ED radiology group**
   - Real-world feedback
   - Pilot site for validation
   - Reference customer for sales

3. **Start with PE detection**
   - Highest urgency (life-threatening)
   - Binary detection (AI-friendly)
   - Clear time-to-diagnosis impact

4. **Focus on time-to-diagnosis metric**
   - Measurable ROI for hospitals
   - Differentiation from competitors
   - Quality metric alignment

5. **Build RSNA conference relationships**
   - Largest radiology gathering
   - Thought leadership platform
   - Customer acquisition channel

### Why This Scores 8.67

**Strengths:**
- 100M CT exams annually = highest volume imaging modality
- Emergency urgency = life-saving (minutes matter)
- 3D CNNs = ideal for CT (AI-native application)
- Clear validation path (PE binary detection)
- $2,500/month pricing = ED budgets can afford
- High switching costs = low churn
- Time-to-diagnosis = measurable ROI

**Weaknesses:**
- Competition exists (Aidoc, Annalise)
- FDA Class II pathway required (time, cost)
- ED sales cycles = 6-12 months

**The Verdict:**
This is a **life-saving emergency AI application** with measurable time impact. The highest urgency, largest addressable market, and clear AI-native technical approach make this worth pursuing.

The key is **focus**: ED triage only (not general radiology), time-to-diagnosis as primary metric, and PE detection as entry wedge.

---

## 13. Next Steps

### Immediate Actions (Week 1)

1. **Form founding team**
   - Technical co-founder (ML/medical imaging)
   - Clinical co-founder/advisor (radiologist)
   - Regulatory advisor (FDA pathways)

2. **Secure pilot partnership**
   - Identify ED radiology group for pilot
   - Draft MOU for data access/validation

3. **Begin data collection**
   - IRB application for CT dataset access
   - Identify public datasets (RSNA, Kaggle)

4. **Build regulatory roadmap**
   - Engage FDA counsel
   - Map 510(k) pathway with predicate devices

### Milestones for First 6 Months

| Month | Milestone | Success Criteria |
|-------|-----------|------------------|
| 1-2 | Data collection + model setup | 500+ PE CT studies annotated |
| 3-5 | PE detection model built | >0.90 sensitivity, >0.85 specificity |
| 5-6 | Pilot deployment | 1 ED radiology group live |
| 6 | Pilot results | 50%+ time-to-diagnosis reduction |
| 6-8 | Fundraising / FDA filing | Seed round or 510(k) submission |

---

## Appendix: Key Resources

### Datasets
- RSNA Pulmonary Embolism Detection Challenge
- RadImageNet (medical imaging pre-training)
- MIMIC-CXR (though X-ray, relevant for transfer)

### Frameworks
- MONAI (Medical Open Network for AI)
- PyTorch Medical Imaging
- NVIDIA Clara (medical imaging SDK)

### Regulatory
- FDA Software as a Medical Device (SaMD) guidelines
- 510(k) pathway resources
- DICOM standards

### Conferences
- RSNA Annual Meeting (November/December)
- ARRS Annual Meeting (April/May)
- ASER (American Society of Emergency Radiology)
- SIIM (Society for Imaging Informatics in Medicine)

---

**Document Version:** 1.0
**Last Updated:** 2026-03-02
**Status:** GO - Proceed to MVP development
