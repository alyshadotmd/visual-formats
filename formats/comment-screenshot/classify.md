---
name: comment-screenshot-classification
description: How to identify whether an ad should be classified/named as the Comment Screenshot visual format. Covers Instagram, TikTok, and Facebook comments, standing alone or with a reply captured in the same screenshot. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Comment Screenshot — Classification Guide

## Definition

A static whose hero element is a **screenshotted comment left on a social media post** (Instagram, TikTok, or Facebook comment UI: username, avatar, comment text, like count, "Reply", relative timestamp). The screenshotted comment is the hook. It can **stand alone**, the comment itself doing all the work overlaid on the image, or it can include a **reply captured inside the same screenshot** (like the harrys example in the files folder). A response is not required.

## The one thing that must be true

There is a **screenshotted comment-thread UI element** as the visual hero, complete with commenter identity chrome (handle/avatar) and platform comment styling (like count, reply link, timestamp). It is a real (or real-seeming) comment on a post. It is **not** a question or comment-response sticker, and not a plain block of native-styled text.

## Quick test

Ask: *does this look like a screenshot of someone's comment on a social post?* If yes, Comment Screenshot, whether or not anyone replied to it. If the hero is a question / comment-response sticker being answered, that's `comment-response`. If it's caption/story text with no comment-thread chrome, it's something else.

## Commonly confused with

- **Comment Response:** also features social-feeling UI and often a reply, but the hero is a **question / comment-response sticker** (black bar + white question box, or the TikTok equivalent), not a screenshotted comment thread. No visible sticker element, and a real comment screenshot instead, means `comment-screenshot`, not `comment-response`.
- **Instagram Text Overlay:** uses IG's native caption/story text styling directly over an image, with no comment-thread chrome (no username/avatar/like count) at all.
- **Greenscreen:** can also feature a screenshot as evidence, but the creator is composited over it reacting live on video; Comment Screenshot is a static comment screenshot, with no reacting creator overlay required.

## What to look for as supporting signals

- Believable, non-brand-adjacent username/handle
- Casual typed register in the comment text (lowercase starts, contractions)
- Real platform comment chrome (like count, "Reply", relative timestamp)
- Optional reply captured in the same screenshot (often the brand's verified handle, as in the harrys example), but not required

See `execute.md` in this same folder for the full build/scripting rules.
