---
name: unboxing-classification
description: How to identify whether an ad should be classified/named as the Unboxing visual format. Use when naming an ad or auditing its format tag. Distinct from execute.md, which governs how to build one.
---

# Unboxing — Classification Guide

## Definition

A video built around the **reveal of a product from its packaging** — opening the box, cutting the tape, pulling back wrapping, lifting out and laying out what's inside. The **anticipation and the reveal are the hook**, and it usually carries voiceover or talking (this is what separates it from sound-led ASMR).

## The things that must all be true

1. **A packaged product is opened on camera.** There is a box, mailer, pouch, or wrapper that gets opened.
2. **The reveal is the spine of the ad.** The build is anticipation then payoff: what's inside, what you get, first impressions.
3. **First-look framing.** It's shot as discovering the product for the first time (contents laid out, "here's everything that comes with it").

## Quick test

Is the whole ad organized around opening a package and showing what's inside? If yes, Unboxing. If the ad is instead organized around amplified tactile sound with little or no talking, it's ASMR, not Unboxing.

## Commonly confused with

- **ASMR:** sound-led, reveal-agnostic, little or no voiceover. Unboxing is reveal-led and usually has talking. (An ad can be **both** — see the dual-format note below.)
- **Behind-the-scenes:** how the product is *made/developed*, not how it's *unpacked*.
- **Demo:** feature explanation and use, after the product is already out of the box.
- **Haul:** multiple products shown/reviewed; unboxing centers on opening one package.

## Dual-format note

Unboxing pairs cleanly as a **secondary** format. An install or reveal video that is both sound-led and reveal-led can carry two `vf=` tags (e.g. `vf=asmr_vf=unboxing`). Tag Unboxing as the secondary when the packaging reveal is present but a different format (ASMR, founder, greenscreen) is doing the primary work.

## Signals

Box/mailer/wrapper on camera, tape or seal being opened, contents lifted out and arranged, "here's what comes with it," first-impression reactions, close-ups of the packaging and the product's first appearance.

Example carrying this tag: `b=rough-country_vf=asmr_vf=unboxing.mp4` (in `../files/`) — a truck bed-cover install that reveals the product as it's unpacked and fitted; it leans ASMR (primary), with Unboxing as the secondary reveal tag. A dedicated Unboxing-primary example is still needed.

See `execute.md` for the build rules.
