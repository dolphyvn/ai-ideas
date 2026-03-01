# AI Venture Spec

## Name:
**AI Receptionist Network**

## Core Concept:
A voice AI receptionist that answers phones for local SMBs, handles appointment booking, answers FAQs, and never misses a customer call. Plug-and-play deployment with existing phone systems.

## Problem:
- **Missed calls = missed revenue**: Local businesses lose 20-40% of new customers to voicemail
- **After-hours gap**: No booking capability when staff goes home
- **Labor cost**: Front desk staff costs $3,000-$5,000/month
- **Inconsistent experience**: Human receptionists have bad days, forget details
- **Scalability constraints**: Can't handle multiple simultaneous calls

## Target Vertical:
**Primary**: Local service businesses with appointment-based models
- Hair salons & barbershops
- Auto repair shops
- Medical practices (chiropractors, dentists, therapists)
- Spas & wellness centers
- Pet groomers

**Initial Wedge**: Hair salons + barbershops (high call volume, clear scheduling logic)

## Why Now:
1. **Sub-300ms latency voice AI**: Real-time conversations now feel natural
2. **Vapi/Retell APIs**: Voice infrastructure is plug-and-play (was custom build 18mo ago)
3. **Calendar API maturity**: Calendly, Square, Google Calendar integrations are stable
4. **SMB labor crisis**: Minimum wage increases + hiring shortages
5. **Consumer expectation shift**: "Why can't I book at 10pm?"

## AI Advantage:
- **Natural conversation**: Sub-300ms response time (indistinguishable from human)
- **Context awareness**: Remembers customer preferences, history
- **Multi-intent handling**: Can reschedule AND answer pricing in same call
- **Voice cloning**: Custom voice per business (brand consistency)
- **24/7 availability**: Never sleeps, never calls in sick

## Viral Mechanism:
- **Consumer-visible**: Every caller experiences the AI ("I didn't know I was talking to AI!")
- **Story-worthy**: TikTok/Reels of impressive AI interactions
- **Local FOMO**: Salon A uses it → Salon B's customers ask "why don't you have this?"
- **Review sharing**: "Sorry I missed you, our AI receptionist helped you" (visible on Google Reviews)
- **Demo calls**: Share recordings of funny/impressive interactions

**Viral Loop:**
Customer experiences AI booking → Posts about it / Tells friends → Local business owners see engagement → Investigate → Deploy → Their customers share

## Revenue Model:
**Per-Location Subscription:**
- **Starter**: $99/month - Up to 100 minutes, standard voice
- **Pro**: $199/month - Up to 500 minutes, custom voice clone
- **Enterprise**: $399/month - Unlimited minutes, multi-location, priority support

**Setup Fees:**
- $149 one-time (voice training, calendar integration)

**Unit Economics:**
- CAC: $35 (local walk-ins + referrals)
- LTV: $2,400 (24-month avg retention)
- Gross Margin: 65% (voice API costs are real)
- Payback Period: <2 months

**Expansion Revenue:**
- Multi-location businesses (3-5 locations average)
- Up-sell: SMS follow-up, review automation

## Moat:
1. **Distribution**: First in local business = relationship lock-in
2. **Integration depth**: Calendar + phone system knowledge per business
3. **Voice library**: Custom-trained voices per brand
4. **Network effects**: Multi-location businesses deploy across all locations
5. **Switching costs**: Once customers know "call anytime," removing it is downgrade

## MVP in 7 Days:
**Day 1:**
- Sign up for Vapi.ai or Retell.ai API
- Build basic phone webhook handler

**Days 2-3:**
- Calendly integration for appointment booking
- Build FAQ handling (business hours, pricing, services)

**Day 4:**
- Voice cloning (ElevenLabs) for custom voices
- Test call flow

**Days 5-7:**
- Walk into 20 local businesses (salons, auto shops)
- "AI answers your phone, books appointments. $99/month. Free trial for a week."
- Deploy on Day 6 for 3 businesses

**Validation Metric:**
- 5+ businesses agree to trial
- 3+ convert to paid after week
- 10+ appointments booked autonomously

## Tech Stack:
**Voice Infrastructure:**
- Vapi.ai or Retell.ai (turnkey voice AI)
- ElevenLabs (voice cloning)
- Twilio (phone numbers, call routing)

**Backend:**
- Python/FastAPI or Node.js
- PostgreSQL (business configs, call logs)
- Redis (real-time call state)

**Integrations:**
- Calendly API (booking)
- Google Calendar API
- Square/Appointment Plus API
- Mindbody (for salons/spas)

**Frontend:**
- Next.js (dashboard for businesses)
- Call recording/playback
- Booking calendar view

**Infrastructure:**
- AWS (ECS, RDS)
- S3 (call recordings)

## Monthly Revenue Potential (Year 1–3):
**Year 1:**
- 200 businesses × $125 ARPU = $25,000 MRR
- Focus: Single metropolitan area (proof of market)

**Year 2:**
- 1,000 businesses × $150 ARPU = $150,000 MRR
- Expand: 5-10 metro areas
- Multi-location expansion (30% of locations)

**Year 3:**
- 3,000 businesses × $175 ARPU = $525,000 MRR
- Enterprise tier (200 multi-location @ $400 = $80,000)
- **Total: $605,000 MRR / $7.3M ARR**

## Risk Factors:
1. **Margin Pressure**: Voice API costs consume 35-40% of revenue
2. **Churn**: SMBs have high churn (30-50% annual)
3. **Competition**: Sameday, Ruby, Slang.ai already exist
4. **Quality Variance**: Accents, background noise kill ASR accuracy
5. **Phone System Fragmentation**: Every business has different setup

## Competitive Threat:
- **Ruby**: Premium live receptionists, expensive ($249-$549/month)
- **Sameday**: AI + human hybrid, focuses on medical/dental
- **Slang.ai**: Similar product, better funded
- **Google Screened AI**: Could launch free version

**Differentiation:**
- 80% cheaper than Ruby
- Pure AI (no human fallback cost)
- Local sales (walk into businesses)
- Fastest deployment (24 hours vs. 2 weeks)

---

## Go/No-Go Decision: **GO** ✅

**Why:**
- Highest validation speed (9/10) - can test immediately
- Strongest viral potential (9/10) - consumer-visible
- Fast revenue (month 1)
- Clear 10x value vs. Ruby

**Next Steps:**
1. Build MVP with Vapi (3 days)
2. Walk into 20 local businesses (Day 4-5)
3. Deploy free trials (Day 6-7)
4. Launch in 14 days

**Caveat:**
- Low margins (65% vs. 85%+ for other ideas)
- High churn requires aggressive acquisition
- Play to win fast before incumbents react
