# Carbon Icon Discovery Tool
**Status:** Discovery  
**Last Updated:** 2026-08-14

---

## Problem Statement

Designers and developers working with the Carbon Design System struggle to find the right icon when icon names are technical or unintuitive. This slows down design and development workflows and leads to inconsistent icon usage across products.

---

## Opportunity

When designers encounter a visual pattern they want to represent — such as a screenshot from a competitor product, a hand-drawn sketch, or a vague description — they currently have no tool that bridges the gap between visual intent and the correct Carbon icon name.

---

## Proposed Solution

An AI-assisted tool that:
- Accepts a screenshot, image, or text description as input
- Recommends matching Carbon icons with confidence scores
- Provides alternatives ranked by relevance
- Links directly to the Carbon icon library for immediate use

---

## Discovery Tasks

### 1. User Research
- [ ] Identify target users (designers, front-end developers)
- [ ] Draft research questions to understand the pain point depth
- [ ] Conduct 3–5 interviews with designers or developers who use Carbon
- [ ] Synthesise findings into key themes and pain points

### 2. Problem Validation
- [ ] Confirm frequency of the problem (how often do users struggle with icon discovery?)
- [ ] Identify current workarounds (e.g. manual browsing, Slack asks, Google search)
- [ ] Assess severity: does this block work or just slow it down?

### 3. Technical Feasibility
- [ ] Explore Carbon icon library structure and metadata
- [ ] Assess Bob's `carbon-image-analysis` and `carbon-builder` skills for icon matching
- [ ] Identify whether image-to-icon matching is achievable without external APIs
- [ ] Define scope: MVP features vs. future enhancements

### 4. Define Success Metrics
- [ ] What does a successful solution look like for the user?
- [ ] How will we measure accuracy of icon recommendations?
- [ ] What is the acceptable confidence threshold for a recommendation?

### 5. Edge Cases to Explore
- [ ] Ambiguous or abstract visual inputs
- [ ] Icons that don't exist in Carbon (gap identification)
- [ ] Accessibility considerations for icon usage
- [ ] Multiple valid icon matches with similar meanings

---

## Key Questions

1. How often do designers encounter this problem in a typical week?
2. What is the biggest frustration with the current Carbon icon browsing experience?
3. Would a confidence score alongside suggestions be useful or confusing?
4. Should the tool support text descriptions, images, or both?

---

## Next Steps

1. Draft and run user research interviews
2. Summarise findings back into this file
3. Assess technical feasibility with Bob
4. Decide whether to proceed to planning and implementation

---

## References

- [Diya Namita Transcript](./Diya%20Namita%20transcript.md)
- Carbon Design System Icon Library: https://carbondesignsystem.com/elements/icons/library/
