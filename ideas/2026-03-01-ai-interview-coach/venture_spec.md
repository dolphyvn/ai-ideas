# AI Venture Spec

## Name:
**AI Interview Coach**

## Core Concept:
Real-time job interview coaching via earbud. As the user practices interviews, the AI transcribes their responses, provides immediate feedback on content, tone, and delivery, and suggests improvements—all in real-time.

## Problem:
- **Job search anxiety**: Candidates are unprepared, practice alone
- **No feedback loop**: Candidates don't know how they sound
- **High stakes**: One interview determines $50K-$200K+ career outcomes
- **Coaching is expensive**: Human coaches cost $200-500/hour
- **Practice is awkward**: Talking to mirror doesn't simulate real pressure

## Target Vertical:
**Primary**: Active job seekers in high-income roles
- Tech workers (software engineers, product managers)
- Consultants, finance professionals
- Recent MBAs, career switchers

**Secondary**: University career centers, corporate L&D

## Why Now:
1. **Sub-100ms latency**: Real-time streaming is now feasible
2. **Mobile speech recognition**: On-device transcription works reliably
3. **Job market volatility**: More frequent job changes = more interviews
4. **AI coaching acceptance**: People now expect AI feedback
5. **Earbud hardware**: AirPods/Bluetooth make delivery seamless

## AI Advantage:
- **Real-time pattern matching**: Detects filler words, weak language, talking speed
- **Contextual feedback**: Understands role-specific answers (STAR method, technical concepts)
- **Adaptive difficulty**: Adjusts question difficulty based on performance
- **Voice analytics**: Tone, confidence, pacing analysis
- **Content improvement**: Suggests stronger phrasing in real-time

## Viral Mechanism:
- **Success stories**: "I got the job!" posts on LinkedIn/TikTok
- **Before/after content**: Show improvement over practice sessions
- **Celebrity endorsement**: "I used AI to prep for my CEO interview"
- **Social proof**: Shareable practice clips
- **Interview content**: Job search is inherently shareable

## Revenue Model:
**Consumer Subscription:**
- **Basic**: $49/month - Self-guided practice, common questions
- **Pro**: $99/month - Role-specific coaching, unlimited sessions
- **Premium**: $199/month - 1:1 AI customization, interview simulations

**Enterprise:**
- **Career Center**: $5K/year - University site license
- **Corporate L&D**: $10K/year - Outplacement services

**Unit Economics:**
- CAC: $75 (content marketing + TikTok)
- LTV: $600 (12-month avg)
- Gross Margin: 80%

## Moat:
1. **Performance data**: What answers actually get jobs
2. **Role-specific libraries**: Industry-specific interview patterns
3. **Real-time optimization**: Latency tricks are hard engineering
4. **Outcome network**: More users = better hiring predictions

## MVP in 7 Days:
**Days 1-2:**
- WebRTC audio capture
- OpenAI Whisper API for transcription
- Claude API for feedback generation

**Days 3-4:**
- Question library (top 50 interview questions)
- Feedback rules (filler words, conciseness, STAR method)

**Days 5-7:**
- Mobile web app
- Beta testing with 10 job seekers
- TikTok content from users

**Validation Metric:**
- 50+ practice sessions completed
- 5+ users say "this helped me get an offer"

## Tech Stack:
- **Backend**: Python/FastAPI
- **Audio**: WebRTC, Whisper API
- **AI**: Claude 4.6 for coaching logic
- **Frontend**: React Native (mobile)
- **Infrastructure**: AWS ECS, Redis

## Monthly Revenue Potential (Year 1–3):
- **Year 1**: $25K MRR (500 users × $50 ARPU)
- **Year 2**: $150K MRR (3,000 users × $50 ARPU)
- **Year 3**: $500K MRR (10,000 users × $50 ARPU)

## Risk Factors:
1. **Platform risk**: Apple/Google could block earbud access
2. **Low willingness to pay**: Job seekers are budget-constrained
3. **One-time use**: Churn after job landed
4. **Competition**: Interview preparation tools exist

## Competitive Threat:
- Google Interview Warmup (free, limited)
- Big Interview (video-based, not real-time)
- Human coaches ($300+/hour)

**Differentiation**: Real-time feedback, role-specific AI, low cost

---

## Agent Debate Summary

**Strengths:**
- Highest validation score (9/10) - can test immediately
- Real-time engineering challenge = genuine moat
- Strong viral potential in job search communities

**Weaknesses:**
- Horizontal (all job seekers, not vertical-specific)
- Low retention (churn after landing job)
- B2C monetization (lower ARPU)

**Final Score: 6.4/10**

## Go/No-Go Decision: **CONDITIONAL** ⚠️

Pursue if:
- Can achieve $75 or lower CAC
- Viral loop proves out (TikTok/LinkedIn sharing)
- Enterprise revenue (career centers) materializes

Otherwise: Pivot to vertical-specific version (Medical Interview Coach, Sales Interview Coach)
