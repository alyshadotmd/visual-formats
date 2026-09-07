---
name: greenscreen-classification
description: How to identify whether an ad should be classified/named as the Greenscreen visual format. Greenscreen ads are always videos, and the hook must open on the greenscreen. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Greenscreen — Classification Guide

## Definition

A **video** where a creator is composited (greenscreened) in front of a full-frame background "screen" (an image, a video, a screenshot, a webpage, a product, or a scene), and the **hook opens on that greenscreen**. The greenscreen is the anchor of the format: there is a relationship between what is on the screen behind them and what the creator is saying.

Greenscreen is almost always the **anchor (primary)** format and frequently pairs with a **secondary** format via the dual-format tagging rule. Example: the Lyka pet food example in the files folder is a greenscreen ad (anchor) that is also an unboxing (secondary), so it would be tagged greenscreen + unboxing.

## The things that must all be true

1. **It's a video.** Greenscreen is never a static.
2. **The hook opens on the greenscreen.** The composited background is there from the first beat and anchors the ad, the same way the comment sticker anchors a comment-response ad. If the greenscreen only shows up later, it isn't the anchor and it isn't this format.
3. **The creator is composited in front of a full-frame background.**
4. **There is a relationship between the background and what the creator is saying.** They can point at it or reference it directly, or the background can simply add a context layer to what they are saying. It does not have to be acknowledged out loud.

## The relationship, two ways

- **Direct (react / reference):** the background is evidence (a screenshot, article, review, chart, or page) and the creator reacts to and points at it ("wait, look at this").
- **Context layer:** the background reinforces or adds to what they are saying without being acknowledged. Example: the Native Pet example, where she talks about probiotic chews with dog chews on the screen behind her but doesn't immediately call them out. The screen adds a layer rather than being reacted to.

Both are Greenscreen, as long as the hook opens on the greenscreen and the background relates to the talk.

## Quick test

Mute it. In the first beat, do you see a person composited in front of a full-frame screen that relates to what they're saying? If yes, Greenscreen. If the greenscreen isn't there in the hook, or there's no relationship between the screen and the talk, it's something else.

## Commonly confused with

- **Yapper:** a talking-head monologue with no greenscreen behind them. If there's no composited background anchoring the hook, it's `yapper`, not Greenscreen.
- **Comment-screenshot:** a screenshotted comment used as the static hero, with no creator composited in front reacting to it. If it's a static comment doing the work, it's `comment-screenshot`.
- **Comment-response:** a native story-reply look (a question sticker over a selfie/lifestyle image, answered by text or on camera), not a creator composited over a full-frame screen. That's `comment-response`.
- **Founder:** founder-to-camera storytelling. A founder can be greenscreened (then it's Greenscreen too, likely dual-tagged), but a founder just telling their story with no greenscreen is `founder`.

## What to look for as supporting signals (not required)

- Fast cuts as the background changes (new point, new screen), common in the react/reference version
- Highlighting, circling, or zooming on a specific part of the screen (react version)
- Casual, low-effort visual treatment: often intentional (the casual-disarm / effort-mismatch mechanic), not a production shortcut

See `execute.md` in this same folder for the full build/scripting rules.
