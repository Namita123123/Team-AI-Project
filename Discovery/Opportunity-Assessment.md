# Opportunity Assessment — Perspective Radar
**Document Type:** Opportunity Assessment (OpA)  
**Project:** Multi-Perspective News Aggregator  
**Status:** Draft  
**Last Updated:** 2026-08-14  
**Based on:** User interviews with Animesh Jain and Jyotish Sonowal + prototype feedback session

---

## 1. Opportunity

### The Unmet Need

News consumers today are aware that media is biased, but lack a fast, effortless way to get multiple perspectives on the same story. The current experience forces users to manually seek out alternative sources — a behaviour that most people start, then abandon because it takes too much time and cognitive effort.

> *"I like to collect a lot of data and then make an informed choice — but that takes time."* — Animesh  
> *"I have done that in the past but I felt it was just consuming too much time and energy."* — Jyotish

Both users are intelligent, motivated news consumers who have independently concluded that mainstream media cannot be trusted as a single source. Yet neither has found a satisfying tool that solves this for them at scale.

### Why Now

- Mainstream media trust is declining; both users have moved to independent, international, and community sources (Reddit, Al Jazeera, YouTube independents)
- Algorithm-driven platforms (Google News, YouTube, Instagram) are reinforcing filter bubbles, not breaking them
- Short-form content (Instagram Reels, YouTube Shorts, InShorts) has shifted news consumption behaviour to mobile, bite-sized formats
- AI tools now make it possible to search, retrieve, and synthesise multiple news sources in seconds — work that previously took users 20–30 minutes

---

## 2. Problem Statement

**For people who actively follow current events**, the problem is that **getting a balanced, multi-perspective view of a news story requires manual effort across multiple platforms** — effort so high that most users either skip it entirely or fall back into a single-source bias they know is incomplete.

This results in:
- Uninformed or one-sided opinions on important topics
- Filter bubbles reinforced by algorithm-driven platforms
- Growing distrust in news with no practical alternative
- Users feeling they "should" cross-reference but lacking the time or tools to do so

---

## 3. Target Users

### Primary Persona — The Informed Skeptic
A digitally-native professional in their 25–35 age range who follows current events regularly but does not trust mainstream media. They actively seek independent sources, cross-reference manually when they have time, and worry about their own filter bubble. They consume news primarily on mobile, in under 30 minutes a day.

**Representative users from research:** Animesh (tech professional, active cross-referencer), Jyotish (geopolitics and tech follower, former deep-diver who scaled back due to information fatigue)

### Secondary Persona — The Casual Informer
A professional who wants to stay generally informed but does not have the appetite for deep dives. They scan headlines on Google News or Instagram, rely on friends and Reddit for perspective, and would benefit from a low-effort way to get balanced context without committing significant time.

---

## 4. Proposed Solution

**Perspective Radar** — a mobile-first news experience that automatically surfaces multiple perspectives on the same story, presented as brief bullet-point summaries with source labels, allowing users to stay informed with balance in under 30 minutes a day.

### Core Capabilities (MVP)
1. **Topic-based feed** — personalised by user-selected interests (tech, geopolitics, business, etc.) with a separate "Trending now" section for globally significant stories
2. **Multi-perspective summary cards** — each story shows 2–4 bullet-point perspectives from different sources/viewpoints, with source labels visible
3. **Progressive disclosure** — headline → 3-line summary → full article link; source detail is hidden by default and expandable
4. **Timestamp on every article** — recency is a critical trust signal for users
5. **Visual hierarchy** — a hero story per topic category with supporting smaller cards; thumbnail images alongside each card

---

## 5. Risk Factors

### Value Risk — Does this solve a problem users will pay attention to?
**Score: 4/5 — High confidence**

Both interviewees validated the core problem strongly. Animesh explicitly described a wish for a "Rotten Tomatoes for news." Jyotish confirmed his YouTube and Google feeds are "completely optimised for supporting my worldview" and he wants something to challenge that. The prototype received positive initial reactions on concept (card layout, source attribution, topic following).

### Usability Risk — Can users understand and use this comfortably?
**Score: 3/5 — Medium confidence**

The prototype session revealed significant usability concerns: navigation was confusing, the desktop layout felt intimidating to mobile-first users, flat card hierarchies gave users no visual anchor, and information overload from upfront source detail caused fatigue. These are real design challenges that need to be solved before launch.

### Feasibility Risk — Can we build this with available tools?
**Score: 4/5 — High confidence**

Bob's Tavily MCP integration enables real-time multi-source web search and content extraction. AI summarisation of multiple articles into perspective-labelled bullet points is achievable. Mobile-first implementation is standard. Main risks are paywall restrictions on certain premium sources and the quality/consistency of AI-generated perspective labelling.

### Viability Risk — Is there a sustainable path to value?
**Score: 3/5 — Medium confidence**

The problem is real and validated, but the market is competitive (Google News, AllSides, Flipboard, Ground News). Differentiation must come from the quality of AI-driven perspective synthesis, the mobile-first UX, and the bias-challenge feature. Viability of a standalone product vs. an embedded feature needs further exploration.

---

## 6. Key Assumptions

- Users are willing to try a new news app if it demonstrably saves them time while improving perspective breadth
- AI-generated perspective summaries will be accurate and fair enough to build user trust
- Tavily-sourced articles will have sufficient variety to represent genuinely different viewpoints
- Mobile-first design will significantly improve adoption vs. the desktop prototype
- Source credibility labelling can be done at a basic level without requiring a proprietary credibility database

---

## 7. Key Questions Still Open

1. What is the monetisation model? (Free with ads? Subscription? Freemium?)
2. How do we handle topics where only one narrative exists in coverage?
3. How do we define and measure "balanced" perspectives programmatically?
4. Do we need user account creation / preference persistence for personalisation, or can we start stateless?
5. What is the minimum number of perspectives that constitutes a "complete" view?

---

## 8. Success Criteria

The opportunity is worth pursuing if:
- Users can get a balanced view of a story in under 5 minutes
- Users feel their filter bubble is being actively challenged (qualitative)
- At least 3 distinct perspectives can be reliably surfaced per story
- Mobile experience scores higher on usability than the initial prototype
- Users return daily or multiple times per week (habit formation)

---

## 9. Recommendation

**Proceed to solution design.** The opportunity is validated by user research. Both core pain points (time cost of cross-referencing, distrust of single sources) are strong and consistent across interviewees. The prototype has provided clear design direction. The feasibility risks are manageable with the Tavily + AI stack available.

**Immediate next steps:**
- Define detailed persona and user journey (see [`Discovery/Persona-and-User-Journey.md`](./Persona-and-User-Journey.md))
- Redesign prototype with mobile-first, summary-first, progressive disclosure principles
- Define the technical architecture for perspective retrieval and summarisation

---

## References
- [Interview Insights Synthesis](./User%20Interviews/Interview-Insights-Synthesis.md)
- [Multi-Perspective News Aggregator Discovery Doc](./Multi-Perspective-News-Aggregator.md)
- [Diya Namita Transcript](./Diya%20Namita%20transcript.md)
