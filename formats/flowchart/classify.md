---
name: flowchart-classification
description: How to identify whether an ad should be classified/named as the Flowchart visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Flowchart — Classification Guide

## Definition

An ad built as a **decision tree**: a question or entry point at the top, then **branching paths** (yes/no or option forks) connected by **arrows**, routing the viewer down the branch that matches them to a recommendation (usually a specific product or variant). The viewer "follows the arrows to their answer." Usually a static image.

## The things that must all be true

1. **There's a branching structure.** Arrows/connectors route the viewer through choices (yes/no or option forks), not a straight top-to-bottom list.
2. **It starts from a question/entry point and ends at a recommendation** on each branch.
3. **The viewer self-selects a path** — the whole point is "answer these and follow the arrows to the thing for you."

## Quick test

Do you follow arrows through forks to land on a personalized pick? If yes, Flowchart. If it's a straight list with no branching, or a table with no routing, it's something else.

## Commonly confused with

- **Listicle:** a straight, ordered list of points, one per row/slide, no branching. No forks or routing means it's a `listicle`, not a flowchart.
- **Us vs Them:** a two-column comparison of brand vs. alternative, not a branching path to a personalized recommendation.
- **Matching chart / "which one are you":** a table that maps each self-selected category straight to a recommendation, with parallel rows and no decision forks. If there's no branching, it's a matching chart, not a flowchart. (Not yet its own format in this library.)

## What to look for as supporting signals

- A question as the headline ("Is this your ___?", "Which ___ are you?")
- Yes/No labels on the branches, arrows connecting steps
- Each terminal node is a product/variant or a clear next step, ending in a CTA

Example in the files folder:

- the Honeylove "Is this your boob shape?" ad branches through yes/no questions to the CloudEmbrace recommendation

See `execute.md` in this same folder for the full build rules.
