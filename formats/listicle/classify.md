---
name: listicle-classification
description: How to identify whether an ad should be classified/named as the Listicle visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Listicle — Classification Guide

## Definition

**A list of things.** That's it. Two or more discrete items presented as a list — numbered or not, in a single frame or across multiple slides. The list *is* the format.

The device that carries the list (plain overlay text, a Notes-app card, a handwritten note, icon+label rows, photo captions) is a separate dimension. A Listicle **often also carries a device-format tag** (commonly `Notes App`, but also `Post-it`, `Instagram Text Overlay`, etc.), tagged as two `vf:` values.

## The thing that must be true

There is a **list of 2+ discrete items**. Delivery doesn't matter:
- stacked in **one frame** (rows/bullets/lines), or
- across **multiple slides**, one item per slide.

Numbering is optional. Order may or may not matter. If it reads as a list of separate things, it's a Listicle.

## Quick test

Is the content a list of separate items I read through? If yes, Listicle.

## Commonly confused with

- **Feature Benefit Pointout:** also enumerates points, but they are **call-outs that point *at* specific parts of the product** (lines/arrows to features). If the list does **not** point at the product and just presents items beside/over it, it's Listicle.
- **Us Vs Them:** a two-column comparison table (brand vs. alternative), not a one-direction list.
- **Notes App:** a common device paired with a listicle — check `notes-app/classify.md` separately.

## Supporting signals

- Single-frame: a stack of bulleted/numbered lines or icon+label rows.
- Multi-slide: a cover/title slide, consistent treatment across slides, one item per slide.

Example in the files folder:

- Merit "SPF that doubles as a blur filter" — a single-frame list of four benefit rows (Blurs pores, Evens skin tone, Shields with mineral SPF, Feels like nothing) beside the product, none pointing at it

See `execute.md` in this same folder for the full build rules.
