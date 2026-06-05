# ParleBien — Bug Tracker & Issue Log
*Upload to GitHub alongside index.html and PARLEBIEN_TODOLIST.md*
*Updated: Session 1 — Initial build*

---

## Bug Status Key
- 🔴 **OPEN** — Not yet fixed
- 🟡 **IN PROGRESS** — Being worked on
- 🟢 **FIXED** — Resolved and deployed
- ⚪ **WONT FIX** — Acknowledged, not a priority
- 🔵 **FEATURE REQUEST** — Reclassified as enhancement

---

## Fixed Bugs

---

### BUG-001 — Mic permission popup repeats every session
**Status:** 🟢 FIXED (Session 1)
**Reported by:** Developer testing
**Platform:** Desktop Chrome, Android Chrome
**Severity:** Medium
**Description:**
When opening the app as a local HTML file, Chrome treats it as an untrusted origin and does not save the "always allow" mic permission. Users had to re-allow the mic every time they opened the app.
**Root cause:**
Local file:// origin — Chrome does not persist permissions for local files.
**Fix applied:**
Deployed app to parlebien.com via GitHub Pages with HTTPS. Chrome now remembers mic permission permanently for the domain after one allow.
**Verified on:** Pixel 9 Pro (Chrome), Desktop Chrome

---

### BUG-002 — Mic button only — no fallback text input
**Status:** 🟢 FIXED (Session 1)
**Reported by:** Developer testing
**Platform:** All platforms
**Severity:** Medium
**Description:**
Original design had mic button as the only answer input. If mic was blocked or denied, user had no way to answer cards.
**Fix applied:**
Redesigned answer area — mic button and text input field now always visible side by side in a single combined input row. Spoken answer populates the text field; typed answer works identically. Either method activates the Check Answer button.

---

### BUG-003 — Sets view: blank space at top, content below fold
**Status:** 🟢 FIXED (Session 1)
**Reported by:** User — Pixel 9 Pro and laptop
**Platform:** Android Chrome, Desktop Chrome
**Severity:** Medium
**Description:**
When tapping the Sets tab, the top-center portion of the screen was blank and all set cards appeared below the visible area, requiring scrolling to find them.
**Root cause:**
Two issues combined:
1. `renderSets()` was building the All Words card last and prepending it to the grid after the fact, causing a render order issue
2. `.sets-view` CSS was competing with the practice view for flex space, pushing content down
**Fix applied:**
- All Words card now built first in correct DOM order
- Sets view CSS corrected — `flex:1` only applied when `.active` class present
- Cards now render immediately visible from top of screen

---

### BUG-004 — Selecting a set locks the Check Answer / mic button
**Status:** 🟢 FIXED (Session 1)
**Reported by:** User — Pixel 9 Pro and laptop
**Platform:** Android Chrome, Desktop Chrome
**Severity:** High — blocked core practice flow
**Description:**
After selecting a word set from the Sets tab, the set card showed a checkmark and "Active" badge correctly, but tapping "Practice This Set" (or equivalent) left the Check Answer button disabled/locked. The mic button was also unresponsive. The only workaround was navigating back to Sets, selecting "All Words", then re-entering practice.
**Root cause:**
`activateSet()` called `newSession()` then `showView('practice')` without fully resetting session state. If a session had just ended, `awaitingNext` remained `true`, which disabled the mic and submit button. The flash card also retained its previous correct/wrong highlight colour.
**Fix applied:**
`activateSet()` now performs a complete session state reset before loading new set:
- `awaitingNext` set to `false`
- Submit button text, handler and disabled state reset
- Mic button emoji and label reset
- Text input cleared
- Result banner hidden
- Flash card correct/wrong classes removed
- `buildSession()` and `loadCard()` called fresh

---

## Open Bugs

*None currently open*

---

## Known Limitations (Not Bugs)

---

### LIMIT-001 — Speech recognition requires Chrome or Edge
**Status:** ⚪ WONT FIX (by design)
**Platform:** Firefox, Safari
**Description:**
Web Speech API (SpeechRecognition) is not supported in Firefox or Safari. Users on these browsers see a warning and fall back to text input only. Voice output (text-to-speech) works in all browsers.
**Mitigation:**
Warning message displayed. Text input always available as fallback. App fully functional without voice input.
**Future consideration:**
When native Android/iOS apps are built (Capacitor wrapper), platform speech APIs will be used instead, resolving this for mobile users on any browser.

---

### LIMIT-002 — Imported words stored on device only
**Status:** ⚪ WONT FIX (current stage)
**Platform:** All
**Description:**
User-imported word sets are saved to browser localStorage. They do not sync across devices. A word set imported on a laptop will not appear on the user's phone.
**Mitigation:**
Users can re-import the same CSV on each device.
**Future fix:**
Supabase backend (planned for seed stage) will move word storage to cloud database, syncing across all devices per user account.

---

### LIMIT-003 — Word limit enforced per device not per account
**Status:** ⚪ WONT FIX (current stage)
**Platform:** All
**Description:**
The 50-word free tier limit is stored in localStorage per device. A user could bypass it by using a different browser or device.
**Mitigation:**
Acceptable at current pre-revenue stage. No real accounts exist yet.
**Future fix:**
Supabase + Stripe integration will enforce limits server-side per authenticated user account.

---

### LIMIT-004 — Tense mode only works for verbs with pre-loaded conjugations
**Status:** ⚪ WONT FIX (current stage)
**Platform:** All
**Description:**
Tense practice mode only shows verbs that have tense data in the word set. User-imported verbs without tense data (present/past/future fields) will not appear in Tense mode.
**Mitigation:**
Import format supports tense fields: `to run | courir | verb | je cours / j'ai couru / je courrai`
**Future fix:**
Consider AI-assisted conjugation — user imports a verb, app auto-generates conjugations via API.

---

## Pending Investigation

*Issues reported but not yet fully diagnosed*

---
*(none currently)*

---

## Feature Requests (Reclassified from Bug Reports)

| ID | Request | Status | Priority |
|---|---|---|---|
| FR-001 | In-app bug reporting button | 🔵 Feature Request | High |
| FR-002 | Help / FAQ section in app | 🔵 Feature Request | High |
| FR-003 | Combined Help + Feedback panel | 🔵 Feature Request | High |

*See PARLEBIEN_TODOLIST.md for full feature backlog*

---

## How to Report a Bug
*(For future in-app reporting — currently manual)*

When reporting a bug please include:
1. **What you were doing** — which screen, which mode, what action
2. **What you expected** to happen
3. **What actually happened**
4. **Your device and browser** — e.g. Pixel 9 Pro, Chrome / MacBook, Safari
5. **Does it happen every time** or only sometimes?

---

## Bug Severity Definitions

| Level | Definition | Example |
|---|---|---|
| **Critical** | App unusable, data loss | App crashes on open |
| **High** | Core feature blocked | Can't submit an answer |
| **Medium** | Feature impaired but workaround exists | Mic needs re-allowing each session |
| **Low** | Minor visual or cosmetic issue | Badge misaligned on small screen |
| **Cosmetic** | No functional impact | Colour slightly off in dark mode |

---
*Last updated: Session 1 | Next review: After next build session*
