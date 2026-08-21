# Persona & User Journey — Perspective Radar
**Document Type:** UX Design Artifact  
**Project:** Multi-Perspective News Aggregator  
**Status:** Draft  
**Last Updated:** 2026-08-14  
**Based on:** User interviews with Animesh Jain and Jyotish Sonowal + prototype feedback session

---

## Persona 1 — The Informed Skeptic

> *"I like to collect a lot of data and then make an informed choice. I definitely have trust issues with our media."*

### Profile

| Attribute | Detail |
|---|---|
| **Name** | Aryan |
| **Age** | 28 |
| **Role** | Tech professional |
| **Primary device** | Mobile (phone first, laptop for deep dives) |
| **News time budget** | 30–45 minutes/day, spread across commute and breaks |
| **Current sources** | Independent YouTube channels, Al Jazeera, Instagram reels, occasional Google News |

### Goals
- Form his own well-rounded opinion without being fed a narrative
- Stay on top of tech, AI, geopolitics, and major world events
- Spend limited time but come away feeling genuinely informed — not just updated
- Find out about major breaking stories even outside his chosen topics

### Frustrations
- Mainstream Indian news channels are polarised and under political influence
- Google News aggregates from unknown sources with no visible credibility logic
- Cross-referencing multiple sources manually takes too long — he does it, but it's effortful
- Wants a "Rotten Tomatoes for news" — a credibility/quality rating for each story
- The prototype felt too plain (no images, no timestamps, navigation was confusing)

### Behaviours
- Actively follows 3–4 trusted independent channels/creators
- Cross-references Al Jazeera and other international sources when he wants a global view
- Watches YouTube Shorts / Al Jazeera shorts for bite-sized coverage of ongoing stories
- Would pay attention to ongoing story threads (e.g. a 30-day protest) if the tool maintained a timeline

### Quote
> *"You can only form your own opinion when you have multiple cross-references from credible sources. I want to be told the facts — not the narrative."*

---

## Persona 2 — The Casual Informer

> *"I don't want to spend too much time. I want to limit it to half an hour and get a good all-round view."*

### Profile

| Attribute | Detail |
|---|---|
| **Name** | Kiran |
| **Age** | 32 |
| **Role** | Business/operations professional |
| **Primary device** | Mobile and TV (watches YouTube on TV for deep dives) |
| **News time budget** | Max 30 minutes/day |
| **Current sources** | Google News (India), Reddit (global + stock market), Instagram (headlines) |

### Goals
- Stay generally informed without going deep on every story
- Get a headline + enough context to join a conversation with colleagues
- Avoid sensationalised, clickbait-driven news
- Have her filter bubble challenged — she knows algorithms are reinforcing her worldview

### Frustrations
- Google News and YouTube are now "completely optimised for supporting my worldview"
- Too much information upfront causes fatigue — she stopped doing deep cross-referencing because of this
- The prototype had no visual hierarchy; everything looked the same — no clear entry point
- Desktop layouts feel unfamiliar and overwhelming; she exclusively reads news on mobile now
- Sensationalised news articles are everywhere; she prefers no-drama, short-paragraph Reddit-style content

### Behaviours
- Scans headlines; deep dives only on topics she cares about (geopolitics, economics, tech)
- Uses Reddit for Bollywood news and stock market — values the no-drama community writing style
- Would use a bias-challenge mode if it surfaced the "other side" she would never find organically
- Doesn't track ongoing stories — consumes news episodically
- Relies on friends and colleagues to get different perspectives in conversation

### Quote
> *"I've really limited myself. If something can give me high-level bullet points and a good all-round view in 30 minutes — that would really add value."*

---

## User Journey — Perspective Radar (Mobile App)

### Journey Overview

```
Discover → Open → Scan → Read → Deep Dive (optional) → Return
```

---

### Stage 1: Discover / First Use

**Touchpoint:** Word of mouth, social media recommendation, or app store  
**User need:** Understand why this is different from Google News  
**Action:** Downloads app, sees onboarding

**Experience:**
- Onboarding asks user to pick 3–5 interest topics (tech, geopolitics, business, sport, etc.)
- Clear value prop shown: *"Multiple perspectives, one place. No algorithm bias."*
- App immediately shows a feed tailored to chosen topics

**Pain points to avoid:**
- Don't overwhelm with too many topic choices on first screen
- Don't ask for account creation before showing value

**Design principle:** Show value before asking for commitment

---

### Stage 2: Daily Open (Habitual Use)

**Touchpoint:** Phone, morning routine or commute  
**User need:** Quick scan — what happened today?  
**Action:** Opens app, sees personalised feed

**Experience:**
- Feed opens to **"Today" view** — hero story at the top (large card with image + 2-line summary)
- Below: smaller story cards for each topic category
- Separate **"Trending"** section surfaces globally significant stories outside chosen topics
- Each card shows: headline, thumbnail image, **timestamp**, topic tag

**Pain points to avoid:**
- No flat equal-weight card grids — visual hierarchy is essential
- No deep source detail on the surface — keep it clean and scannable
- No desktop-style dense layouts — mobile first, always

**Design principle:** Hero → secondary → trending. One clear visual anchor per screen.

---

### Stage 3: Scan a Story Card

**Touchpoint:** Story card in feed  
**User need:** Understand the story in 10 seconds  
**Action:** Reads headline + inline summary

**Experience:**
- Tapping a card expands it **in-place** to reveal 3–5 bullet-point perspectives
- Each perspective is 1–2 sentences with a source label (e.g. "BBC", "Al Jazeera", "Reddit r/worldnews")
- Source credibility/lean indicator is visible as a small tag (e.g. "International", "Independent", "Mainstream India")
- Timestamp visible on every perspective

**Pain points to avoid:**
- Don't force user into a new screen to see perspective summary
- Don't surface source analysis upfront — keep it one tap away
- Don't truncate perspectives so aggressively that they lose meaning

**Design principle:** Summary-first. Depth on demand. Never force a full-page load to get context.

---

### Stage 4: Deep Dive (Optional)

**Touchpoint:** Expanded story card  
**User need:** I want to understand this story fully  
**Action:** Taps "Read full article" or "See all sources"

**Experience:**
- "Read full article" opens the original source article (external browser or in-app reader)
- "See all sources" expands to show all retrieved articles with source names, publication dates, and brief extracts
- "Story timeline" button (for ongoing stories) opens a chronological thread of updates from inception to now

**Pain points to avoid:**
- Don't make the deep-dive path the default — it's a power-user action
- Don't lose the user's place in the feed when they return from an article

**Design principle:** Progressive disclosure. Surface → Summary → Sources → Full article. Each step is a conscious opt-in.

---

### Stage 5: Bias Challenge (Power Feature)

**Touchpoint:** Story card or user settings  
**User need:** I want to see a perspective I wouldn't naturally encounter  
**Action:** Taps "Challenge my view" or has it enabled as a daily push

**Experience:**
- Once per session (or daily notification), one story card is highlighted: *"This might challenge your usual view"*
- The highlighted perspective comes from a source with a known lean opposite to the user's typical consumption
- User can dismiss, read, or react with a thumbs up/down

**Pain points to avoid:**
- Don't push this aggressively — it should feel like an invitation, not a confrontation
- Don't use political labels (left/right) — use neutral descriptors (regional, international, community)

**Design principle:** Gentle friction. Challenge without alienating.

---

### Stage 6: Return / Habit Formation

**Touchpoint:** Daily notification or organic return  
**User need:** Stay current without spending too much time  
**Action:** Returns to app same time next day

**Experience:**
- Daily digest notification: *"5 stories you should know about today"*
- App remembers topic preferences and continues learning what the user deep-dives on
- Streak or "informed days" counter (optional) to encourage habit

---

## Edge Cases

| Scenario | How to Handle |
|---|---|
| Only one perspective exists on a story | Show what's available; label: *"Limited perspectives found — only one narrative in current coverage"* |
| Breaking news — sources still developing | Timestamp prominently; label card as *"Developing story"* |
| Paywalled articles | Show summary only; label source as *"Subscription required for full article"* |
| Highly sensitive or disputed topics | Add a neutral framing note; avoid bias labels on politically charged issues |
| User has no internet (offline) | Show cached feed from last session with *"Last updated [time]"* indicator |
| Topic with no news today | Show *"Nothing new in [Topic] today"* rather than empty state |

---

## References
- [Opportunity Assessment](./Opportunity-Assessment.md)
- [Interview Insights Synthesis](./User%20Interviews/Interview-Insights-Synthesis.md)
- [Multi-Perspective News Aggregator Discovery Doc](./Multi-Perspective-News-Aggregator.md)
