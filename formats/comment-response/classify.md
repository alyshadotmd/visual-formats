---
name: comment-response-classification
description: How to identify whether an ad should be classified/named as the Comment Response visual format. Covers Instagram and TikTok, static or video. Use when naming an ad (resolving the Visual Format taxonomy token) or auditing an existing ad's format tag. Distinct from execute.md, which governs how to build one.
---

# Comment Response — Classification Guide

## Definition

An ad built to look like a person **acknowledging and answering a question posed through a comment-response sticker** on Instagram or TikTok. On Instagram that is the question sticker (the black-bar prompt with a user-typed question in the white box below, the classic "Ask me anything"); on TikTok it is the equivalent comment-response sticker. The whole move of the ad is "someone asked this, here's my reply." It can run as a **static** with a free-placed text-overlay reply, or as a **video** where the creator's on-camera response is the content.

## The two things that must both be true

1. **There's a comment-response / question sticker** from Instagram or TikTok (the black-bar-plus-white-box question sticker, or TikTok's equivalent) presented as the thing being answered. Not a screenshotted comment, and not plain caption text.
2. **The ad acknowledges and replies to it**, either as free-placed native **text overlay** answering the question (static or video), OR as a **video whose whole point is the creator responding to that question** on camera.

If there's no question sticker being answered, or the "reply" is really a generic hook/caption, it's a different format.

## Quick test

Ask: *does this look like someone answering a question posed through an Instagram or TikTok question sticker?* If yes, Comment Response, whether the reply is written over the frame or spoken in the video. If the hero is a screenshotted comment instead of a question sticker, it belongs in the comment-screenshot format, not here.

## Platform + format variants (all still Comment Response)

- Instagram question sticker (AMA) answered in free-placed text overlay. The original static form.
- TikTok comment-response sticker answered the same way.
- A video (Instagram or TikTok) where the creator reads or references the sticker question and responds to it as the body of the ad (e.g. the Javvy example in the files folder).

## Commonly confused with

- **Comment-screenshot (the `comment-screenshot` format):** the hero is a **screenshotted real comment** (username, avatar, like count, timestamp), not a question sticker. If you see comment-thread chrome instead of a question sticker, classify it there, not as Comment Response.
- **Instagram Text Overlay:** IG's native caption/story text with no question being posed and answered. No Q&A structure means `instagram-text-overlay`.
- **Yapper:** a straight-to-camera monologue with no specific sticker question being answered is `yapper`. A Comment Response video must be anchored to a specific question it is replying to.
- **Post-it:** handwritten-feeling personal text over a scene, not a platform question sticker.

## What to look for as supporting signals

- Native Instagram/TikTok question-sticker UI (the black-bar prompt plus white question box, or TikTok's equivalent)
- Casual, non-studio setting (selfie, mirror selfie, POV product-in-hand, or talking head)
- The reply reads verdict-first, first person, answering the specific question
- For video: the creator explicitly references the question ("someone asked…", "you asked…") before answering

See `execute.md` in this same folder for the full build/scripting rules.
