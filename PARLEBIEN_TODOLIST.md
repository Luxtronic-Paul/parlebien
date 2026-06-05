# ParleBien — Master Project Todo List
*Document version: 1.2.0*
*Last updated: 2025-06-05*
*Session: 1 (single session — all work completed in one conversation)*
*Paste this at the start of any new Claude session to restore full context*

### Document Changelog
| Doc Ver | Date | Changes |
|---|---|---|
| 1.2.0 | 2025-06-05 | Added patent assessment, live EULA, account login spec |
| 1.1.0 | 2025-06-05 | Added offline downloadable version spec |
| 1.0.9 | 2025-06-05 | Added language selector redesign plan |
| 1.0.8 | 2025-06-05 | Added Italian and German language items |
| 1.0.7 | 2025-06-05 | Added AI dataset builder feature |
| 1.0.6 | 2025-06-05 | Added dual language speaker buttons feature |
| 1.0.5 | 2025-06-05 | Added pronunciation repeat feature, skip reveals answer |
| 1.0.4 | 2025-06-05 | Added Claude Code evaluation, Cowork migration triggers |
| 1.0.3 | 2025-06-05 | Added combined Help + Feedback + Bug Report panel |
| 1.0.2 | 2025-06-05 | Added flashcard order feature, business proposal item |
| 1.0.1 | 2025-06-05 | Added word sets, sets button, language toggle features |
| 1.0.0 | 2025-06-05 | Initial todo list created |

---

## 🚀 THE VISION
ParleBien is not just a language app. It is a **verbal learning platform** — the language module is the proof of concept. The engine (voice input, fuzzy matching, custom content, tier system, progress tracking) is subject-agnostic and extensible to math, science, homeschooling, and speech pathology.

**Current live URL:** https://parlebien.com
**GitHub repo:** https://github.com/Luxtronic-Paul/parlebien
**Stack:** Single HTML file, vanilla JS, Web Speech API, localStorage
**Hosting:** GitHub Pages + GoDaddy domain (parlebien.com)

---

## ✅ COMPLETED
- [x] Core flashcard app (English ↔ French, English ↔ Spanish)
- [x] Voice input (mic) + text input fallback always visible
- [x] Fuzzy matching (accent-forgiving, article-stripping)
- [x] Text-to-speech pronunciation playback
- [x] 5 practice modes: EN→Lang, Lang→EN, Tenses, Phrases, Random
- [x] French/Spanish language toggle with per-language theming
- [x] 6 pre-built French word sets (20 words each)
- [x] 6 pre-built Spanish word sets (20 words each)
- [x] Sets tab with filter by language + activate set → jump to practice
- [x] Custom word import (paste format: english | translation | type | tenses)
- [x] localStorage persistence (words survive between sessions)
- [x] Word limit tier system (Free 50 / Basic 150 / Unlimited)
- [x] My Words tab with delete button per imported word
- [x] Progress tracking (score, streak, accuracy %)
- [x] Stats view
- [x] Deployed to parlebien.com via GitHub Pages
- [x] HTTPS active (mic permission saves permanently on Chrome)
- [x] Tested working on Pixel 9 Pro (Chrome)

---

## 🔴 HIGH PRIORITY — BUILD NEXT

### Landing Page
- [ ] Hero section — "Speak well. Speak with confidence"
- [ ] Science of flashcards section
  - Spaced repetition (Ebbinghaus spacing effect, 1885)
  - Active recall (2–3x more effective than passive reading)
  - Multisensory learning (hear + read + speak = stronger retention)
  - Tone: warm, confident, slightly playful — "proven, not trendy"
- [ ] Feature highlights section
- [ ] Word sets preview (browsable on landing page)
- [ ] "Order My Flashcards" CTA section (see Flashcard Orders below)
- [ ] LinguaKids coming soon teaser + email capture
- [ ] Feedback button (footer)
- [ ] Dark / light mode toggle (🌙/☀️ in logo dropdown menu)
- [ ] "Launch App" button → goes to practice view
- [ ] Google Analytics 4 integration (one script tag, needs GA4 Measurement ID)

### Flashcard Orders (Physical + Digital) — HIGH PRIORITY
- [ ] "Order My Flashcards" button on My Words tab
- [ ] Order sheet with two options:
  - Print & Ship (~$12–15) — printed card stock, ring hole, shipped to door
  - Print-Ready PDF (~$3–5) — formatted PDF emailed instantly, Avery card format
  - Digital Export (~$1–2) — Anki-compatible or Quizlet import file
- [ ] Stripe payment integration for orders
- [ ] PDF generation from user's current word set (automated)
- [ ] Print-on-demand partner integration (Gelato recommended — global network, API available)
- [ ] Email delivery for PDF orders (automated fulfillment)
- [ ] Pricing fits tier system:
  - Basic $1/mo → Practice + PDF export
  - Premium $5/mo → Practice + PDF + print order discount
  - One-time → Any size, any tier

### Business Proposal Document — HIGH PRIORITY
- [ ] Build full business proposal outline from three perspectives:
  - **Investor perspective** — market size, revenue model, growth trajectory, competitive moat, exit potential
  - **CTO perspective** — current architecture, scaling path, tech debt, build vs buy decisions, team needs
  - **Potential hire perspective** — mission, product roadmap, culture, equity/comp context, growth opportunity
- [ ] Include platform vision (not just language app)
- [ ] Include all product modules (ParleBien, LinguaKids, SoundSteps, World Explorer, MathVoice)
- [ ] Include homeschool market data
- [ ] Include SLP market opportunity
- [ ] Financial projections skeleton (tier pricing × user projections)

---

## 🟡 MEDIUM PRIORITY — APP FEATURES

### Practice Modes
- [ ] Skip reveals answer — when user skips a card:
  - Show the correct answer on screen (unmask it)
  - Speak the word/phrase aloud in the target language
  - Brief 1.5 second pause so user can see and hear it
  - Then auto-advance to next card
  - Currently skip just moves on silently — user learns nothing from it
- [ ] AI-Powered Custom Dataset Builder — HIGH PRIORITY
  - User types a topic or theme (e.g. "travel", "fishing", "exercise")
  - App calls Claude/OpenAI API to generate a themed word set:
    - 20 words or phrases relevant to that topic
    - English word + French translation + Spanish translation
    - Word type (noun / verb / adjective / phrase)
    - Verb conjugations auto-generated (present / past / future)
    - Example sentence in each language (optional, premium tier)
  - Generated set is instantly playable AND saveable to user's library
  - User can regenerate if they don't like the set
  - User can edit individual words before saving

  EXAMPLE TOPICS TO PRE-BUILD AS STARTER SETS:
  - ✈️ Travel & Tourism (airports, hotels, sightseeing)
  - 🎣 Fishing (tackle, techniques, fish names, weather)
  - 🏋️ Exercise & Fitness (gym equipment, body parts, workout phrases)
  - 🍳 Cooking & Kitchen (ingredients, techniques, equipment)
  - 🏥 Health & Medical (symptoms, body parts, pharmacy)
  - 🌿 Nature & Outdoors (weather, terrain, wildlife)
  - 💼 Business & Work (meetings, emails, professional phrases)
  - 🏠 Home & Family (rooms, furniture, daily routines)
  - 🎵 Music & Arts (instruments, genres, performance)
  - ⚽ Sports (team sports, scoring, equipment)

  ACCESS MODEL:
  - Internal use only (proprietory) — generate sets for the built-in library
  - Free tier — browse and use pre-generated topic sets (read only)
  - Basic $1/mo — generate up to 3 custom topic sets per month
  - Premium $5/mo — unlimited topic set generation
  - One-time — $0.99 per generated set (no subscription needed)

  TECHNICAL APPROACH:
  - Claude API (claude-sonnet) called with structured prompt
  - Response formatted as JSON matching existing word set structure
  - Identical format to current wordSets array — drops straight in
  - Prompt engineering to ensure:
    - Accurate translations verified against dictionary sources
    - Appropriate difficulty level
    - Practical everyday vocabulary prioritised
    - Consistent formatting for tense conjugations
  - API cost: ~$0.002 per set generated (essentially free at scale)
  - Could also use this internally to expand the built-in set library

  FUTURE EXTENSIONS:
  - "Find me words from this text" — paste an article, extract vocabulary
  - "Words my class needs" — teacher pastes curriculum, app extracts vocab
  - "Words from this song" — paste lyrics, learn the vocabulary
  - Difficulty slider (beginner / intermediate / advanced vocabulary)
  - Generate sets in any language pair (not just EN↔FR/ES)

- [ ] Dual language speaker buttons on flash card
  - Currently: one 🔊 button speaks the prompt language only
  - Add a second button that speaks the OTHER language
  - Example in EN→FR mode: 🔊 speaks English prompt, 🇫🇷 speaks French answer
  - Example in FR→EN mode: 🔊 speaks French prompt, 🇬🇧 speaks English answer
  - Both buttons always visible on the card — tap either repeatedly
  - User can listen to both sides back and forth before answering
  - Reinforces the auditory pairing of the two languages simultaneously
  - Answer side button should be slightly muted/greyed until after answer
    is submitted (so it doesn't give away the answer before attempting)
  - Connects directly to the See → Hear → Vocalize loop and
    the dual-language audio prompt feature (Listen & Respond mode)
- [ ] Pronunciation repeat / mimicry mode — after answer is revealed:
  - If answer was wrong or skipped, show a 🔁 Repeat button
  - Tapping it speaks the correct word/phrase again at slow speed (rate 0.7)
  - User can tap as many times as needed to hear and mimic it
  - Add a "Try Again" mic button so user can attempt the pronunciation
    without it counting against their score
  - Goal: hear it → mimic it → hear it again → mimic again until confident
  - Connects directly to the See → Hear → Vocalize learning loop
  - Foundation for the SoundSteps phoneme analysis feature later
- [ ] Speed Flash mode
  - 3 different words shown simultaneously
  - 5 second countdown timer
  - User must say all three
  - Becomes mental math drill when math module added
- [ ] Verb tense sequence
  - Show infinitive form
  - User must say present tense → then past → then future in sequence
  - Score each individually
  - Don't skip to next word until all three tenses attempted
- [ ] Logo dropdown menu
  - Tap ParleBien logo → small menu drops down
  - Contains: dark/light mode toggle, language settings, about, feedback
  - Back to main page option

### Offline Downloadable Version — HIGH COST TIER
- [ ] Offline downloadable app package — HIGH PRIORITY REVENUE ITEM
  - A fully self-contained version of ParleBien that runs without internet
  - All word sets, all languages, all features bundled into one download
  - Works on PC (Windows/Mac), tablet, and phone without a browser connection
  - Critical for travellers, students in low-connectivity areas, schools

  PRICING & ACCESS MODEL:
  - One-time purchase: $49–99 (TBD based on market research)
  - Annual licence renewal: $19/year for updates and new word sets
  - Institutional site licence (schools, language schools): $299–499/year
  - No subscription — one payment, permanent offline access to that version
  - New word sets and languages released as paid update packs

  STRICT LEGAL PROTECTIONS REQUIRED — build these before release:
  - [ ] End User Licence Agreement (EULA) displayed and accepted at install
        - Single user licence — not transferable
        - No redistribution, sharing, or resale of the downloaded file
        - No reverse engineering or extraction of word sets
        - No commercial use without separate commercial licence
        - Licence revoked if terms violated
  - [ ] Copyright notice embedded in every file and visible in the app UI
        - "© ParleBien [year]. All rights reserved."
        - "This software and its content are protected by copyright law."
        - "Unauthorised copying, distribution or modification is prohibited."
  - [ ] Licence key system — unique key per purchase, required to activate
        - Prevents sharing of downloaded file between users
        - Keys tied to email address at purchase
        - Maximum 2 device activations per licence
  - [ ] Watermarking — user's email/licence ID embedded invisibly in data
        - If content is extracted and shared, can be traced back to source
  - [ ] Terms displayed on every app open (brief, dismissable after reading)

  TECHNICAL APPROACH:
  - Package as Electron app (Windows/Mac desktop) — wraps the HTML/JS
  - Package as PWA (Progressive Web App) for offline mobile use
  - Or Capacitor wrapper for Android/iOS (already planned for mobile app)
  - Word sets encrypted at rest — not readable as plain text if extracted
  - Licence validation checks against server on first launch and monthly

  DISTRIBUTION:
  - Direct download from parlebien.com (Stripe payment → download link)
  - Do NOT distribute via App Store initially — 30% fee and less control
  - App Store as secondary channel once established

  CONTENT INCLUDED IN OFFLINE VERSION:
  - All 6 pre-built French and Spanish word sets
  - All 2,178 master word list entries
  - All future Italian and German sets when released
  - All practice modes (EN→FR, FR→EN, Tenses, Speed Flash, etc.)
  - Does NOT include AI dataset builder (requires internet by nature)
  - Does NOT include cloud sync or cross-device features

  IMPORTANT NOTES:
  - Consult IP/software licence lawyer before release
  - Trademark ParleBien before releasing offline version (higher visibility)
  - COPPA compliance required if any children's content included
  - Consider separate LinguaKids offline version at lower price point ($29)
  - Physical flashcard ordering still requires internet (by design)

### Additional Languages — MEDIUM PRIORITY
- [ ] Italian 🇮🇹
  - Add Italian vocab database matching French/Spanish structure
  - 6 pre-built word sets (Survival, Café, Travel, Numbers, People, Verbs)
  - langConfig entry: speechCode 'it-IT', articles regex, theme colour
  - Suggested accent colour: green (#009246) matching Italian flag
  - Add 🇮🇹 Italian button to language toggle in header
  - Speech recognition: Web Speech API supports it-IT natively
- [ ] German 🇩🇪
  - Add German vocab database — note: German nouns have grammatical gender
    (der/die/das) which should be included with each noun
  - 6 pre-built word sets matching other languages
  - langConfig entry: speechCode 'de-DE', articles regex, theme colour
  - Suggested accent colour: gold (#FFCE00) matching German flag
  - Add 🇩🇪 German button to language toggle in header
  - Speech recognition: Web Speech API supports de-DE natively
  - Special consideration: German compound words and umlauts (ä/ö/ü)
    need fuzzy match tuning
  - Note: header language toggle will need redesign when 4 languages
    are present — consider a dropdown selector instead of inline buttons
  - Language selector redesign plan (do when Italian or German added):
    - Remove inline FR/ES toggle buttons from header
    - Landing page: prominent language selector as primary entry point
      "What would you like to learn?" → flag grid → Start Practicing
    - Logo dropdown menu: "Switch Language" option for mid-session changes
    - Header stays clean — just logo and score badge
    - Settings page: language preference saved as default

### Content & Import
- [ ] CSV file upload (drag and drop or file picker)
- [ ] CSV template download button (pre-formatted, ready to fill in Excel)
- [ ] CSV format: english, translation, type, present, past, future
- [ ] Additional pre-built sets (future):
  - Body & Health (connects to SoundSteps)
  - Classroom & School (bridges to LinguaKids)
  - Colours & Shapes (young children)
  - Animals (young children)

### Navigation & UX
- [ ] Dark mode / light mode toggle
  - Light mode palette: bg #f8f4ed, surface #ffffff, card #f0ebe0, text #1a1a24
  - Same CSS variable swap approach as Spanish/French theming
  - Saved to localStorage
- [ ] Combined Help + Feedback + Bug Report panel — HIGH PRIORITY
  - Accessible from logo dropdown AND floating "?" button on practice screen
  - Three tabs in one bottom sheet:
    - ❓ Help / FAQ — mic usage, how to import words, mode explanations, tips
    - 💬 Feedback — star rating + open text, submits to Google Form or email
    - 🐛 Report a Bug — structured: what happened / device / does it repeat
  - All three in one panel keeps interface clean
- [ ] "Coming Soon: LinguaKids" badge somewhere visible in app

---

## 🟢 FUTURE PRODUCTS

### LinguaKids (Children's Vocabulary)
- [ ] Full UI redesign — bright, large text, playful
- [ ] Age group selector (3–5, 6–8, 9–12, Teen)
- [ ] Age-appropriate word sets per group
- [ ] Image cards (essential for ages 3–5, no reading required)
- [ ] Enthusiastic voice feedback (stars, animations, encouraging sounds)
- [ ] Age-normed scoring against developmental milestones
  - Phoneme acquisition timeline encoded (what sounds are normal at each age)
  - Vocabulary size milestones by age
  - Percentile-style progress display for parents
- [ ] Child profile with birth date (precise age = better scoring)
- [ ] Multiple child profiles under one parent account
- [ ] Parent dashboard — weekly progress summary per child
- [ ] Printable progress certificates

### World Explorer (Family Travel)
- [ ] Destination-based vocabulary packs
- [ ] Airport, restaurant, hotel, emergency phrase sets
- [ ] Trip countdown timer ("12 days until your trip")
- [ ] Cultural context cards (currency, customs, food)
- [ ] Offline mode (critical for international travel)
- [ ] Pricing: $2.99/destination pack or $9.99/year unlimited
- [ ] Partnership angle: airlines, travel agencies, booking platforms

### SoundSteps (Speech Pathology Practice)
- [ ] Azure Pronunciation Assessment API integration
  - Phoneme-by-phoneme scoring
  - Fluency, accuracy, completeness, prosody scores
  - Already trained on child speech
  - Cost: ~$1/hour of audio
- [ ] SLP professional account type
  - Manages multiple child profiles
  - Uploads custom target word lists
  - Views session-by-session progress data
  - Exports PDF reports for clinical notes
- [ ] Phoneme-specific exercise sequences
- [ ] Age-normed phoneme milestone comparison
- [ ] "Share with therapist" weekly summary button
- [ ] Pricing: Free for families, $29/month SLP professional accounts
- [ ] IMPORTANT: Position as practice tool NOT clinical diagnosis
  - Never claim to diagnose speech disorders
  - Always suggest consulting a licensed SLP for concerns

### Math & Science Modules
- [ ] MathVoice — verbal math practice
  - Times tables (show equation, say answer)
  - Math vocabulary definitions
  - Mental arithmetic (timed)
  - Formula recall
  - Numeric fuzzy matching improvement (fifty-six = 56)
  - MathJax library for equation rendering
- [ ] ScienceSpeak — science vocabulary
  - Element symbols ↔ names
  - Taxonomy levels
  - Definitions and terms
  - Human body parts (image cards)
  - Lab safety vocabulary
  - Multi-part answer support ("name the three states of matter")

### Homeschool Features
- [ ] Multiple child profiles under parent account
- [ ] Lesson plan sequencer (order sets by week)
- [ ] Co-op sharing (group leader shares set link with multiple families)
- [ ] Offline mode
- [ ] Curriculum alignment tags (without using branded names)
- [ ] Progress reports exportable as PDF
- [ ] Homeschool co-op go-to-market strategy
  - Target co-op leaders as distribution channel
  - Homeschool curriculum fair presence

---

## 💼 BUSINESS & INFRASTRUCTURE

### Payments & Backend
- [ ] Stripe integration (payments for tiers + one-time orders)
- [ ] Supabase backend (user accounts + cloud word storage)
  - Words follow users across devices
  - Free tier: up to 50,000 users
- [ ] Tier system activation (currently hardcoded to 'free')
  - Free: 50 imported words
  - Basic $1/month: 150 words + PDF export
  - Premium $5/month: Unlimited + print discount

### Analytics & Tracking
- [ ] Google Analytics 4 (needs GA4 Measurement ID from user)
  - Track: session starts, set selections, completions, order clicks
- [ ] Hotjar (user screen recordings — free tier sufficient early on)
- [ ] Email capture for LinguaKids waitlist

### Development Tools
- [ ] Evaluate Claude Code for GitHub integration — NEAR TERM
  - Claude Code is a command-line tool that connects Claude directly to your file system and Git
  - Would allow Claude to commit and push file changes to GitHub directly
  - Eliminates the manual download → paste → commit workflow
  - Check: claude.ai → Claude Code (desktop/CLI tool)
  - Best evaluated when moving to Cowork for LinguaKids build
- [ ] Check claude.ai/settings periodically for GitHub MCP connector
  - When available, will allow direct repo updates from chat interface
  - No installation required — one-click connect like other MCP connectors

### Legal & Brand

#### Patent Assessment & Strategy — HIGH PRIORITY
- [ ] Conduct patent landscape assessment before any public fundraising
  - Assess whether core innovations are patentable:
    - Voice-first active recall learning loop (hear → process → speak → evaluate)
    - Fuzzy phonetic matching for spoken language answer evaluation
    - AI-powered custom vocabulary set generation from topic prompts
    - Age-normed developmental scoring for children's speech/vocabulary
    - Combined verbal + visual + auditory triple-channel flashcard system
    - SLP-integrated home practice with phoneme-level AI scoring
  - Search existing patents: USPTO (patents.google.com is easiest interface)
  - Key question: is the METHOD patentable, even if the technology is not new?
    (Software patents cover novel APPLICATION of technology, not technology itself)
  - Recommended: provisional patent application first (~$320 USPTO fee)
    - Gives 12 months of "patent pending" status while you validate the business
    - Low cost, buys time, establishes priority date
    - Full patent application can follow once funded
- [ ] Build patent proposal document (separate deliverable)
  - Describe the invention in plain language
  - Identify claims — what specifically is novel and non-obvious
  - Prior art search — what exists already
  - Recommended: use a patent attorney for final filing
    (provisional can be drafted without attorney, non-provisional should not be)
  - Budget: $320 provisional (self-filed) + $3,000–8,000 non-provisional (attorney)
- [ ] Trade secret assessment
  - Even without a patent, some elements may be better protected as trade secrets
  - The specific fuzzy matching algorithm parameters
  - The AI prompt engineering for dataset generation
  - The age-normed scoring thresholds
  - Trade secrets have no filing cost but require internal confidentiality practices

#### EULA & Legal Pages for Live Site — HIGH PRIORITY
- [ ] Terms of Service page at parlebien.com/terms
  - Acceptable use policy
  - Intellectual property ownership statement
  - Limitation of liability
  - Governing law and jurisdiction
  - Account termination conditions
- [ ] Privacy Policy page at parlebien.com/privacy
  - What data is collected (analytics, account info, word sets)
  - How it is used and stored
  - Third party services (Google Analytics, Stripe, Supabase)
  - GDPR compliance statement (if serving EU users)
  - COPPA compliance statement (required for children's features)
  - Cookie policy
- [ ] Simple site-wide EULA banner / notice
  - Brief notice on first visit: "By using ParleBien you agree to our Terms"
  - Links to full Terms and Privacy Policy
  - Cookie consent banner (required for GDPR / EU users)
  - One-line copyright notice in footer: "© 2025 ParleBien. All rights reserved."
- [ ] Copyright notice embedded in app footer and HTML source
  - Already in HTML comment block — needs to also appear in visible UI
  - Add subtle copyright line to landing page footer
- [ ] COPPA compliance plan
  - Required for any features targeting children under 13 in the US
  - Parental consent mechanism for LinguaKids
  - Data minimisation for children's accounts

#### Account Login & Authentication — FUTURE (Supabase Stage)
- [ ] User account system — full spec:
  - Email + password registration and login
  - OAuth options: Google Sign-In, Apple Sign-In (required for iOS App Store)
  - Email verification on registration
  - Password reset flow
  - Account deletion (required by GDPR and App Store policies)
  - Session management (remember me, logout all devices)
  - Account tiers stored server-side (Free / Basic / Premium)
  - Word sets synced to account — available on any device
  - Multiple child profiles under one parent account (LinguaKids)
  - SLP professional account type with patient management
- [ ] Authentication provider: Supabase Auth (already planned — handles all above)
  - Free tier covers up to 50,000 monthly active users
  - Built-in OAuth, email verification, session management
  - No separate auth service needed

#### Trademark & Brand Protection
- [ ] Trademark search for "ParleBien" in language learning category
  - USPTO search (US): patents.google.com / USPTO TESS
  - Check EU trademark database (EUIPO) if targeting European market
- [ ] File trademark application when revenue begins
  - Class 41 (Education and Training services)
  - Class 9 (Software and apps)
  - Cost: ~$250–350 per class per jurisdiction
- [ ] Consider umbrella platform name as products expand
  - Suggested: VoiceLearn (ParleBien, LinguaKids, SoundSteps as modules)
  - Trademark umbrella name AND individual product names

### Copyright Notes
- [ ] Vocabulary words: SAFE — individual words not copyrightable
- [ ] Common phrases: SAFE — common language
- [ ] Never use "Coffee Break French" or similar brand names as feature labels
- [ ] Images added later: use Unsplash, Pexels, or commission originals
- [ ] Scientific claims: keep accurate, cite general research

### Print Partner
- [ ] Evaluate Gelato (recommended — global print network, API, no minimum)
- [ ] Evaluate Printful (alternative)
- [ ] Set up print API integration when order feature is ready

---

## 🏗️ ARCHITECTURE NOTES
*For CTO reference and future hires*

**Current stack:**
- Single HTML file (~1,300 lines), vanilla JS, no framework
- Web Speech API (SpeechRecognition + SpeechSynthesis)
- CSS custom properties for theming (language + dark/light mode ready)
- localStorage for word persistence
- GitHub Pages hosting (static, free)
- No backend, no database, no accounts yet

**When to move to Cowork:**
- When building LinguaKids (multi-file project, image assets needed)
- When adding Supabase backend
- Trigger: moving from one product to a platform

**Scaling path:**
- Phase 1: Static HTML on GitHub Pages ← current
- Phase 2: Add Supabase (auth + database) + Stripe (payments)
- Phase 3: Separate React app, API layer, admin dashboard
- Phase 4: Native mobile apps (wrap with Capacitor for Android/iOS)

**Key architectural decisions already made:**
- CSS variables for theming = easy dark mode + language switching
- Tier system in JS = swap one variable when Stripe is connected
- wordSets data structure = extensible to any subject
- fuzzy matching = language-agnostic, works for math answers too

---

## 📋 SESSION NOTES
*Add notes here when picking up in a new session*

- Session 1: Built core app, deployed to parlebien.com, added 12 word sets
- Session 1 cont: Fixed 4 bugs (mic permission, no text fallback, sets blank space, locked button)
- Session 1 cont: Built investor proposal, competitive positioning document
- Session 1 cont: Added bug tracker (PARLEBIEN_BUG_TRACKER.md)
- Next session: Landing page OR CTO proposal OR Speed Flash / Listen & Respond features
- User has: GitHub account (Luxtronic-Paul), GoDaddy (parlebien.com), Pixel 9 Pro
- User context: Learning French, exploring building this as a product
- Development path: Continue in Claude.ai chat until LinguaKids → then move to Cowork
- GitHub repo files: index.html, PARLEBIEN_TODOLIST.md, PARLEBIEN_BUG_TRACKER.md, PARLEBIEN_INVESTOR_PROPOSAL.md

### ⚠️ Cowork Migration Triggers — Watch For These
Move ParleBien development to Claude Cowork when ANY of these are true:
- [ ] Starting LinguaKids build (multi-file project, image assets needed)
- [ ] Adding Supabase backend (config files, environment variables, multiple JS modules)
- [ ] Adding Stripe integration (server-side code, webhook handlers)
- [ ] index.html exceeds ~1,500 lines and edits become risky
- [ ] Need to run live local server to test changes before pushing to GitHub
- [ ] Hiring a CTO or contractor who needs to work in the same codebase
- [ ] Building the Android app wrapper (Capacitor — requires Node.js project structure)
Current line count: ~1,345 lines — getting close, monitor each session

