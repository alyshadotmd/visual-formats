# Evergreen example files — index

This folder holds every **year-round (evergreen)** example creative. Black Friday / Cyber Monday examples live in `../bfcm/`. Both use the same format definitions in `../../formats/`. Each ad lives **once**, no duplicate files.

## Naming convention

```
[b=<brand>][_c=<creator>]_s=evergreen_vf=<format>[_vf=<format2>]_ot=none[_tag=favorite][_n=<k>].<ext>
```

At least one of `b=` or `c=` is required. Order is brand, then creator, then season, then visual format(s), then offer type.

- **`b=`** brand, at most one. lowercase, dashes for spaces, strip punctuation, transliterate accents, `&` becomes `and`, keep the true spelling (`comfrt`, `mott-and-bow`, `the-farmers-dog`, `gruns`).
- **`c=`** creator handle, at most one. Same formatting rules as brand.
- **When to use which:**
  - Brand ad (no named creator): `b=<brand>` only.
  - Brand x creator partnership: include **both**, brand first: `b=<brand>_c=<creator>`.
  - Organic content or a creator-led post with no brand: `c=<creator>` only.
- **`s=`** season. Always `evergreen` in this folder (`bfcm` in `../bfcm/`).
- **`vf=`** visual format, one required, **up to two** (a genuine dual-format ad repeats the `vf=` token). Value is the format folder name. **The primary (anchor) format goes first, the secondary format second.**
- **`ot=`** offer type, same tokens and rules as Black Friday (`/agent/brain/black-friday-swipe-file/offer-taxonomy.md`): amount-off, free-gift, bundle, tiered, buy-x-get-y, other, none. Repeats for more than one offer; `none` when the ad shows no offer. Season says when, offer type says what: subscription, first-order and creator-code deals are tagged by the deal itself (added 2026-10-06). Goes after the visual format(s) and before any `_n=`.
- **`tag=`** optional special tag, after offer type. Only value so far: `favorite` = one of Alysha's favorite ads ever. Favorites also get a same-name `.md` beside the file with the source, transcript, and creative analysis pre-read. Find them all by matching `_tag=favorite` (see Favorites below).
- Fields are separated by `_`; values use `-` inside a term; each field is prefixed with its tag and an `=`.
- Extension matches the media (`.jpg`, `.jpeg`, `.png`, `.mp4`).

> `=` is used instead of `:` because it is legal in filenames on Linux, macOS, and Windows, so the repo clones cleanly everywhere once the GitHub mirror is back.

### Collisions
If a new ad would produce a filename identical to an existing one (same brand/creator and same format(s)), append `_n=2`, `_n=3`, and so on in the order added. Never overwrite or delete an existing file to resolve a collision without an explicit instruction on which to keep. Dedupe by bytes first (md5): an exact byte match is a true duplicate, skip it.

### Finding examples
Match the format token: all greenscreen examples are files containing `vf=greenscreen`. (Per-device example lists in the messaging-devices library were cleared on 2026-08-29 and are being rebuilt, so match by format token here for now.)

## ⭐ Favorites

Alysha's favorite ads ever, tagged `_tag=favorite`. Each has a same-name `.md` with the full breakdown. Newest first.

| File | Why it's a favorite |
|---|---|
| `b=vella-studios_s=evergreen_vf=text-message_vf=cart-screenshot_ot=none_tag=favorite.jpg` | Organic post, not an ad (but she'd run it as one). Dad's "$281.15 for groceries" text matches the Pilates class pack total exactly. The price becomes the punchline and you work out the joke yourself. |
| `b=portland-leather-goods_c=heather-grace_s=evergreen_vf=comment-response_vf=yapper_ot=none_tag=favorite.mp4` | Replies to a real comment ("What size did you get?"), shows the proof in the first second, then answers each buyer question in order. "I'm really hard on bags" sells the durability. |

## Entries

| File | Brand | Creator | Visual format(s) |
|---|---|---|---|
| `b=portland-leather-goods_c=heather-grace_s=evergreen_vf=comment-response_vf=yapper_ot=none_tag=favorite.mp4` | portland-leather-goods | heather-grace | comment-response, yapper |
| `b=vella-studios_s=evergreen_vf=text-message_vf=cart-screenshot_ot=none_tag=favorite.jpg` | vella-studios | - | text-message, cart-screenshot |
| `b=actandacre_s=evergreen_vf=case-study_ot=none.jpg` | actandacre | - | case-study |
| `b=agemate_s=evergreen_vf=post-it_ot=amount-off.jpeg` | agemate | - | post-it |
| `b=alo-yoga_s=evergreen_vf=bento-grid_ot=none.jpg` | alo-yoga | - | bento-grid |
| `b=armra_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | armra | - | ad-in-the-wild |
| `b=armra_s=evergreen_vf=web-search_ot=none.jpg` | armra | - | web-search |
| `b=arrae_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | arrae | - | instagram-text-overlay |
| `b=arrae_s=evergreen_vf=whiteboard_ot=none.jpg` | arrae | - | whiteboard |
| `b=atlas-coffee-club_s=evergreen_vf=post-it_ot=none.mp4` | atlas-coffee-club | - | post-it |
| `b=atlas-coffee-club_s=evergreen_vf=text-message_ot=none.jpg` | atlas-coffee-club | - | text-message |
| `b=babylist_s=evergreen_vf=comment-screenshot_ot=none.jpg` | babylist | - | comment-screenshot |
| `b=barkbox_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | barkbox | - | unexpected-text-placement |
| `b=barkbox_s=evergreen_vf=whiteboard_ot=none.jpg` | barkbox | - | whiteboard |
| `b=betterhelp_s=evergreen_vf=post-it_ot=none.mp4` | betterhelp | - | post-it |
| `b=billie_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | billie | - | feature-benefit-pointout |
| `b=billie_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | billie | - | instagram-text-overlay |
| `b=bobbie_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | bobbie | - | ad-in-the-wild |
| `b=boll-and-branch_s=evergreen_vf=press_ot=none.jpeg` | boll-and-branch | - | press |
| `b=boll-and-branch_s=evergreen_vf=web-search_ot=none.jpeg` | boll-and-branch | - | web-search |
| `b=bonafide_s=evergreen_vf=greenscreen_ot=none.mp4` | bonafide | - | greenscreen |
| `b=bonafide_s=evergreen_vf=post-it_ot=none.jpeg` | bonafide | - | post-it |
| `b=brooklinen_s=evergreen_vf=press_ot=none.jpeg` | brooklinen | - | press |
| `b=buoy_s=evergreen_vf=founder_ot=none.mp4` | buoy | - | founder |
| `b=buoy_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | buoy | - | instagram-text-overlay |
| `b=buoy_s=evergreen_vf=podcast_ot=none.mp4` | buoy | - | podcast |
| `b=buoy_s=evergreen_vf=taste-test_vf=yapper_ot=none.mp4` | buoy | - | taste-test + yapper |
| `b=buoy_s=evergreen_vf=us-vs-them_ot=amount-off.jpg` | buoy | - | us-vs-them |
| `b=caraway_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | caraway | - | instagram-text-overlay |
| `b=caraway_s=evergreen_vf=letter_ot=none.jpeg` | caraway | - | letter |
| `b=caraway_s=evergreen_vf=press_ot=none.jpeg` | caraway | - | press |
| `b=caraway_s=evergreen_vf=us-vs-them_ot=none.jpeg` | caraway | - | us-vs-them |
| `b=cartablet_s=evergreen_vf=press_ot=none.jpeg` | cartablet | - | press |
| `b=clickup_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | clickup | - | instagram-text-overlay |
| `b=comfrt_s=evergreen_vf=comment-response_ot=none.mp4` | comfrt | - | comment-response |
| `b=coterie-baby_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | coterie-baby | - | feature-benefit-pointout |
| `b=dae_s=evergreen_vf=us-vs-them_ot=none.jpeg` | dae | - | us-vs-them |
| `b=dedcool_s=evergreen_vf=founder_ot=none.mp4` | dedcool | - | founder |
| `b=dermalogica_s=evergreen_vf=review_ot=none.jpeg` | dermalogica | - | review |
| `b=dermalogica_s=evergreen_vf=product-animation_ot=none.mp4` | dermalogica | - | product-animation |
| `b=dermatica_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | dermatica | - | instagram-text-overlay |
| `b=divi_s=evergreen_vf=statistic_ot=none.jpg` | divi | - | statistic |
| `b=dollar-shave-club_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | dollar-shave-club | - | instagram-text-overlay |
| `b=dose_s=evergreen_vf=fortune-cookie_ot=none.jpg` | dose | - | fortune-cookie |
| `b=dose_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | dose | - | feature-benefit-pointout |
| `b=dose_s=evergreen_vf=flyer_ot=none.jpg` | dose | - | flyer |
| `b=dose_s=evergreen_vf=whiteboard_ot=none.jpg` | dose | - | whiteboard |
| `b=dose_s=evergreen_vf=whiteboard_ot=none_n=2.mp4` | dose | - | whiteboard |
| `b=eight-sleep_s=evergreen_vf=listicle_ot=none.mp4` | eight-sleep | - | listicle |
| `b=ergobaby_s=evergreen_vf=us-vs-them_ot=none.jpeg` | ergobaby | - | us-vs-them |
| `b=everyday-dose_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | everyday-dose | - | instagram-text-overlay |
| `b=everyday-dose_s=evergreen_vf=skit_ot=none.mp4` | everyday-dose | - | skit |
| `b=everyday-dose_s=evergreen_vf=yapper_ot=none.mp4` | everyday-dose | - | yapper |
| `b=feel-goods_s=evergreen_vf=yapper_ot=none.mp4` | feel-goods | - | yapper |
| `b=finalputt_s=evergreen_vf=press_ot=none.jpeg` | finalputt | - | press |
| `b=fiverr_s=evergreen_vf=before-and-after_ot=none.jpg` | fiverr | - | before-and-after |
| `b=flakes_s=evergreen_vf=founder_ot=none.mp4` | flakes | - | founder |
| `b=flakes_s=evergreen_vf=post-it_ot=amount-off.jpeg` | flakes | - | post-it |
| `b=girlfriend-collective_s=evergreen_vf=press_ot=none.jpeg` | girlfriend-collective | - | press |
| `b=glossier_s=evergreen_vf=yapper_ot=none.mp4` | glossier | - | yapper |
| `b=gousto_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | gousto | - | instagram-text-overlay |
| `b=grove-collaborative_s=evergreen_vf=greenscreen_vf=listicle_ot=none.mp4` | grove-collaborative | - | greenscreen + listicle |
| `b=grove-collaborative_s=evergreen_vf=news_ot=none.jpg` | grove-collaborative | - | news |
| `b=gruns_s=evergreen_vf=comment-response_ot=none.jpg` | gruns | - | comment-response |
| `b=gruns_s=evergreen_vf=text-message_ot=none.jpg` | gruns | - | text-message |
| `b=gruns_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | gruns | - | unexpected-text-placement |
| `b=gruns_s=evergreen_vf=us-vs-them_ot=none.jpeg` | gruns | - | us-vs-them |
| `b=happy-mammoth_s=evergreen_vf=ai-animation_ot=none.mp4` | happy-mammoth | - | ai-animation |
| `b=happy-mammoth_s=evergreen_vf=before-and-after_ot=none.jpg` | happy-mammoth | - | before-and-after |
| `b=happy-mammoth_s=evergreen_vf=letter_ot=none.jpeg` | happy-mammoth | - | letter |
| `b=happy-mammoth_s=evergreen_vf=post-it_ot=none.jpeg` | happy-mammoth | - | post-it |
| `b=happy-mammoth_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | happy-mammoth | - | unexpected-text-placement |
| `b=harrys_s=evergreen_vf=comment-screenshot_ot=none.jpg` | harrys | - | comment-screenshot |
| `b=headspace_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | headspace | - | ad-in-the-wild |
| `b=hers_s=evergreen_vf=ad-in-the-wild_ot=amount-off.jpg` | hers | - | ad-in-the-wild |
| `b=hers_s=evergreen_vf=review_ot=none.jpg` | hers | - | review |
| `b=hexclad_s=evergreen_vf=post-it_ot=none.mp4` | hexclad | - | post-it |
| `b=hims_s=evergreen_vf=comment-response_ot=none.jpg` | hims | - | comment-response |
| `b=hinge_s=evergreen_vf=yapper_ot=none.mp4` | hinge | - | yapper |
| `b=honeylove_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | honeylove | - | ad-in-the-wild |
| `b=honeylove_s=evergreen_vf=ai-animation_ot=none.mp4` | honeylove | - | ai-animation |
| `b=honeylove_s=evergreen_vf=comment-response_ot=none.jpg` | honeylove | - | comment-response |
| `b=honeylove_s=evergreen_vf=flowchart_ot=none.jpg` | honeylove | - | flowchart |
| `b=honeylove_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | honeylove | - | instagram-text-overlay |
| `b=honeylove_s=evergreen_vf=matching-chart_ot=none.jpg` | honeylove | - | matching-chart |
| `b=honour-health_s=evergreen_vf=whiteboard_ot=none.mp4` | honour-health | - | whiteboard |
| `b=huda-beauty_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | huda-beauty | - | asmr + unboxing |
| `b=huel_s=evergreen_vf=explainer_ot=none.mp4` | huel | - | explainer |
| `b=huel_s=evergreen_vf=letter_ot=none.jpeg` | huel | - | letter |
| `b=hum-nutrition_s=evergreen_vf=web-search_ot=none.jpg` | hum-nutrition | - | web-search |
| `b=hydrant_s=evergreen_vf=line-chart_ot=buy-x-get-y.jpg` | hydrant | - | line-chart |
| `b=hydrant_s=evergreen_vf=post-it_ot=none.jpeg` | hydrant | - | post-it |
| `b=hydrant_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | hydrant | - | unexpected-text-placement |
| `b=hydrant_s=evergreen_vf=point-to-screen_ot=buy-x-get-y.mp4` | hydrant | - | point-to-screen |
| `b=ilia-beauty_s=evergreen_vf=behind-the-scenes_ot=none.mp4` | ilia-beauty | - | behind-the-scenes |
| `b=infinity-hoop_s=evergreen_vf=us-vs-them_ot=amount-off_ot=free-gift.jpeg` | infinity-hoop | - | us-vs-them |
| `b=instant-hydration_s=evergreen_vf=letter_ot=none.jpeg` | instant-hydration | - | letter |
| `b=instant-hydration_s=evergreen_vf=skit_ot=none.mp4` | instant-hydration | - | skit |
| `b=intelligent-change_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | intelligent-change | - | instagram-text-overlay |
| `b=javvy_s=evergreen_vf=comment-response_vf=behind-the-scenes_ot=none.mp4` | javvy | - | comment-response + behind-the-scenes |
| `b=javvy_s=evergreen_vf=notes-app_ot=none.jpg` | javvy | - | notes-app |
| `b=javvy_s=evergreen_vf=whiteboard_ot=none.jpg` | javvy | - | whiteboard |
| `b=jcrew_s=evergreen_vf=flatlay_ot=none.jpg` | jcrew | - | flatlay |
| `b=jenny-bird_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | jenny-bird | - | instagram-text-overlay |
| `b=jolie_s=evergreen_vf=statistic_ot=none.jpg` | jolie | - | statistic |
| `b=jolie_s=evergreen_vf=statistic_ot=none_n=2.jpg` | jolie | - | statistic |
| `b=jones-road-beauty_s=evergreen_vf=founder_ot=none.mp4` | jones-road-beauty | - | founder |
| `b=jones-road-beauty_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | jones-road-beauty | - | instagram-text-overlay |
| `b=jones-road-beauty_s=evergreen_vf=letter_ot=none.jpeg` | jones-road-beauty | - | letter |
| `b=juniper_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | juniper | - | ad-in-the-wild |
| `b=kitsch_s=evergreen_vf=post-it_ot=amount-off.mp4` | kitsch | - | post-it |
| `b=kitsch_s=evergreen_vf=skit_ot=none.mp4` | kitsch | - | skit |
| `b=kosas_s=evergreen_vf=founder_ot=none.mp4` | kosas | - | founder |
| `b=laseraway_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | laseraway | - | instagram-text-overlay |
| `b=lemme_s=evergreen_vf=comment-response_ot=none.jpeg` | lemme | - | comment-response |
| `b=lemme_s=evergreen_vf=comment-screenshot_ot=none.jpeg` | lemme | - | comment-screenshot |
| `b=lemme_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | lemme | - | feature-benefit-callout |
| `b=little-caesars_c=jaredbuccii_s=evergreen_vf=skit_ot=none.mp4` | little-caesars | jaredbuccii | skit |
| `b=loop_s=evergreen_vf=comment-response_ot=none.jpg` | loop | - | comment-response |
| `b=loop_s=evergreen_vf=flyer_ot=amount-off.jpg` | loop | - | flyer |
| `b=loop_s=evergreen_vf=greenscreen_ot=none.mp4` | loop | - | greenscreen |
| `b=loop_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | loop | - | instagram-text-overlay |
| `b=loop_s=evergreen_vf=meme_ot=none.jpg` | loop | - | meme |
| `b=loop_s=evergreen_vf=street-interview_ot=none.mp4` | loop | - | street-interview |
| `b=lume-deodorant_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | lume-deodorant | - | instagram-text-overlay |
| `b=lume-deodorant_s=evergreen_vf=letter_ot=none.jpeg` | lume-deodorant | - | letter |
| `b=lyka_s=evergreen_vf=greenscreen_ot=none.mp4` | lyka | - | greenscreen |
| `b=lyka_s=evergreen_vf=letter_ot=none.jpg` | lyka | - | letter |
| `b=lyka_s=evergreen_vf=us-vs-them_ot=none.jpeg` | lyka | - | us-vs-them |
| `b=made-in_s=evergreen_vf=bento-grid_ot=none.jpg` | made-in | - | bento-grid |
| `b=made-in_s=evergreen_vf=product-grid_ot=amount-off.jpg` | made-in | - | product-grid |
| `b=magic-mind_s=evergreen_vf=sign_ot=none.jpg` | magic-mind | - | sign |
| `b=marpipe_s=evergreen_vf=letter_ot=none.jpeg` | marpipe | - | letter |
| `b=mejuri_s=evergreen_vf=product-grid_ot=none.jpeg` | mejuri | - | product-grid |
| `b=meller_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | meller | - | instagram-text-overlay |
| `b=menofmanual_s=evergreen_vf=before-and-after_ot=none.jpg` | menofmanual | - | before-and-after |
| `b=menofmanual_s=evergreen_vf=feature-benefit-pointout_ot=amount-off.jpeg` | menofmanual | - | feature-benefit-pointout |
| `b=merit_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | merit | - | feature-benefit-callout |
| `b=misfits-market_s=evergreen_vf=founder_ot=none.mp4` | misfits-market | - | founder |
| `b=misfits-market_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | misfits-market | - | instagram-text-overlay |
| `b=momcozy_s=evergreen_vf=yapper_ot=none.mp4` | momcozy | - | yapper |
| `b=monday-haircare_s=evergreen_vf=press_ot=none.jpeg` | monday-haircare | - | press |
| `b=moon-juice_s=evergreen_vf=before-and-after_ot=none.jpg` | moon-juice | - | before-and-after |
| `b=moon-magic_s=evergreen_vf=comment-response_ot=none.png` | moon-magic | - | comment-response |
| `b=moonbrew_s=evergreen_vf=founder_ot=none.mp4` | moonbrew | - | founder |
| `b=mott-and-bow_s=evergreen_vf=comment-screenshot_ot=none.jpg` | mott-and-bow | - | comment-screenshot |
| `b=mott-and-bow_s=evergreen_vf=post-it_ot=none.jpeg` | mott-and-bow | - | post-it |
| `b=mous_s=evergreen_vf=high-production-edit_ot=none.mp4` | mous | - | high-production-edit |
| `b=mud-wtr_s=evergreen_vf=founder_ot=none.mp4` | mud-wtr | - | founder |
| `b=nanit_s=evergreen_vf=found-footage_vf=post-it_ot=none.mp4` | nanit | - | found-footage + post-it |
| `b=native-pet_s=evergreen_vf=greenscreen_ot=none.mp4` | native-pet | - | greenscreen |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=none_n=3.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=4.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=line-chart_ot=none.jpg` | natural-cycles | - | line-chart |
| `b=nestig_s=evergreen_vf=comment-response_ot=none.jpeg` | nestig | - | comment-response |
| `b=nutrafol-men_s=evergreen_vf=before-and-after_ot=none.jpg` | nutrafol-men | - | before-and-after |
| `b=o-positiv_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | o-positiv | - | asmr + unboxing |
| `b=o-positiv_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | o-positiv | - | feature-benefit-callout |
| `b=o-positiv_s=evergreen_vf=post-it_ot=none.jpg` | o-positiv | - | post-it |
| `b=o-positiv_s=evergreen_vf=review_ot=none.jpg` | o-positiv | - | review |
| `b=oats-overnight_s=evergreen_vf=founder_ot=none.mp4` | oats-overnight | - | founder |
| `b=obvi_s=evergreen_vf=whiteboard_ot=none.jpg` | obvi | - | whiteboard |
| `b=olipop_s=evergreen_vf=asmr_ot=none.mp4` | olipop | - | asmr |
| `b=olipop_s=evergreen_vf=meme_ot=none.jpeg` | olipop | - | meme |
| `b=onnit_s=evergreen_vf=venn-diagram_vf=whiteboard_ot=none.jpg` | onnit | - | venn-diagram + whiteboard |
| `b=orgain_s=evergreen_vf=toggle_ot=none.jpg` | orgain | - | toggle |
| `b=our-place_s=evergreen_vf=letter_ot=none.jpeg` | our-place | - | letter |
| `b=pehr_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | pehr | - | instagram-text-overlay |
| `b=pela-case_s=evergreen_vf=founder_ot=none.mp4` | pela-case | - | founder |
| `b=primally-pure-skincare_s=evergreen_vf=before-and-after_ot=amount-off.jpg` | primally-pure-skincare | - | before-and-after |
| `b=prose_s=evergreen_vf=before-and-after_vf=listicle_ot=none.mp4` | prose | - | before-and-after + listicle |
| `b=prose_s=evergreen_vf=letter_ot=amount-off.jpeg` | prose | - | letter |
| `b=purdy-and-figg_s=evergreen_vf=letter_ot=none.jpg` | purdy-and-figg | - | letter |
| `b=purple_s=evergreen_vf=letter_ot=none.jpeg` | purple | - | letter |
| `b=purple_s=evergreen_vf=us-vs-them_ot=none.jpeg` | purple | - | us-vs-them |
| `b=rheal_s=evergreen_vf=handwritten_ot=amount-off_ot=free-gift_ot=other.jpeg` | rheal | - | handwritten |
| `b=rheal_s=evergreen_vf=notes-app_vf=listicle_ot=none.jpeg` | rheal | - | notes-app + listicle |
| `b=rheal_s=evergreen_vf=post-it_ot=none.mp4` | rheal | - | post-it |
| `b=rough-country_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | rough-country | - | asmr + unboxing |
| `b=runna_s=evergreen_vf=post-it_ot=none.mp4` | runna | - | post-it |
| `b=ryze_s=evergreen_vf=annotation_ot=none.mp4` | ryze | - | annotation |
| `b=saie-beauty_s=evergreen_vf=press_ot=none.jpg` | saie-beauty | - | press |
| `b=sans_s=evergreen_vf=feature-benefit-callout_ot=none.jpeg` | sans | - | feature-benefit-callout |
| `b=sans_s=evergreen_vf=live-demo_ot=none.mp4` | sans | - | live-demo |
| `b=scentbird_s=evergreen_vf=post-it_ot=none.mp4` | scentbird | - | post-it |
| `b=seed_c=bobby-parrish_s=evergreen_vf=explainer_ot=amount-off_ot=free-gift.mp4` | seed | bobby-parrish | explainer |
| `b=seed_s=evergreen_vf=text-echo_ot=amount-off.jpeg` | seed | - | text-echo |
| `b=seed_s=evergreen_vf=faq_ot=none.jpeg` | seed | - | faq |
| `b=seed_s=evergreen_vf=whiteboard_ot=none.mp4` | seed | - | whiteboard |
| `b=smol_s=evergreen_vf=post-it_ot=none.mp4` | smol | - | post-it |
| `b=solawave_s=evergreen_vf=yapper_vf=graphic-anchor_ot=none.mp4` | solawave | - | yapper + graphic-anchor |
| `b=solderstick_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | solderstick | - | instagram-text-overlay |
| `b=solderstick_s=evergreen_vf=us-vs-them_ot=none.jpeg` | solderstick | - | us-vs-them |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=amount-off_n=2.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=amount-off_n=3.mp4` | spacegoods | - | instagram-text-overlay |
| `b=suri_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | suri | - | instagram-text-overlay |
| `b=suri_s=evergreen_vf=press_ot=none.jpeg` | suri | - | press |
| `b=surreal_s=evergreen_vf=behind-the-scenes_ot=none.mp4` | surreal | - | behind-the-scenes |
| `b=the-farmers-dog_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | the-farmers-dog | - | feature-benefit-pointout |
| `b=the-farmers-dog_s=evergreen_vf=post-it_ot=amount-off.jpeg` | the-farmers-dog | - | post-it |
| `b=the-oodie_s=evergreen_vf=us-vs-them_ot=none.jpg` | the-oodie | - | us-vs-them |
| `b=thrive-causemetics_s=evergreen_vf=comment-response_ot=none.jpeg` | thrive-causemetics | - | comment-response |
| `b=thrive-causemetics_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | thrive-causemetics | - | instagram-text-overlay |
| `b=thrive-causemetics_s=evergreen_vf=post-it_ot=none.jpeg` | thrive-causemetics | - | post-it |
| `b=timeline-longevity_s=evergreen_vf=instagram-text-overlay_ot=amount-off.mp4` | timeline-longevity | - | instagram-text-overlay |
| `b=timeline-longevity_s=evergreen_vf=press_ot=none.jpeg` | timeline-longevity | - | press |
| `b=timeline-longevity_s=evergreen_vf=us-vs-them_ot=none.jpeg` | timeline-longevity | - | us-vs-them |
| `b=trade_s=evergreen_vf=comment-response_vf=us-vs-them_ot=none.jpg` | trade | - | comment-response + us-vs-them |
| `b=trade_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | trade | - | instagram-text-overlay |
| `b=viome_s=evergreen_vf=press_ot=none.jpg` | viome | - | press |
| `b=vitable_s=evergreen_vf=post-it_ot=none.jpeg` | vitable | - | post-it |
| `b=vrbo_s=evergreen_vf=whiteboard_ot=none.mp4` | vrbo | - | whiteboard |
| `b=vuori_s=evergreen_vf=bento-grid_ot=none.jpeg` | vuori | - | bento-grid |
| `b=wild-nutrition_s=evergreen_vf=us-vs-them_ot=none.jpeg` | wild-nutrition | - | us-vs-them |
| `b=winona_s=evergreen_vf=comment-response_ot=none.jpg` | winona | - | comment-response |
| `b=your-heights_s=evergreen_vf=sign_ot=none.jpg` | your-heights | - | sign |
| `b=your-heights_s=evergreen_vf=us-vs-them_ot=none.jpeg` | your-heights | - | us-vs-them |
| `b=your-heights_s=evergreen_vf=yapper_ot=none.mp4` | your-heights | - | yapper |
