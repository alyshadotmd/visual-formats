---
name: flyer-classification
description: How to identify whether an ad should be classified/named as the Flyer visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Flyer — Classification Guide

## Definition

A single printed sheet shown visibly **taped, stapled, or tacked into a real everyday space** — a hydro pole, community board, elevator wall, laundromat, storefront window, bus-stop pillar. Low-fi and handmade-feeling. The device borrows **grassroots, "a real person printed this and stuck it up" authenticity**, not the scale or spend of a paid media placement. Usually a static image; sometimes a scene with a passerby interacting with the sheet.

## The things that must all be true

1. **The brand's message is carried on a single printed sheet** (a flyer/poster), not a large-format built surface.
2. **It's physically affixed** (tape, staples, tacks) **into a real, ordinary public or semi-public space** — pole, board, wall, window.
3. **The scrappy grassroots placement is the device** — the point is that it looks handmade and stuck up by a person, not bought. If you strip the placement, the whole idea deflates.

## Quick test

Does it look like a flyer someone printed and taped up around town? Flyer. Does it look like a paid billboard, transit poster, or wall-scape? That's `ad-in-the-wild`.

## Commonly confused with

- **`ad-in-the-wild` (OOH):** a large paid-media surface (billboard, transit, building wall-scape) that borrows **scale and legitimacy**. Flyer is the opposite signal: small, non-paid-looking, grassroots. The dividing line is paid-media scale vs. handmade-sheet scrappiness.
- **`letter`:** a chunky text-block image with one headline hook and no physical staging. Flyer shows a sheet affixed in a real scene; letter fills the frame as a plain static.
- **The *inner* treatment:** the sheet itself can carry another format — a wanted/missing-poster meme, a listicle, a review. Tag that inner treatment as a **secondary** format when it's useful (e.g. `flyer + meme`). Flyer describes the outer placement.

## What to look for as supporting signals

- Tape corners, staples, or pushpins holding a sheet to a textured pole/board/wall
- Tear-off phone-number tabs; "missing," "wanted," "lost," or "free to a good home" flyer tropes
- A hand or passerby interacting with the sheet; slightly off-angle, handheld framing
- Real-space texture behind the sheet (brick, corkboard, elevator panel, glass)

Examples in the files folder:

- Loop "SUSPECT: Full Coverage Bundle" wanted-poster taped in an elevator (inner treatment: meme)

See `execute.md` in this same folder for the full build rules.
