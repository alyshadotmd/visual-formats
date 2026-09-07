---
name: ad-in-the-wild-classification
description: How to identify whether an ad should be classified/named as the Ad in the Wild (out-of-home) visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Ad in the Wild (OOH) — Classification Guide

## Definition

An ad staged to look like a **physical out-of-home placement** — a billboard, building wall, bus shelter, or transit poster — composited into a **real-world street or public scene**, usually with sidewalk, city backdrop, and sometimes passersby. The message-within-the-message is the brand's creative; the outer frame makes it look like a big, real-world ad someone is walking past. Usually a static image.

## The things that must all be true

1. **The brand's message is shown as an out-of-home surface** (billboard, wall, poster, transit) rather than filling the whole frame as a plain static.
2. **It's set in a real-world outdoor/public scene** — street, station, building, sky — often with a person or vehicle for scale and realism.
3. **The placement is the device** — the "wow, that's a real billboard in the wild" framing is the point, not just a background texture.

## Quick test

Does it look like a photo of the brand's ad living on a real billboard/wall/poster out in a public space? If yes, Ad in the Wild. If the message just fills the frame with no placement surface, it's a different format.

## Commonly confused with

- **The *inner* creative's own format:** the poster on the billboard can itself be another format (a letter, a feature-benefit-pointout, etc.). Ad in the Wild describes the *outer* placement staging; tag the inner treatment as a secondary format when it's useful.
- **Press:** borrows third-party editorial credibility (publication logos, pull-quotes). Ad in the Wild borrows the scale and legitimacy of a real-world media placement, not a publication.
- **Lifestyle/product static:** a plain product-in-a-scene with no simulated ad surface is not an Ad in the Wild.

## What to look for as supporting signals

- Billboard, wall-scape, bus shelter, or transit frame around the creative
- Street furniture, sidewalk, sky, buildings; a pedestrian or vehicle for scale
- Often AI-composited or mocked-up rather than a genuine photographed placement

Examples in the files folder:

- Honeylove CloudEmbrace streetside billboard
- ARMRA "Have you pooped yet?" highway billboard
- Juniper "Don't weigh in on my weight" transit poster
- Bobbie "trusted by parents… 700K of them" building wall-scape

See `execute.md` in this same folder for the full build rules.
