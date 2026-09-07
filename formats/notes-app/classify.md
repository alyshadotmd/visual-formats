---
name: notes-app-classification
description: How to identify whether an ad should be classified/named as the Notes App visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Notes App — Classification Guide

## Definition

A screenshot styled as a **recognizable Apple Notes card** (the native chrome: back arrow, undo/redo, share, ellipsis) used as the device carrying text, whether that's one standalone note, a tip, a quote, or one point within a longer sequence.

This is a **device**, not a structure. It answers "what is the text sitting inside," not "how many points are there." A single ad with one Notes-card screenshot is Notes App on its own. An ad that uses a Notes card to deliver each point of a multi-slide list is Notes App **plus** `Listicle` (see that format's classification guide), tagged as two `vf:` values.

## The one thing that must be true

There's a **screenshot with visible Apple Notes chrome** (the back arrow / undo-redo / share / ellipsis bar), not just any typed-looking text.

## Quick test

Ask: *does this look like a screenshot of an actual Apple Notes card, chrome and all?* If yes, Notes App. If it's typed text without that specific app chrome, it's a different format.

## Commonly confused with

- **Post-it:** also feels personal/unpolished, but Post-it is a handwritten sticky note or scrawl, not a typed, screenshotted Notes card.
- **Instagram Text Overlay:** native-styled text over an image, but that's Instagram's own type treatment, not Apple's Notes app chrome.
- **Listicle:** if the ad is a multi-slide sequence with one point per slide, check whether it also qualifies as `Listicle` and tag both. Notes App alone doesn't imply a list structure.

See `execute.md` in this same folder for the full build rules.
