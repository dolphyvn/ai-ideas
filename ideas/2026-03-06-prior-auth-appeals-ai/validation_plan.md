# Prior Auth Appeals AI - Validation Plan

## Hypothesis

Practices will pay $750/month for AI that generates winning prior auth appeal letters with clinical rationale, achieving 60%+ first-level success.

## Riskiest Assumptions

1. AI can generate clinically-valid appeal rationales
2. Practices will share patient records for analysis
3. 60% success rate is achievable
4. Cycle 110 customers will upsell (natural extension)

## Validation Experiments

### Experiment 1: Clinical Rationale Quality (Week 1)

**Goal:** Prove AI can generate valid clinical appeals

**Method:**
- Collect 50 real denied prior auth cases
- Manually extract denial reasons + patient records
- Generate appeal letters using Claude
- Have 3 physicians review on: clinical accuracy, persuasiveness
- Target: 4/5 average rating

**Success:** 80% rated "would use this letter"

### Experiment 2: Wizard-of-Oz MVP (Week 2-3)

**Goal:** Test real-world appeal success

**Method:**
- Recruit 5 practices (2 from Cycle 110)
- For each denial: generate appeal letter
- Track: first-level success, time to overturn
- Compare to baseline appeal win rate

**Success:** >50% first-level success, 2x improvement

### Experiment 3: Cycle 110 Upsell Test (Week 2-3, parallel)

**Goal:** Validate upsell potential

**Method:**
- Email Cycle 110 customers with offer
- 50% discount for first 3 months
- Demo + case study template
- Track conversion

**Success:** >30% convert (natural upsell confirmed)

### Experiment 4: Payer Pattern Analysis (Week 1, parallel)

**Goal:** Map payer denial patterns

**Method:**
- Research top 5 payers' appeal processes
- Document: denial codes, required evidence, timeliness
- Build payer-specific templates

**Success:** Playbook for top 5 payers

## Success Criteria

| Metric | Target | Timeline |
|--------|--------|----------|
| Clinical rating | 4/5 | Week 1 |
| Appeal success rate | 50%+ | Week 3 |
| Cycle 110 conversion | 25%+ | Week 3 |
| Upsell pipeline | 10 leads | Week 2 |

## Pivot Triggers

- **Pivot** if clinical rating < 3/5 (AI not good enough)
- **Pivot** if success rate < 30% (not enough value)
- **Niche down** if general appeal success < 40% (focus on drug/specialty)
- **Human-in-the-loop** if AI appeals rejected > 50% (hybrid model)

## Next Steps After Validation

1. **Build EHR integration** for record extraction
2. **Expand payer templates** to top 10
3. **Create peer-to-peer prep** for second-level appeals
4. **Hire clinical consultant** for quality assurance
