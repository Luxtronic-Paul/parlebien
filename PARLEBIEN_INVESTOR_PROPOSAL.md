# ParleBien — Investor Brief
### Verbal Learning Platform | Seed Stage
*Confidential — For Discussion Purposes Only*

---

## The One-Paragraph Pitch

ParleBien is a voice-first verbal learning platform built on the oldest and most proven learning method in existence — the flashcard — reimagined for the age of AI. Starting with adult language learning and expanding into children's development, speech pathology practice, and academic subject drilling, ParleBien does what no major competitor has done: it puts speaking at the centre of the learning loop. Users hear a word, process it, and speak their answer aloud — replicating the exact sequence through which every human being on earth first acquired language. The platform is live today at parlebien.com, validated on real devices, architectured to scale across five product modules, and positioned to capture meaningful share of a $47B global edtech market.

---

## The Foundational Principles

*These are not marketing positions. They are the pedagogical spine of everything ParleBien builds.*

### 1. The Historic Flashcard Foundation

Flashcards are not a trend. They are one of the oldest and most battle-tested learning tools in human history — used for over 200 years by medical students memorising anatomy, military linguists preparing for foreign postings, diplomats learning languages before assignments abroad, and children learning to read in every culture on earth.

The reason flashcards have survived while countless other learning methods have come and gone is simple: they work. They enforce two mechanisms that neuroscience has repeatedly validated as the most effective pathways to long-term retention:

- **Spaced repetition** — reviewing material at increasing intervals as it becomes more familiar, exploiting the spacing effect first documented by psychologist Hermann Ebbinghaus in 1885
- **Active recall** — being required to *produce* an answer from memory, rather than recognise it from a list — which produces 2–3x stronger retention than passive reading or multiple choice selection

Every major language learning app of the past decade has attempted to gamify this process. None of them have preserved what made the original method work. ParleBien does.

---

### 2. Verbal-First Memory Imprint — The Learning Sequence That Matters

The sequence in which information enters the brain determines how durably it is encoded. ParleBien is built around a specific three-stage sequence that mirrors how the brain actually forms lasting memories:

```
HEAR / SEE  →  PROCESS (transcribe internally)  →  VOCALIZE
```

This sequence is not arbitrary. Each stage engages a distinct memory system:

- **Auditory input** activates the phonological loop — the brain's verbal working memory system
- **Internal processing** (the moment between hearing and responding) forces active retrieval — the learner must search their memory, not copy from a visual prompt
- **Vocalization** creates motor memory — the muscle memory of pronunciation, the physical act of forming sounds — which is among the most durable forms of human memory

When all three engage simultaneously, the result is a multi-encoded memory trace that is significantly more resistant to forgetting than any single-channel input. This is the science behind why ParleBien requires learners to *speak* their answers rather than tap or type them.

---

### 3. A First Principle — Children Learn to Speak Before They Read

This is perhaps the most overlooked insight in edtech: every human being on earth learns language verbally first.

Before a child reads a single letter, before they write a single word, they have already acquired thousands of words through listening and speaking. The spoken language comes first — always, in every culture, in every language, across all of recorded human history. Reading and writing are secondary technologies layered on top of an oral foundation that is already in place.

Yet the overwhelming majority of language learning apps — and educational software broadly — treat text as the primary medium. They show words. They ask learners to tap words. They grade written responses. They are, at a fundamental level, working against the sequence through which the human brain naturally acquires language.

ParleBien inverts this. The spoken word is primary. Text is the support layer.

This first principle extends directly into the children's modules. LinguaKids and SoundSteps are built on the understanding that young children's brains are optimised for verbal acquisition in a way that fades with age. The earliest years are the highest-leverage window for language and vocabulary development — and they are almost entirely oral.

---

### 4. Triple-Channel Encoding — Vocal, Visual and Auditory Simultaneously

The most effective learning engages multiple sensory channels at the same time. When a learner:

- **Sees** a word on screen (visual encoding)
- **Hears** it spoken aloud by the app (auditory encoding)
- **Says** it themselves in response (motor / vocal encoding)

...three independent memory pathways are activated in a single learning moment. Research in cognitive science consistently shows that multi-modal encoding produces stronger, more accessible, and more durable memories than single-channel input.

This is not a feature of ParleBien. It is the architecture of ParleBien. Every interaction in the app is designed to engage all three channels:

- The prompt is displayed visually
- The app reads it aloud on demand (or automatically in Listen & Respond mode)
- The learner must speak their answer — not type it, not tap it — speak it

This triple-channel approach is equally applicable to a five-year-old learning animal names, a thirty-year-old learning French verbs, and a child in speech therapy practicing the "r" sound. The channel architecture scales across every product module.

---

### 5. AI as the Teacher in the Room

A skilled human teacher does several things that no textbook or passive app can replicate:

- Listens to your answer and evaluates it in real time
- Recognises when you were close but not quite right
- Corrects your pronunciation specifically, not generically
- Gives you immediate feedback — not at the end of a test
- Adapts to your pace and your specific weaknesses
- Encourages you when you are struggling
- Tracks your progress over weeks and months

The limiting factor for every learner has always been access to that teacher — the hours of supervised practice that produce fluency. Private tutors cost $40–100 per hour. SLP sessions cost $150–300 per hour. There are simply not enough practice hours available to most learners.

ParleBien's AI layer replicates the teacher's core function: it listens, it evaluates, it corrects, it encourages, and it tracks — at any hour, at any pace, at any price point. It does not replace the teacher. It provides the hundreds of practice repetitions between teacher sessions that no human teacher has time to give.

The current implementation uses fuzzy phonetic matching to evaluate spoken responses with tolerance for accent, speed, and minor pronunciation variation — the same tolerance a good teacher would apply. The roadmap adds Azure Pronunciation Assessment API for phoneme-level scoring, which enables genuine clinical-grade feedback for the SoundSteps speech pathology module.

The AI is not a gimmick in ParleBien. It is the mechanism that makes the teacher-in-the-room model scalable to millions of learners simultaneously.

---

## The Problem

Language learning apps teach you to read and tap. They do not teach you to speak.

Duolingo has 500 million downloads and a $5B valuation. It also has a fundamental pedagogical flaw — the majority of its exercises are multiple choice, tap-the-word, or fill-in-the-blank. Passive recognition, not active production. The very sequence that produces durable memory — hear, process, vocalize — is absent from the dominant product in the market.

The same gap exists across education broadly:
- Children practice spelling by writing, not speaking
- Math students drill times tables by reading, not reciting
- Homeschool parents have no voice-based practice tool for any subject
- Children with speech difficulties have no affordable at-home practice companion between therapy sessions that cost $150–300 per hour with waitlists measured in months

---

## The Solution — Five Modules, One Engine

A single core engine — present a prompt, evaluate a spoken response, track progress over time — deployed across five distinct product modules:

| Module | Target User | Core Problem Solved |
|---|---|---|
| **ParleBien** | Adult language learners | Speaking practice with custom vocabulary |
| **LinguaKids** | Children ages 3–12 | Age-appropriate verbal vocabulary building |
| **World Explorer** | Families traveling internationally | Destination language prep as a family activity |
| **SoundSteps** | Children in speech therapy + SLPs | At-home practice between therapy sessions |
| **MathVoice / ScienceSpeak** | Homeschool and K–12 students | Verbal drill for any academic subject |

Each module is a focused product with its own buyer and price point. All five share the same underlying technology, the same payment infrastructure, and the same content management system.

---

## Practice Modes — The Learning Loop in Action

ParleBien implements the See → Process → Vocalize sequence across five distinct practice modes, each targeting a different learning stage:

**English → Target Language** — See the English word, speak the French or Spanish translation. Classic active production.

**Target Language → English** — See the foreign word, speak the English meaning. Tests recognition and retrieval.

**Tense Practice** — See the infinitive verb, speak the conjugated form in present, past, or future tense. The full verb tense sequence forces learners through all three forms in a single card.

**Phrases Mode** — Full phrases and conversational sentences, not isolated words.

**Listen & Respond** *(in development)* — The app speaks a word or phrase in Language A. No text shown. The learner must respond in Language B. The answer remains masked until after the response. This is the most authentic mode — replicating real conversation where you hear, not read. It is also the most demanding, and therefore the most effective for advanced retention.

**Speed Flash** *(in development)* — Three words shown simultaneously, five second countdown. High pressure, high engagement, high retention.

---

## Traction

- **Live product:** parlebien.com — fully functional, deployed, accessible on any device in any country
- **Technology validated:** Voice input, fuzzy phonetic matching, text-to-speech, and custom vocabulary import all working in production on Android (Pixel 9 Pro, Chrome)
- **Content library:** 12 pre-built word sets across French and Spanish (240 words and phrases), expanding
- **Architecture proven:** Single codebase supports multiple languages, multiple practice modes, tiered access control, and word persistence — without a backend server
- **Domain secured:** parlebien.com — HTTPS active, mic permissions save permanently

*Note: This is pre-revenue, pre-institutional user base. Traction metrics reflect technical validation and product completeness, not commercial scale.*

---

## Market Opportunity

### Total Addressable Market

| Market | Size | Source |
|---|---|---|
| Global e-learning | $457B by 2026 | Grand View Research |
| Language learning apps | $21.2B by 2027 | Mordor Intelligence |
| Speech therapy tools | $4.8B by 2027 | Allied Market Research |
| US homeschool curriculum spend | $1.2B annually | NHERI |

### Serviceable Addressable Market

- 1.5M active adult language learners in English-speaking markets seeking Duolingo alternatives
- 3.3M homeschooled children in the US — parents spend $700–1,800 per child per year on curriculum
- 1.8M children receiving speech-language therapy in the US, significant unmet demand for home practice

**Conservative SAM:** $380M

### Serviceable Obtainable Market (36 months)

- 10,000 paying users at blended ARPU of $4/month = $480K ARR
- Physical/PDF flashcard orders as secondary revenue stream
- Institutional licensing as a third stream

---

## Business Model

### Consumer Tiers (Recurring)

| Tier | Price | Features |
|---|---|---|
| Free | $0 | 50 custom words, all practice modes |
| Basic | $1/month | 150 words + PDF flashcard export |
| Premium | $5/month | Unlimited words + print discount + all modes |

### One-Time Orders (Transactional)

| Product | Price | Margin | Fulfillment |
|---|---|---|---|
| Print-ready PDF | $3–5 | ~95% | Automated — PDF from user's word set |
| Printed & shipped deck | $12–15 | ~40% | Print-on-demand via Gelato API |
| Digital deck export | $1–2 | ~99% | Automated (Anki / Quizlet format) |

### Institutional

| Product | Price | Notes |
|---|---|---|
| SLP professional account | $29/month | Covers all patient profiles |
| School district license | $2–5 per student per year | Bulk pricing |
| Homeschool co-op license | $49/month | Up to 20 families |

### Unit Economics (Projected at Scale)

- **CAC:** $4–8 via homeschool co-op referral and SLP recommendation (word-of-mouth dominant)
- **LTV** at $5/month, 18-month average retention: $90
- **LTV:CAC ratio:** ~12:1 at target scale
- **Gross margin:** 85%+ on subscription revenue

---

## Competitive Landscape

| Competitor | Strength | Critical Weakness |
|---|---|---|
| Duolingo | 500M users, brand, gamification | Passive exercises, no custom vocabulary, speaking secondary |
| Anki | Powerful spaced repetition | No voice, terrible UX, no guided content |
| Quizlet | Easy content creation | No voice-first interaction |
| Rosetta Stone | Established brand | $11.99/month, fixed curriculum, no customisation |
| Babbel | High quality lessons | Fixed curriculum, no custom vocabulary |
| Speech Blubs | Children's speech practice | No custom content, no SLP integration, no progress tracking |

### ParleBien's Defensible Differentiation

1. **Pedagogically grounded** — built on 200 years of flashcard science, not engagement metrics
2. **Voice-first by design** — speaking is the primary interaction, not an afterthought feature
3. **Custom vocabulary** — users practice *their* words, not a generic curriculum
4. **The Listen & Respond mode** — no competitor offers pure audio prompt → spoken response → masked reveal
5. **Platform architecture** — one engine, five markets, five revenue streams
6. **Physical product bridge** — flashcard ordering creates tangible touchpoint no pure software competitor offers
7. **SLP distribution channel** — professional accounts create B2B referral engine into the consumer market

---

## Go-To-Market Strategy

### Phase 1 — Friends, Family & Early Adopters (Now)
Goal: 100 active users, qualitative feedback on the core loop

### Phase 2 — Homeschool Community (Months 3–9)
- Target homeschool co-op leaders as distribution nodes
- Presence at regional homeschool curriculum fairs
- Goal: 1,000 paying users, first revenue

### Phase 3 — SLP Professional Channel (Months 6–18)
- Reach SLPs via ASHA channels
- 50 free professional accounts in exchange for structured feedback
- Each endorsing SLP refers 20–30 families
- Goal: 50 SLP accounts generating 1,000+ family subscriptions

### Phase 4 — Paid Acquisition + Institutional (Months 12–24)
- Google and Meta targeting language learners and homeschool parents
- School district outreach for site licenses
- Android app launch (Capacitor wrapper)
- Goal: 10,000 paying users, $480K ARR

---

## Product Roadmap

### Next 90 Days
- Landing page (science of flashcards, feature highlights, email capture)
- Listen & Respond mode (audio prompt, masked answer)
- Speed Flash mode
- CSV upload/download
- Google Analytics integration

### 90 Days — 12 Months
- Stripe payments (monetisation begins)
- Supabase backend (accounts, cross-device sync)
- LinguaKids v1
- SoundSteps v1 (Azure Pronunciation Assessment)
- Physical/PDF flashcard ordering
- Android app

### 12–24 Months
- SLP professional accounts
- Homeschool parent dashboard
- MathVoice module
- iOS app
- School district licensing

---

## The Team

*[To be completed — founder background, advisors, early team]*

**Seed stage hiring plan:**
- CTO / Lead Engineer — Supabase, Stripe, React migration, mobile
- Content Lead — word sets, curriculum alignment, SLP liaison
- Growth — homeschool community, SLP outreach, paid acquisition

---

## Financial Projections

### Conservative Scenario

| Year | Total Users | Paying | ARPU/mo | ARR |
|---|---|---|---|---|
| Year 1 | 2,500 | 500 | $3.20 | $19,200 |
| Year 2 | 12,000 | 3,000 | $3.80 | $136,800 |
| Year 3 | 40,000 | 12,000 | $4.20 | $604,800 |

### Base Scenario

| Year | Total Users | Paying | ARPU/mo | ARR |
|---|---|---|---|---|
| Year 1 | 5,000 | 1,200 | $3.50 | $50,400 |
| Year 2 | 25,000 | 7,500 | $4.00 | $360,000 |
| Year 3 | 80,000 | 28,000 | $4.50 | $1,512,000 |

### Upside Scenario

| Year | Total Users | Paying | ARPU/mo | ARR |
|---|---|---|---|---|
| Year 1 | 8,000 | 2,000 | $4.00 | $96,000 |
| Year 2 | 45,000 | 15,000 | $4.80 | $864,000 |
| Year 3 | 150,000 | 55,000 | $5.20 | $3,432,000 |

*Projections exclude flashcard orders and institutional licensing — meaningful additional upside*

---

## Use of Funds

### Pre-Seed Ask: $150,000 — $250,000

| Allocation | Amount | Purpose |
|---|---|---|
| Engineering (contract) | $80,000 | Supabase, Stripe, mobile app |
| Content development | $25,000 | Word sets, LinguaKids, SoundSteps |
| Go-to-market | $30,000 | Homeschool fairs, SLP outreach, initial paid acquisition |
| Legal & compliance | $15,000 | Trademark, privacy, COPPA |
| Operations | $20,000 | Azure API, Gelato print partner, tooling |
| Reserve | $30,000 | 6-month runway buffer |

**Runway at $250K:** 18–24 months to revenue positive at conservative projections

---

## Key Risks & Mitigations

| Risk | Likelihood | Mitigation |
|---|---|---|
| Duolingo copies voice-first approach | Medium | Custom vocabulary + platform breadth creates moat they cannot replicate quickly |
| Speech recognition accuracy on mobile | Low | Validated on Android Chrome; Azure API adds clinical robustness |
| COPPA compliance for children's products | Medium | Legal budget allocated; parent-controlled tool positioning |
| SLP adoption slower than projected | Medium | Homeschool channel is parallel, not dependent |
| Single-founder execution risk | Medium | Contract engineering mitigates; early hire plan in place |

---

## Why Now

**1. The science has always been right — the technology just caught up.**
The pedagogical principles behind ParleBien are 200 years old. What is new is a Web Speech API mature enough to evaluate spoken responses reliably on a consumer mobile device. That threshold was crossed in the last 18–24 months.

**2. The dominant player has a structural flaw.**
Duolingo's entire product is built around tapping and typing. Rebuilding it around speaking would require dismantling and rebuilding its core interaction model — a near-impossible pivot for a public company with 500M habituated users. This is ParleBien's window.

**3. Post-COVID learning infrastructure shift.**
3.3M US homeschoolers (up from 2.5M pre-COVID). Demonstrated willingness to pay for digital learning tools. Parents who are now the primary educators are actively seeking curriculum supplements.

**4. SLP shortage creates urgent demand.**
Pediatric speech therapy waitlists are 6–18 months in most US cities. The at-home practice market has never been more motivated or more underserved.

**5. The product exists.**
This is not a pitch for a concept. parlebien.com is live, working, tested on real devices, and in users' hands today.

---

## Contact

*[Founder name]*
*[Email address]*
parlebien.com
github.com/Luxtronic-Paul/parlebien

---

*This document is confidential and intended solely for the named recipient. Financial projections are illustrative, based on market research and comparable company benchmarks, and do not constitute a guarantee of future performance.*

