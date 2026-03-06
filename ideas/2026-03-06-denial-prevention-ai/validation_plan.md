# Denial Prevention AI - Validation Plan

## Hypothesis

Specialty practices will pay $500/month for AI that prevents claim denials before submission, reducing denial rates by 40%+.

## Riskiest Assumptions

1. Practices can integrate before claim submission (not just post-denial analysis)
2. Payer-specific patterns exist and are learnable
3. 40% denial reduction is achievable
4. $500/month pricing resonates

## Validation Experiments

### Experiment 1: Payer Pattern Analysis (Week 1)

**Goal:** Prove payer-specific denial patterns are identifiable

**Method:**
- Acquire 10K+ denied claims dataset
- Cluster by payer + denial reason
- Build classifier predicting denials
- Target: 70%+ accuracy on top 5 denial reasons per payer

**Success:** 5 payers with identifiable, predictable patterns

### Experiment 2: Wizard-of-Oz MVP (Week 2-3)

**Goal:** Test pre-submission workflow integration

**Method:**
- Recruit 5 specialty practices
- Manual analysis of 100 claims/practice before submission
- Email daily "claims at risk" report
- Track prevented denials vs baseline

**Success:** 3+ practices integrate into workflow, 30%+ denial reduction

### Experiment 3: Pricing Test (Week 4)

**Goal:** Validate $500/month price point

**Method:**
- Offer 3 tiers: $350, $500, $750
- 3-month commitment required
- Track conversion by tier

**Success:** >60% choose $500 or higher

### Experiment 4: Landing Page Smoke Test (Week 1-4, parallel)

**Goal:** Measure interest and collect leads

**Method:**
- PPC ads: "prevent claim denials before submission"
- Landing page: demo request + email capture
- Track: CTR, conversion, demo requests

**Success:** >15% conversion from ad → demo request

## Success Criteria

| Metric | Target | Timeline |
|--------|--------|----------|
| Paying customers | 5 | Week 4 |
| Denial reduction | 35%+ | Week 3 |
| Price acceptance | $500+ | Week 4 |
| Integration rate | 80% | Week 3 |

## Pivot Triggers

- **Pivot** if denial reduction < 20% (not enough value)
- **Pivot** if integration > 4 weeks (too hard to adopt)
- **Lower price** if >80% choose $350 tier
- **Niche down** if general specialty adoption < 20%

## Next Steps After Validation

1. **Build automated claim parser** (X12 837p)
2. **Expand payer coverage** to top 10 by market share
3. **Add EHR integrations** (Epic, Cerner, athena)
4. **Hire 2 SDRs** for outbound
