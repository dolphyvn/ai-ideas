# Validation Plan - AI Receptionist Network

## Phase 1: Problem Validation (Days 1-2)

### Goal:
Confirm local businesses actually miss calls and care.

### Method:
**Walk-in Validation**
- Target: 20 local businesses in one area
- Mix: Hair salons (8), auto repair (6), spas (4), other (2)
- Time: 2-5pm (slower period, owners available)

**Script:**
"Hi, I'm a local entrepreneur. Quick question: How many calls do you miss per week because you're with customers or closed?"

Then:
"If I could guarantee every call gets answered, appointments get booked 24/7, and it costs $99/month—would you try it free for a week?"

### Success Criteria:
- 10+ say they miss 5+ calls/week
- 5+ agree to trial
- 3+ express urgency ("I need this now")

### Kill Criteria:
- <3 businesses care
- "I have voicemail, it's fine" >70%
- "Already using [Ruby/Sameday]" >40%

---

## Phase 2: Solution Validation (Days 3-4)

### Goal:
Test if voice AI actually works in real environment.

### Method:
1. Set up Vapi.ai account (3 hours)
2. Configure basic phone number (1 hour)
3. Build simple calendar integration (Calendly, 4 hours)
4. Deploy to 1 willing business from Phase 1

**Day 3 Setup:**
- Business: [Name]
- Phone: Forward existing number or new line
- Knowledge Base: Hours, services, pricing, booking link

**Day 4 Test:**
- Owner calls from personal phone
- Friend calls as new customer
- Monitor: Conversation quality, booking success

### Success Criteria:
- AI handles basic booking successfully
- Owner says "this actually worked"
- Customer understood it was AI or was neutral

### Kill Criteria:
- AI fails to book appointment
- Owner says "too robotic"
- Caller hangs up confused

---

## Phase 3: Viral Validation (Days 5-6)

### Goal:
Test if customers actually notice/talk about AI receptionist.

### Method:
1. Deploy to 3 businesses total
2. Add exit question: "How was your booking experience?"
3. Monitor Google Reviews for mentions
4. Ask owners: "Any customer comments?"

### Success Criteria:
- 1+ customer mentions AI unprompted
- 1+ customer posts about it (social, review)
- Owner says "customers are surprised/impressed"

### Kill Criteria:
- Negative customer sentiment
- "I prefer human" >50% feedback
- Businesses ask to turn it off

---

## Phase 4: Revenue Validation (Days 7-10)

### Goal:
Test willingness-to-pay after trial.

### Method:
**Pricing Offer:**
- $99/month - Starter
- $199/month - Pro (custom voice)
- $149 setup fee

**Conversion Call:**
"Trial's over. Results: X calls answered, Y appointments booked. Ready to continue?"

### Success Criteria:
- 2+ convert to paid
- At least 1 chooses Pro tier
- None ask for major price reduction

### Kill Criteria:
- Everyone asks for free/cheaper
- "I'll just hire someone" pushback
- 0 conversions

---

## Phase 5: Expansion Validation (Days 11-14)

### Goal:
Test if this scales beyond first 3 businesses.

### Method:
- Referrals from initial 3: "Who else do you know?"
- Walk same area, social proof: "[Salon down street] uses this"
- Target: 10 more businesses

### Success Criteria:
- 5+ new trials from referrals
- 3+ new signups from walk-ins with social proof
- 1 multi-location business expresses interest

### Kill Criteria:
- Area saturation at <5 businesses
- Referral rate = 0
- "Everyone knows everyone and no one wants it"

---

## Total Validation Timeline: 14 Days

## Go/No-Go Decision Criteria:

### GO if:
- 5+ paying customers by Day 14
- 80%+ customer satisfaction
- <$40 CAC (walk-in cost)
- Positive word-of-mouth happening

### NO-GO if:
- <3 paying customers
- Negative customer sentiment
- Churn during validation period
- Technical issues can't be resolved

---

## Fallback Plan:
If standalone validation fails, pivot to:
1. **White-label**: Sell to existing marketing agencies serving SMBs
2. **Vertical-only**: Focus only on dental or medical (higher willingness-to-pay)
3. **DIY kit**: Sell "build your own AI receptionist" course + templates
