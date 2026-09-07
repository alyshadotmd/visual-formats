---
name: post-it-classification
description: How to identify whether an ad should be classified/named as the Post-it visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Post-it — Classification Guide

## Definition

A **handwritten sticky note, torn paper, or handwritten scrawl/arrow annotation** placed over a product shot, packaging, or lifestyle image, carrying one short thought (a reminder, tip, confession, or hype note).

## The two things that must both be true

1. **The text is styled as handwriting** (not typeset), on a note, scrawl, or annotation, not a designed text block.
2. **It's one short thought** (≤12 words per note, or a short stack of ≤3 short notes), not multi-paragraph copy.

## Quick test

Ask: *does this look like someone grabbed a pen and jotted one quick thing on a sticky note or the product itself?* If yes, Post-it. If the handwriting-styled text is actually a full paragraph or letter-length copy, it's `letter`, not `post-it`.

## Commonly confused with

- **Letter:** also can feel personal/handwritten in tone, but Letter has full salutation/body/sign-off structure and much more copy. Post-it is one short thought, physically staged as a note.
- **Instagram Text Overlay:** uses IG's native typed text styling, not handwriting.
- **Comment Response:** uses an app-UI question sticker plus typed reply text, not a physical handwritten note.

## What to look for as supporting signals

- Real, everyday base image (product, packaging, lifestyle scene), not a glossy render
- Casual handwritten markers: underline, dash, doodle arrow, ALL-CAPS on one word
- Brand/offer usually kept off the note itself, placed on a separate small printed anchor if present

See `execute.md` in this same folder for the full build/scripting rules.
