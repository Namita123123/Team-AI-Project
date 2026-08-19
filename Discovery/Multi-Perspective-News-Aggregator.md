# Multi-Perspective News Aggregator
**Status:** Discovery  
**Last Updated:** 2026-08-14

---

## Problem Statement

People who rely on a single news source or regional publication get an incomplete or biased picture of world events. Most readers are unaware of how differently the same story is framed across geographies, political leanings, or media outlets — leading to uninformed opinions and echo chambers.

---

## Opportunity

There is a growing demand for tools that help users consume news more critically. A tool that automatically gathers, compares, and summarises multiple perspectives on the same story could significantly improve how people understand current events.

---

## Proposed Solution

An AI-assisted tool that:
- Takes a news topic or headline as input
- Searches multiple sources across different regions and viewpoints
- Summarises each perspective clearly and objectively
- Highlights areas of agreement and disagreement across sources
- Flags potential biases or gaps in coverage

---

## Discovery Tasks

### 1. User Research
- [ ] Identify target users (news readers, students, researchers, professionals)
- [ ] Draft research questions to understand news consumption habits
- [ ] Conduct 3–5 interviews with people who actively follow current events
- [ ] Synthesise findings into key themes and pain points

### 2. Problem Validation
- [ ] Confirm whether users are aware of perspective bias in their news consumption
- [ ] Identify current behaviours: do users already cross-reference sources manually?
- [ ] Assess motivation: are users willing to change how they consume news?

### 3. Technical Feasibility
- [ ] Assess Bob's Tavily MCP integration for multi-source news retrieval
- [ ] Explore whether bias detection and perspective labelling is achievable
- [ ] Identify limitations: paywalled content, regional access restrictions
- [ ] Define scope: MVP features vs. future enhancements

### 4. Define Success Metrics
- [ ] What does a successful summary look like for the user?
- [ ] How many perspectives constitute a balanced view (minimum sources)?
- [ ] How will we assess quality and neutrality of summaries?

### 5. Edge Cases to Explore
- [ ] Stories with only one dominant narrative (limited perspective diversity)
- [ ] Breaking news where sources are still developing their coverage
- [ ] Topics where facts themselves are disputed across sources
- [ ] Paywalled or geo-restricted articles
- [ ] Highly political or sensitive topics requiring careful framing

---

## Key Questions

1. Do users currently cross-reference news sources, and how do they do it?
2. What would make users trust an AI-generated perspective summary?
3. How important is source transparency (knowing where each perspective comes from)?
4. Is the goal to inform, or also to challenge the user's existing views?

---

## Next Steps

1. Draft and run user research interviews
2. Summarise findings back into this file
3. Assess technical feasibility with Bob and Tavily
4. Decide whether to proceed to planning and implementation

---

## References

- [Diya Namita Transcript](./Diya%20Namita%20transcript.md)
- Tavily Web Search MCP: already connected to Bob
