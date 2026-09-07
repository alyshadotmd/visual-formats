---
name: instagram-text-overlay-classification
description: How to identify whether an ad should be classified/named as the Instagram Text Overlay visual format. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Instagram Text Overlay — Classification Guide

## Definition

An ad styled as a native Instagram story or post, a **selfie, POV, or lifestyle shot** you'd actually share to your own story, where **Instagram's own native text** carries the message (the story "add text" look, native fonts, optional colored highlight boxes, or the classic caption placement).

It can also use native story elements: a **link sticker**, an **image sticker**, and **overlaid screenshots or images**. The one hard exclusion is a **comment-response (question) sticker** — that belongs to the comment-response format.

## The things that must all be true

1. **Instagram's own native text is carrying the message** (story add-text / caption look, native fonts, highlight boxes), not a designed banner or a generic bold text-over-image static.
2. **The base reads like something a person would post to their story:** a selfie, a POV shot, or a lifestyle shot.
3. **There's no comment-response (question) sticker.** A question sticker + reply is comment-response, not this.

## Allowed (these do NOT disqualify it)

- A **link sticker** (the native IG story link CTA)
- An **image sticker**
- **Overlaid screenshots or images** on the story — you can drop a screenshot or photo on top and it's still this format, as long as native IG text is doing the talking (see the Space Goods and Natural Cycles examples in the files folder)

## Quick test

Would this look like someone's own Instagram story? Is native IG text doing the talking, with **no** question/comment-response sticker? If yes, this format. Link stickers, image stickers, and overlaid screenshots don't change that.

## Commonly confused with

- **Comment Response:** has a question-sticker UI (black bar + question box) plus a reply. A question sticker means `comment-response`, not this. It's the one sticker this format can't have.
- **Comment-screenshot:** a screenshotted comment is the hero, its comment chrome (username, avatar, likes) doing the work. Overlaying a screenshot here is fine; a comment screenshot *being* the ad is `comment-screenshot`.
- **Post-it:** handwriting-styled note, not IG's native typed text.

## What to look for as supporting signals

- UGC-style selfie/POV/lifestyle base image that reads as an organic story
- Caption-voice copy (lowercase energy, contractions, line breaks pacing the read)
- A native link sticker as the CTA, or an image sticker / overlaid screenshot supporting the point
- Brand enters late and lightly

See `execute.md` in this same folder for the full build/scripting rules.
