# User Interview Insights — Synthesis
**Project:** Multi-Perspective News Aggregator  
**Interviews:** Animesh Jain, Jyotish Sonowal  
**Date:** August 2026  
**Status:** Complete

---

## Key Themes

### 1. 📵 Deep Distrust of Mainstream Media
Both participants expressed low trust in traditional Indian news channels. They described mainstream media as "under influence," "polarised," and "selling a narrative." Both had independently shifted to independent, international, or community-based sources.

> *"These credible news sources are not really doing their job because they are under some influence."* — Animesh
> 
> *"I try not to follow Republic TV and all of that... I find it a waste of my time."* — Jyotish

**Implication:** A solution that labels or flags source bias/credibility would be highly valued.

---

### 2. 🔍 Cross-Referencing Is Manual and Time-Consuming
Both users acknowledged they cross-reference sources, but this behaviour is effortful and inconsistent. Animesh does it actively; Jyotish acknowledged doing it in the past but stopped because it consumed too much time.

> *"I like to collect a lot of data and then try to make an informed choice."* — Animesh
> 
> *"I have done that in the past, but I felt it was just consuming a lot of my time and energy."* — Jyotish

**Implication:** The core job-to-be-done is: **make cross-referencing effortless and fast.** A tool that does the heavy lifting for users is the unlock.

---

### 3. ⏱️ Time Is the Biggest Constraint
Both participants want to spend limited time on news — approximately 30 minutes a day. Long-form, deep-dive content exists but is saved for topics they deeply care about. For day-to-day news, they prefer quick bites.

> *"I want to limit it to say half an hour in a day."* — Jyotish
> 
> *"I used to really like the [InShorts] format — in a quick glance you can understand what's happening."* — Animesh

**Implication:** Any solution must default to a short, digestible format. Depth should be optional (progressive disclosure).

---

### 4. 🗞️ Source Transparency Matters
Both users wanted to know *where* news is coming from. Animesh expressed frustration with Google News's opaque algorithm. Jyotish noted he doesn't always register which outlet an article is from on Google News.

> *"I don't understand what the algorithm behind aggregating that news is — that visibility I don't think we all have."* — Animesh

**Implication:** Source labelling, outlet credibility scores, and transparent aggregation logic are important trust signals.

---

### 5. 🎯 Personalisation Has Limits — Major Events Are Universal
Both users want personalised topics, but also want to stay aware of major world events regardless of their interest category. Animesh follows tech, AI, politics, travel, education. Jyotish follows tech, geopolitics, economics/business.

> *"If it's a major event that's happening, I would like to know without being in a particular category of interest."* — Animesh

**Implication:** The tool should offer a two-tier view — **your topics** + **what the world is talking about right now.**

---

### 6. 💡 Novel Feature Requests from Users

**Animesh — "News Credibility Rating":**
> *"I wish I'd get some kind of rating like we have for movies — like Rotten Tomatoes rated by critics. I'd really like a news critic critiquing the news with an algorithm that tells us how credible this is. That would be a game changer."*

**Animesh — "Story Timeline / Thread:"**
> *"On an ongoing topic, do you have a thread maintained? For example, the protest happened for 30 days — it would be nice to know based on a timeline what's happening from inception till current."*

**Jyotish — "Bias Challenge Mode":**
> *"YouTube and Google are now completely optimised for supporting my worldview. I definitely need something that challenges that."*

---

## Pain Point Summary

| Pain Point | Animesh | Jyotish | Priority |
|---|---|---|---|
| Mainstream media is biased / untrustworthy | ✅ Strong | ✅ Strong | 🔴 High |
| Cross-referencing is too time-consuming | ✅ Does it manually | ✅ Stopped doing it | 🔴 High |
| News is too long / no short format | ✅ Wants InShorts-style | ✅ Max 30 min/day | 🔴 High |
| Lack of source transparency in aggregators | ✅ Google News opaque | ✅ Doesn't notice source | 🟡 Medium |
| Confirmation bias / filter bubble | ✅ Aware | ✅ Actively concerned | 🟡 Medium |
| No credibility/rating signal for news | ✅ Wishes for it | ✅ Implicit | 🟡 Medium |
| No story timeline for ongoing events | ✅ Explicitly requested | Not mentioned | 🟢 Nice to have |

---

## Validated Assumptions

✅ Users feel news media is biased and cannot be fully trusted  
✅ Users want balanced perspectives but lack the time to find them  
✅ Short-form + option to deep-dive is the preferred consumption pattern  
✅ Source credibility and transparency are important to users  
✅ Users want the tool to actively counteract their filter bubble  

---

## Invalidated / Uncertain Assumptions

⚠️ Users may not actively seek perspectives — Jyotish does this passively (relies on friends for perspective) rather than actively seeking alternate sources  
⚠️ Value for non-political topics is less clear — Jyotish sees political/global news as more multi-perspective; for tech news, he sees no right/wrong  

---

## Recommended MVP Features (Based on Interviews)

1. **Topic input** → enter a news topic or headline
2. **Multi-source perspective summary** → short summaries from 3+ sources across different viewpoints
3. **Source label + credibility indicator** → show where each perspective comes from
4. **Short-form default** → bite-sized summaries, with "read more" option
5. **Bias challenge mode** → show a perspective that contradicts the user's likely viewpoint

---

## Next Steps

- [ ] Validate MVP feature set with a third interview or prototype test
- [ ] Proceed to solution design and user journey mapping
- [ ] Define technical approach using Bob + Tavily MCP
