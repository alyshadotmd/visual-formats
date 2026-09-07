# Example files — master index (shared)

This folder is the **single source of truth for every example creative** in the ideation system. Each ad lives here **once**, no duplicate files.

## Naming convention

```
[b=<brand>][_c=<creator>]_vf=<format>[_vf=<format2>].<ext>
```

At least one of `b=` or `c=` is required. Order is brand, then creator, then visual format(s).

- **`b=`** brand, at most one. lowercase, dashes for spaces, strip punctuation, transliterate accents, `&` becomes `and`, keep the true spelling (`comfrt`, `mott-and-bow`, `the-farmers-dog`, `gruns`).
- **`c=`** creator handle, at most one. Same formatting rules as brand.
- **When to use which:**
  - Brand ad (no named creator): `b=<brand>` only.
  - Brand x creator partnership: include **both**, brand first: `b=<brand>_c=<creator>`.
  - Organic content or a creator-led post with no brand: `c=<creator>` only.
- **`vf=`** visual format, one required, **up to two** (a genuine dual-format ad repeats the `vf=` token). Value is the format folder name. **The primary (anchor) format goes first, the secondary format second.**
- Fields are separated by `_`; values use `-` inside a term; each field is prefixed with its tag and an `=`.
- Extension matches the media (`.jpg`, `.jpeg`, `.png`, `.mp4`).

> `=` is used instead of `:` because it is legal in filenames on Linux, macOS, and Windows, so the repo clones cleanly everywhere once the GitHub mirror is back.

### Collisions
If a new ad would produce a filename identical to an existing one (same brand/creator and same format(s)), append `_n=2`, `_n=3`, and so on in the order added. Never overwrite or delete an existing file to resolve a collision without an explicit instruction on which to keep. Dedupe by bytes first (md5): an exact byte match is a true duplicate, skip it.

### Finding examples
Match the format token: all greenscreen examples are files containing `vf=greenscreen`. (Per-device example lists in the messaging-devices library were cleared on 2026-08-29 and are being rebuilt, so match by format token here for now.)

## Entries

| File | Brand | Creator | Visual format(s) |
|---|---|---|---|
| `b=actandacre_vf=case-study.jpg` | actandacre | - | case-study |
| `b=agemate_vf=post-it.jpeg` | agemate | - | post-it |
| `b=armra_vf=ad-in-the-wild.jpg` | armra | - | ad-in-the-wild |
| `b=arrae_vf=instagram-text-overlay.jpeg` | arrae | - | instagram-text-overlay |
| `b=arrae_vf=whiteboard.jpg` | arrae | - | whiteboard |
| `b=atlas-coffee-club_vf=post-it.mp4` | atlas-coffee-club | - | post-it |
| `b=atlas-coffee-club_vf=text-message.jpg` | atlas-coffee-club | - | text-message |
| `b=atlas-coffee-club_vf=us-vs-them.jpeg` | atlas-coffee-club | - | us-vs-them |
| `b=babylist_vf=comment-screenshot.jpg` | babylist | - | comment-screenshot |
| `b=barkbox_vf=ai-generated-static.jpg` | barkbox | - | ai-generated-static |
| `b=barkbox_vf=whiteboard.jpg` | barkbox | - | whiteboard |
| `b=betterhelp_vf=post-it.mp4` | betterhelp | - | post-it |
| `b=billie_vf=feature-benefit-pointout.jpeg` | billie | - | feature-benefit-pointout |
| `b=billie_vf=feature-benefit-pointout_n=2.jpeg` | billie | - | feature-benefit-pointout |
| `b=billie_vf=instagram-text-overlay.jpeg` | billie | - | instagram-text-overlay |
| `b=bobbie_vf=ad-in-the-wild.jpg` | bobbie | - | ad-in-the-wild |
| `b=bonafide_vf=greenscreen.mp4` | bonafide | - | greenscreen |
| `b=bonafide_vf=post-it.jpeg` | bonafide | - | post-it |
| `b=brooklinen_vf=press.jpeg` | brooklinen | - | press |
| `b=buoy_vf=founder.mp4` | buoy | - | founder |
| `b=buoy_vf=us-vs-them.jpg` | buoy | - | us-vs-them |
| `b=caraway_vf=instagram-text-overlay.jpeg` | caraway | - | instagram-text-overlay |
| `b=caraway_vf=letter.jpeg` | caraway | - | letter |
| `b=caraway_vf=press.jpeg` | caraway | - | press |
| `b=caraway_vf=us-vs-them.jpeg` | caraway | - | us-vs-them |
| `b=cartablet_vf=press.jpeg` | cartablet | - | press |
| `b=casely_vf=instagram-text-overlay.jpeg` | casely | - | instagram-text-overlay |
| `b=clickup_vf=instagram-text-overlay.jpeg` | clickup | - | instagram-text-overlay |
| `b=comfrt_vf=comment-response.mp4` | comfrt | - | comment-response |
| `b=coterie-baby_vf=feature-benefit-pointout.jpeg` | coterie-baby | - | feature-benefit-pointout |
| `b=current_vf=post-it.mp4` | current | - | post-it |
| `b=dae_vf=us-vs-them.jpeg` | dae | - | us-vs-them |
| `b=dedcool_vf=founder.mp4` | dedcool | - | founder |
| `b=dermatica_vf=instagram-text-overlay.jpeg` | dermatica | - | instagram-text-overlay |
| `b=divi_vf=statistic.jpg` | divi | - | statistic |
| `b=dollar-shave-club_vf=instagram-text-overlay.jpeg` | dollar-shave-club | - | instagram-text-overlay |
| `b=dose_vf=ai-generated-static.jpg` | dose | - | ai-generated-static |
| `b=dose_vf=feature-benefit-pointout.jpeg` | dose | - | feature-benefit-pointout |
| `b=dose_vf=feature-benefit-pointout_n=2.jpeg` | dose | - | feature-benefit-pointout |
| `b=dose_vf=whiteboard.jpg` | dose | - | whiteboard |
| `b=dose_vf=whiteboard_n=2.mp4` | dose | - | whiteboard |
| `b=ergobaby_vf=us-vs-them.jpeg` | ergobaby | - | us-vs-them |
| `b=everyday-dose_vf=instagram-text-overlay.jpeg` | everyday-dose | - | instagram-text-overlay |
| `b=everyday-dose_vf=yapper.mp4` | everyday-dose | - | yapper |
| `b=finalputt_vf=press.jpeg` | finalputt | - | press |
| `b=fiverr_vf=before-and-after.jpg` | fiverr | - | before-and-after |
| `b=flakes_vf=founder.mp4` | flakes | - | founder |
| `b=flakes_vf=post-it.jpeg` | flakes | - | post-it |
| `b=girlfriend-collective_vf=press.jpeg` | girlfriend-collective | - | press |
| `b=glossier_vf=yapper.mp4` | glossier | - | yapper |
| `b=gousto_vf=instagram-text-overlay.jpeg` | gousto | - | instagram-text-overlay |
| `b=grove-collaborative_vf=greenscreen_vf=listicle.mp4` | grove-collaborative | - | greenscreen + listicle |
| `b=gruns_vf=comment-response.jpg` | gruns | - | comment-response |
| `b=gruns_vf=text-message.jpg` | gruns | - | text-message |
| `b=gruns_vf=us-vs-them.jpeg` | gruns | - | us-vs-them |
| `b=gruns_vf=written-on-body.jpg` | gruns | - | written-on-body |
| `b=happy-mammoth_vf=letter.jpeg` | happy-mammoth | - | letter |
| `b=happy-mammoth_vf=post-it.jpeg` | happy-mammoth | - | post-it |
| `b=happy-mammoth_vf=written-on-body.jpg` | happy-mammoth | - | written-on-body |
| `b=harrys_vf=comment-screenshot.jpg` | harrys | - | comment-screenshot |
| `b=hexclad_vf=post-it.mp4` | hexclad | - | post-it |
| `b=hims_vf=comment-response.jpg` | hims | - | comment-response |
| `b=hinge_vf=yapper.mp4` | hinge | - | yapper |
| `b=honeylove_vf=ad-in-the-wild.jpg` | honeylove | - | ad-in-the-wild |
| `b=honeylove_vf=ai-animation.mp4` | honeylove | - | ai-animation |
| `b=honeylove_vf=comment-response.jpg` | honeylove | - | comment-response |
| `b=honeylove_vf=flowchart.jpg` | honeylove | - | flowchart |
| `b=honeylove_vf=instagram-text-overlay.jpg` | honeylove | - | instagram-text-overlay |
| `b=honeylove_vf=matching-chart.jpg` | honeylove | - | matching-chart |
| `b=huel_vf=letter.jpeg` | huel | - | letter |
| `b=hydrant_vf=post-it.jpeg` | hydrant | - | post-it |
| `b=ilia-beauty_vf=behind-the-scenes.mp4` | ilia-beauty | - | behind-the-scenes |
| `b=infinity-hoop_vf=us-vs-them.jpeg` | infinity-hoop | - | us-vs-them |
| `b=instant-hydration_vf=letter.jpeg` | instant-hydration | - | letter |
| `b=intelligent-change_vf=instagram-text-overlay.jpeg` | intelligent-change | - | instagram-text-overlay |
| `b=javvy_vf=comment-response_vf=unboxing.mp4` | javvy | - | comment-response + unboxing |
| `b=jcrew_vf=flatlay.jpg` | jcrew | - | flatlay |
| `b=jenny-bird_vf=instagram-text-overlay.jpeg` | jenny-bird | - | instagram-text-overlay |
| `b=jolie_vf=statistic.jpg` | jolie | - | statistic |
| `b=jolie_vf=statistic_n=2.jpg` | jolie | - | statistic |
| `b=jones-road-beauty_vf=founder.mp4` | jones-road-beauty | - | founder |
| `b=jones-road-beauty_vf=instagram-text-overlay.jpeg` | jones-road-beauty | - | instagram-text-overlay |
| `b=jones-road-beauty_vf=letter.jpeg` | jones-road-beauty | - | letter |
| `b=juniper_vf=ad-in-the-wild.jpg` | juniper | - | ad-in-the-wild |
| `b=kitsch_vf=post-it.mp4` | kitsch | - | post-it |
| `b=kosas_vf=founder.mp4` | kosas | - | founder |
| `b=laseraway_vf=instagram-text-overlay.jpeg` | laseraway | - | instagram-text-overlay |
| `b=loop_vf=comment-response.jpg` | loop | - | comment-response |
| `b=loop_vf=flyer_vf=meme.jpg` | loop | - | flyer + meme |
| `b=loop_vf=greenscreen.mp4` | loop | - | greenscreen |
| `b=loop_vf=instagram-text-overlay.jpg` | loop | - | instagram-text-overlay |
| `b=loop_vf=meme.jpg` | loop | - | meme |
| `b=loop_vf=street-interview.mp4` | loop | - | street-interview |
| `b=lume-deodorant_vf=instagram-text-overlay.jpeg` | lume-deodorant | - | instagram-text-overlay |
| `b=lume-deodorant_vf=letter.jpeg` | lume-deodorant | - | letter |
| `b=lyka_vf=greenscreen.mp4` | lyka | - | greenscreen |
| `b=lyka_vf=letter.jpg` | lyka | - | letter |
| `b=lyka_vf=us-vs-them.jpeg` | lyka | - | us-vs-them |
| `b=magic-mind_vf=sign.jpg` | magic-mind | - | sign |
| `b=marpipe_vf=letter.jpeg` | marpipe | - | letter |
| `b=meller_vf=instagram-text-overlay.jpeg` | meller | - | instagram-text-overlay |
| `b=menofmanual_vf=before-and-after.jpg` | menofmanual | - | before-and-after |
| `b=menofmanual_vf=feature-benefit-pointout.jpeg` | menofmanual | - | feature-benefit-pointout |
| `b=merit_vf=listicle.jpg` | merit | - | listicle |
| `b=misfits-market_vf=founder_vf=behind-the-scenes.mp4` | misfits-market | - | founder + behind-the-scenes |
| `b=misfits-market_vf=instagram-text-overlay.jpeg` | misfits-market | - | instagram-text-overlay |
| `b=momcozy_vf=yapper.mp4` | momcozy | - | yapper |
| `b=monday-haircare_vf=press.jpeg` | monday-haircare | - | press |
| `b=moon-juice_vf=before-and-after.jpg` | moon-juice | - | before-and-after |
| `b=moon-magic_vf=comment-response.png` | moon-magic | - | comment-response |
| `b=mott-and-bow_vf=comment-screenshot.jpg` | mott-and-bow | - | comment-screenshot |
| `b=mott-and-bow_vf=post-it.jpeg` | mott-and-bow | - | post-it |
| `b=mous_vf=high-craft-edit.mp4` | mous | - | high-craft-edit |
| `b=mud-wtr_vf=founder.mp4` | mud-wtr | - | founder |
| `b=nanit_vf=post-it.mp4` | nanit | - | post-it |
| `b=native-pet_vf=greenscreen.mp4` | native-pet | - | greenscreen |
| `b=natural-cycles_vf=instagram-text-overlay.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_vf=instagram-text-overlay_n=2.jpeg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_vf=instagram-text-overlay_n=3.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_vf=instagram-text-overlay_n=4.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=nestig_vf=comment-response.jpeg` | nestig | - | comment-response |
| `b=nutrafol-men_vf=before-and-after.jpg` | nutrafol-men | - | before-and-after |
| `b=oats-overnight_vf=founder.mp4` | oats-overnight | - | founder |
| `b=o-positiv_vf=post-it.jpg` | o-positiv | - | post-it |
| `b=orgain_vf=toggle.jpg` | orgain | - | toggle |
| `b=our-place_vf=letter.jpeg` | our-place | - | letter |
| `b=pehr_vf=instagram-text-overlay.jpeg` | pehr | - | instagram-text-overlay |
| `b=pela-case_vf=founder.mp4` | pela-case | - | founder |
| `b=primally-pure-skincare_vf=before-and-after.jpg` | primally-pure-skincare | - | before-and-after |
| `b=prose_vf=before-and-after_vf=listicle.mp4` | prose | - | before-and-after + listicle |
| `b=prose_vf=letter.jpeg` | prose | - | letter |
| `b=purple_vf=letter.jpeg` | purple | - | letter |
| `b=purple_vf=us-vs-them.jpeg` | purple | - | us-vs-them |
| `b=rheal_vf=post-it.mp4` | rheal | - | post-it |
| `b=rough-country_vf=asmr_vf=unboxing.mp4` | rough-country | - | asmr + unboxing |
| `b=runna_vf=post-it.mp4` | runna | - | post-it |
| `b=saie-beauty_vf=press.jpg` | saie-beauty | - | press |
| `b=scentbird_vf=post-it.mp4` | scentbird | - | post-it |
| `b=smol_vf=post-it.mp4` | smol | - | post-it |
| `b=solderstick_vf=instagram-text-overlay.jpeg` | solderstick | - | instagram-text-overlay |
| `b=solderstick_vf=us-vs-them.jpeg` | solderstick | - | us-vs-them |
| `b=spacegoods_vf=instagram-text-overlay.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_vf=instagram-text-overlay_n=2.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_vf=instagram-text-overlay_n=3.mp4` | spacegoods | - | instagram-text-overlay |
| `b=suri_vf=instagram-text-overlay.jpeg` | suri | - | instagram-text-overlay |
| `b=suri_vf=press.jpeg` | suri | - | press |
| `b=the-farmers-dog_vf=feature-benefit-pointout.jpeg` | the-farmers-dog | - | feature-benefit-pointout |
| `b=the-farmers-dog_vf=post-it.jpeg` | the-farmers-dog | - | post-it |
| `b=the-oodie_vf=us-vs-them.jpg` | the-oodie | - | us-vs-them |
| `b=thrive-causemetics_vf=comment-response.jpeg` | thrive-causemetics | - | comment-response |
| `b=thrive-causemetics_vf=instagram-text-overlay.jpeg` | thrive-causemetics | - | instagram-text-overlay |
| `b=thrive-causemetics_vf=post-it.jpeg` | thrive-causemetics | - | post-it |
| `b=timeline-longevity_vf=instagram-text-overlay.mp4` | timeline-longevity | - | instagram-text-overlay |
| `b=timeline-longevity_vf=press.jpeg` | timeline-longevity | - | press |
| `b=timeline-longevity_vf=us-vs-them.jpeg` | timeline-longevity | - | us-vs-them |
| `b=trade_vf=comment-response_vf=us-vs-them.jpg` | trade | - | comment-response + us-vs-them |
| `b=trade_vf=instagram-text-overlay.jpeg` | trade | - | instagram-text-overlay |
| `b=vitable_vf=post-it.jpeg` | vitable | - | post-it |
| `b=vrbo_vf=whiteboard.mp4` | vrbo | - | whiteboard |
| `b=wild-nutrition_vf=us-vs-them.jpeg` | wild-nutrition | - | us-vs-them |
| `b=winona_vf=comment-response.jpg` | winona | - | comment-response |
| `b=your-heights_vf=sign.jpg` | your-heights | - | sign |
| `b=your-heights_vf=us-vs-them.jpeg` | your-heights | - | us-vs-them |
| `b=your-heights_vf=yapper.mp4` | your-heights | - | yapper |
| `c=livrollings_vf=face-peeking-into-bottom-of-frame.jpg` | - | livrollings | face-peeking-into-bottom-of-frame |
| `c=oren-john_vf=graphic-anchor_vf=listicle.mp4` | - | oren-john | graphic-anchor + listicle |
| `b=happy-mammoth_vf=before-and-after_vf=ai-generated-static.jpg` | happy-mammoth | - | before-and-after + ai-generated-static |
| `b=natural-cycles_vf=line-chart.jpg` | natural-cycles | - | line-chart |
| `b=happy-mammoth_vf=ai-animation.mp4` | happy-mammoth | - | ai-animation |
| `b=buoy_vf=podcast.mp4` | buoy | - | podcast |
| `b=seed_vf=whiteboard.mp4` | seed | - | whiteboard |
| `b=surreal_vf=behind-the-scenes.mp4` | surreal | - | behind-the-scenes |
| `b=huel_vf=explainer.mp4` | huel | - | explainer |
| `b=o-positiv_vf=listicle.jpg` | o-positiv | - | listicle |
| `c=tesspagel_vf=graphic-anchor.mp4` | - | tesspagel | graphic-anchor |
| `b=ryze_vf=annotation.mp4` | ryze | - | annotation |
| `b=o-positiv_vf=review.jpg` | o-positiv | - | review |
| `b=hydrant_vf=ai-generated-static.jpg` | hydrant | - | ai-generated-static |
| `b=hydrant_vf=line-chart.jpg` | hydrant | - | line-chart |
| `b=headspace_vf=ad-in-the-wild.jpg` | headspace | - | ad-in-the-wild |
| `b=hers_vf=review.jpg` | hers | - | review |
| `b=hers_vf=ad-in-the-wild.jpg` | hers | - | ad-in-the-wild |
| `b=viome_vf=press.jpg` | viome | - | press |
| `b=buoy_vf=instagram-text-overlay.jpg` | buoy | - | instagram-text-overlay |
| `b=purdy-and-figg_vf=letter.jpg` | purdy-and-figg | - | letter |
| `b=hum-nutrition_vf=web-search.jpg` | hum-nutrition | - | web-search |
| `b=armra_vf=web-search.jpg` | armra | - | web-search |
| `b=grove-collaborative_vf=news.jpg` | grove-collaborative | - | news |
| `b=lemme_vf=feature-benefit-callout.jpg` | lemme | - | feature-benefit-callout |
| `b=olipop_vf=asmr.mp4` | olipop | - | asmr |
| `b=olipop_vf=meme.jpeg` | olipop | - | meme |
| `b=mejuri_vf=product-grid.jpeg` | mejuri | - | product-grid |
| `b=made-in_vf=product-grid.jpg` | made-in | - | product-grid |
| `b=made-in_vf=bento-grid.jpg` | made-in | - | bento-grid |
| `b=vuori_vf=bento-grid.jpeg` | vuori | - | bento-grid |
| `b=honour-health_vf=whiteboard.mp4` | honour-health | - | whiteboard |
| `c=siffhaider_vf=podcast_vf=founder.mp4` | - | siffhaider | podcast + founder |
| `b=alo-yoga_vf=bento-grid.jpg` | alo-yoga | - | bento-grid |
| `b=dose_vf=flyer.jpg` | dose | - | flyer |
| `b=armra_vf=letter.jpg` | armra | - | letter |
| `b=obvi_vf=whiteboard.jpg` | obvi | - | whiteboard |
| `b=onnit_vf=venn-diagram_vf=whiteboard.jpg` | onnit | - | venn-diagram + whiteboard |
