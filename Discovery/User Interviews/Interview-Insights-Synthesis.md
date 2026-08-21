# User Interview Insights — Synthesis
**Project:** Multi-Perspective News Aggregator  
**Interviews:** Animesh Jain, Jyotish Sonowal
**Date:** August 2026
**Status:** Updated — prototype feedback added

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

---

## 🖥️ Prototype Feedback (Missed in First Pass)

Both participants were shown an early prototype called **"Perspective Radar"** during the interview. This section captures their direct reactions.

---

### Animesh — Prototype Feedback

**What he liked:**
- The card layout showing headlines was clear: *"This looks nice. It gives me the heading."*
- Source attribution visible on the right side: *"Where is it sourcing the news from? That is also listed."* → *"That's good. Quite like it."*
- Topic following / personalisation concept: *"I can follow some topics… all topics segregated."*

**What he found missing or wanted improved:**

1. **Date / timestamp on articles** — His first reaction on seeing a card was: *"I wanted to know when was this news available."* → Recency is a critical trust and relevance signal.

2. **Story threading for ongoing events** — *"On an ongoing topic, do you have a thread maintained? The protest happened for 30 days — I'd like to know based on a timeline what's happening from inception till current."* → Users want continuity, not just one-off articles.

3. **Expand-in-place preview (no forced deep dive)** — *"I'd like to read at least three more lines so I don't have to open each card."* → Users want a middle ground between headline and full article — a 3–5 line summary inline.

4. **Overall summary per topic** — *"An overall summary giving me enough overview so I can choose to go and deep dive."*

5. **Images / visual richness** — *"It's looking very plain. Maybe some images will be nice."* and *"Apart from that, this looks good — just maybe some pictures would be appreciated."*

6. **Video / short-form media integration** — *"Al Jazeera is making 1.5-minute shorts. All of these people have started bite-sized content — maybe that could be associated with these cards."* → He suggested embedding short YouTube video clips alongside text summaries.

7. **Unclear primary navigation** — *"Which is the primary navigation I'm looking at?"* → The prototype had tabs for "Today's Topics," "All Topics," and "Deep Dives" — Animesh found this confusing and redundant.

8. **Trending / breaking news surfacing** — *"Something that's not in my topic but is gaining too much traction… a major thing in the world — that could be surfaced here."* → Users want serendipitous discovery of globally significant news outside their chosen topics.

---

### Jyotish — Prototype Feedback

**What he liked:**
- Content curation quality: *"I think this is curated well."*
- The concept of perspective segments per story (economic, government etc.): *"Multiple perspectives — is this like segments that will get impacted? Good."*

**What he found missing or wanted improved:**

1. **Mobile-first design is critical** — *"I have stopped consuming news on laptops or computers. It's mostly on phone. So I'm seeing this after a long time — it's bringing back memories of 10 years ago."* → The desktop prototype felt unfamiliar and intimidating to him. **The product must be designed mobile-first.**

2. **Visual hierarchy — no "hero story"** — *"One thing that is missing is images. The hierarchy — everything is at the same level right now. Like we used to have a hero story, a big story, and then smaller cutouts. Visually, what is my eye movement right now? I'm finding that a little tricky."* → Flat card grids without size differentiation make it hard to prioritise attention.

3. **Information overload from sources shown upfront** — *"There's so much detailed analysis. Finishing one news and then going to the next one itself gets very tiring."* → Jyotish explicitly said showing all source detail upfront was overwhelming. He stopped reading news due to this fatigue. → *"Maybe not have it upfront — I would then see if I really need to trust [the source]."*

4. **High-level bullet points as default** — *"If you give me just this much — very high-level bullet points — I think I'll be more than happy with that."* → This directly contradicts the prototype's depth-first approach. Users want summary-first, depth on demand.

5. **Personalisation expectation** — *"Maybe this will also get curated based on what I prefer."* → Users assume and expect personalisation to kick in over time.

6. **Topic breadth is overwhelming at first** — *"I don't know what to see. I mean, I'll definitely sort this with maybe if there was a headline that could be helpful."* → The prototype showed too many topics with no clear starting point for new users.

---

## Revised Priority Insights from Prototype Session

| Insight | Source | Revised Priority |
|---|---|---|
| Timestamp / recency on every article | Animesh | 🔴 High — must-have |
| Inline 3–5 line summary (no forced click) | Animesh | 🔴 High — must-have |
| Mobile-first design | Jyotish | 🔴 High — must-have |
| Visual hierarchy / hero story concept | Jyotish | 🔴 High — must-have |
| Source detail hidden by default, expandable | Jyotish | 🔴 High — must-have |
| High-level bullet points as default view | Jyotish | 🔴 High — must-have |
| Images alongside article cards | Both | 🟡 Medium |
| Trending / breaking news outside chosen topics | Animesh | 🟡 Medium |
| Story timeline / thread for ongoing events | Animesh | 🟡 Medium |
| Short-form video (YouTube Shorts / Al Jazeera) integration | Animesh | 🟢 Nice to have |
| Navigation clarity (tabs vs. single feed) | Animesh | 🟡 Medium |

---

## Next Steps

- [ ] Validate MVP feature set with a third interview or prototype test
- [ ] Proceed to solution design and user journey mapping
- [ ] Define technical approach using Bob + Tavily MCP
- [ ] Revisit prototype design with mobile-first, hierarchy, and summary-first principles
