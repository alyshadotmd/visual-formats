---
name: matching-chart-classification
description: How to identify whether an ad should be classified/named as the Matching Chart visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Matching Chart — Classification Guide

## Definition

A static (usually an image) built as a **matching table**: several self-select categories listed down one side (body type, skin type, hair type, goal, personality, etc.), each mapped straight across to a **recommended product or variant**. The viewer finds the row that's them and reads across to their pick. No branching logic (that's flowchart) and no ranked argument (that's listicle).

## The things that must all be true

1. **A set of parallel self-select categories.** The viewer picks the one that's them from a list of options ("which one are you").
2. **Each category maps to a recommendation** — a product, variant, or answer, read straight across.
3. **It's a lookup/matching structure** — find yourself, read your match — not branching forks and not a sequential list building one argument.

## Quick test

Do you scan a table for your category and read across to your recommended pick, with no yes/no branches? If yes, Matching Chart.

## Commonly confused with

- **Flowchart:** branching yes/no forks with arrows that route you to an answer. If you follow forks, it's `flowchart`; if you find your row in a table, it's matching-chart.
- **Listicle:** an ordered list of points building one argument, not a category → recommendation map.
- **Us vs Them:** a two-column brand-vs-alternative comparison, not self-select category → your pick.
- **Feature-benefit-pointout:** call-outs on one hero product, not multiple categories each mapped to a different product.

## What to look for as supporting signals

- A "Which ___ are you?" / "What ___ is best for you?" headline
- A column of categories (often with little icons/illustrations) aligned to a column of products
- Arrows or aligned rows connecting each category to its match; often implies a shop action

Example in the files folder:

- the Honeylove "What shapewear is best for you?" ad maps body types (Rectangle, Pear, Hourglass, Inverted Triangle, Apple) each to a specific style

See `execute.md` in this same folder for the full build rules.
