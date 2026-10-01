# Evergreen example files — index

This folder holds every **year-round (evergreen)** example creative. Black Friday / Cyber Monday examples live in `../bfcm/`. Both use the same format definitions in `../../formats/`. Each ad lives **once**, no duplicate files.

## Naming convention

```
[b=<brand>][_c=<creator>]_s=evergreen_vf=<format>[_vf=<format2>].<ext>
```

At least one of `b=` or `c=` is required. Order is brand, then creator, then season, then visual format(s).

- **`b=`** brand, at most one. lowercase, dashes for spaces, strip punctuation, transliterate accents, `&` becomes `and`, keep the true spelling (`comfrt`, `mott-and-bow`, `the-farmers-dog`, `gruns`).
- **`c=`** creator handle, at most one. Same formatting rules as brand.
- **When to use which:**
  - Brand ad (no named creator): `b=<brand>` only.
  - Brand x creator partnership: include **both**, brand first: `b=<brand>_c=<creator>`.
  - Organic content or a creator-led post with no brand: `c=<creator>` only.
- **`s=`** season. Always `evergreen` in this folder (`bfcm` in `../bfcm/`).
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
| `b=actandacre_s=evergreen_vf=case-study.jpg` | actandacre | - | case-study |
| `b=agemate_s=evergreen_vf=post-it.jpeg` | agemate | - | post-it |
| `b=alo-yoga_s=evergreen_vf=bento-grid.jpg` | alo-yoga | - | bento-grid |
| `b=armra_s=evergreen_vf=ad-in-the-wild.jpg` | armra | - | ad-in-the-wild |
| `b=armra_s=evergreen_vf=web-search.jpg` | armra | - | web-search |
| `b=arrae_s=evergreen_vf=instagram-text-overlay.jpeg` | arrae | - | instagram-text-overlay |
| `b=arrae_s=evergreen_vf=whiteboard.jpg` | arrae | - | whiteboard |
| `b=atlas-coffee-club_s=evergreen_vf=post-it.mp4` | atlas-coffee-club | - | post-it |
| `b=atlas-coffee-club_s=evergreen_vf=text-message.jpg` | atlas-coffee-club | - | text-message |
| `b=babylist_s=evergreen_vf=comment-screenshot.jpg` | babylist | - | comment-screenshot |
| `b=barkbox_s=evergreen_vf=unexpected-text-placement.jpg` | barkbox | - | unexpected-text-placement |
| `b=barkbox_s=evergreen_vf=whiteboard.jpg` | barkbox | - | whiteboard |
| `b=betterhelp_s=evergreen_vf=post-it.mp4` | betterhelp | - | post-it |
| `b=billie_s=evergreen_vf=feature-benefit-pointout.jpeg` | billie | - | feature-benefit-pointout |
| `b=billie_s=evergreen_vf=instagram-text-overlay.jpeg` | billie | - | instagram-text-overlay |
| `b=bobbie_s=evergreen_vf=ad-in-the-wild.jpg` | bobbie | - | ad-in-the-wild |
| `b=bonafide_s=evergreen_vf=greenscreen.mp4` | bonafide | - | greenscreen |
| `b=bonafide_s=evergreen_vf=post-it.jpeg` | bonafide | - | post-it |
| `b=brooklinen_s=evergreen_vf=press.jpeg` | brooklinen | - | press |
| `b=buoy_s=evergreen_vf=founder.mp4` | buoy | - | founder |
| `b=buoy_s=evergreen_vf=instagram-text-overlay.jpg` | buoy | - | instagram-text-overlay |
| `b=buoy_s=evergreen_vf=podcast.mp4` | buoy | - | podcast |
| `b=buoy_s=evergreen_vf=taste-test_vf=yapper.mp4` | buoy | - | taste-test + yapper |
| `b=buoy_s=evergreen_vf=us-vs-them.jpg` | buoy | - | us-vs-them |
| `b=caraway_s=evergreen_vf=instagram-text-overlay.jpeg` | caraway | - | instagram-text-overlay |
| `b=caraway_s=evergreen_vf=letter.jpeg` | caraway | - | letter |
| `b=caraway_s=evergreen_vf=press.jpeg` | caraway | - | press |
| `b=caraway_s=evergreen_vf=us-vs-them.jpeg` | caraway | - | us-vs-them |
| `b=cartablet_s=evergreen_vf=press.jpeg` | cartablet | - | press |
| `b=clickup_s=evergreen_vf=instagram-text-overlay.jpeg` | clickup | - | instagram-text-overlay |
| `b=comfrt_s=evergreen_vf=comment-response.mp4` | comfrt | - | comment-response |
| `b=coterie-baby_s=evergreen_vf=feature-benefit-pointout.jpeg` | coterie-baby | - | feature-benefit-pointout |
| `b=current_s=evergreen_vf=post-it.mp4` | current | - | post-it |
| `b=dae_s=evergreen_vf=us-vs-them.jpeg` | dae | - | us-vs-them |
| `b=dedcool_s=evergreen_vf=founder.mp4` | dedcool | - | founder |
| `b=dermatica_s=evergreen_vf=instagram-text-overlay.jpeg` | dermatica | - | instagram-text-overlay |
| `b=divi_s=evergreen_vf=statistic.jpg` | divi | - | statistic |
| `b=dollar-shave-club_s=evergreen_vf=instagram-text-overlay.jpeg` | dollar-shave-club | - | instagram-text-overlay |
| `b=dose_s=evergreen_vf=creative-parking-lot_vf=fortune-cookie.jpg` | dose | - | creative-parking-lot + fortune-cookie |
| `b=dose_s=evergreen_vf=feature-benefit-pointout.jpeg` | dose | - | feature-benefit-pointout |
| `b=dose_s=evergreen_vf=flyer.jpg` | dose | - | flyer |
| `b=dose_s=evergreen_vf=whiteboard.jpg` | dose | - | whiteboard |
| `b=dose_s=evergreen_vf=whiteboard_n=2.mp4` | dose | - | whiteboard |
| `b=eight-sleep_s=evergreen_vf=listicle.mp4` | eight-sleep | - | listicle |
| `b=ergobaby_s=evergreen_vf=us-vs-them.jpeg` | ergobaby | - | us-vs-them |
| `b=everyday-dose_s=evergreen_vf=instagram-text-overlay.jpeg` | everyday-dose | - | instagram-text-overlay |
| `b=everyday-dose_s=evergreen_vf=skit.mp4` | everyday-dose | - | skit |
| `b=everyday-dose_s=evergreen_vf=yapper.mp4` | everyday-dose | - | yapper |
| `b=feel-goods_s=evergreen_vf=yapper.mp4` | feel-goods | - | yapper |
| `b=finalputt_s=evergreen_vf=press.jpeg` | finalputt | - | press |
| `b=fiverr_s=evergreen_vf=before-and-after.jpg` | fiverr | - | before-and-after |
| `b=flakes_s=evergreen_vf=founder.mp4` | flakes | - | founder |
| `b=flakes_s=evergreen_vf=post-it.jpeg` | flakes | - | post-it |
| `b=girlfriend-collective_s=evergreen_vf=press.jpeg` | girlfriend-collective | - | press |
| `b=glossier_s=evergreen_vf=yapper.mp4` | glossier | - | yapper |
| `b=gousto_s=evergreen_vf=instagram-text-overlay.jpeg` | gousto | - | instagram-text-overlay |
| `b=grove-collaborative_s=evergreen_vf=greenscreen_vf=listicle.mp4` | grove-collaborative | - | greenscreen + listicle |
| `b=grove-collaborative_s=evergreen_vf=news.jpg` | grove-collaborative | - | news |
| `b=gruns_s=evergreen_vf=comment-response.jpg` | gruns | - | comment-response |
| `b=gruns_s=evergreen_vf=text-message.jpg` | gruns | - | text-message |
| `b=gruns_s=evergreen_vf=unexpected-text-placement.jpg` | gruns | - | unexpected-text-placement |
| `b=gruns_s=evergreen_vf=us-vs-them.jpeg` | gruns | - | us-vs-them |
| `b=happy-mammoth_s=evergreen_vf=ai-animation.mp4` | happy-mammoth | - | ai-animation |
| `b=happy-mammoth_s=evergreen_vf=before-and-after.jpg` | happy-mammoth | - | before-and-after |
| `b=happy-mammoth_s=evergreen_vf=letter.jpeg` | happy-mammoth | - | letter |
| `b=happy-mammoth_s=evergreen_vf=post-it.jpeg` | happy-mammoth | - | post-it |
| `b=happy-mammoth_s=evergreen_vf=unexpected-text-placement.jpg` | happy-mammoth | - | unexpected-text-placement |
| `b=harrys_s=evergreen_vf=comment-screenshot.jpg` | harrys | - | comment-screenshot |
| `b=headspace_s=evergreen_vf=ad-in-the-wild.jpg` | headspace | - | ad-in-the-wild |
| `b=hers_s=evergreen_vf=ad-in-the-wild.jpg` | hers | - | ad-in-the-wild |
| `b=hers_s=evergreen_vf=review.jpg` | hers | - | review |
| `b=hexclad_s=evergreen_vf=post-it.mp4` | hexclad | - | post-it |
| `b=hims_s=evergreen_vf=comment-response.jpg` | hims | - | comment-response |
| `b=hinge_s=evergreen_vf=yapper.mp4` | hinge | - | yapper |
| `b=honeylove_s=evergreen_vf=ad-in-the-wild.jpg` | honeylove | - | ad-in-the-wild |
| `b=honeylove_s=evergreen_vf=ai-animation.mp4` | honeylove | - | ai-animation |
| `b=honeylove_s=evergreen_vf=comment-response.jpg` | honeylove | - | comment-response |
| `b=honeylove_s=evergreen_vf=flowchart.jpg` | honeylove | - | flowchart |
| `b=honeylove_s=evergreen_vf=instagram-text-overlay.jpg` | honeylove | - | instagram-text-overlay |
| `b=honeylove_s=evergreen_vf=matching-chart.jpg` | honeylove | - | matching-chart |
| `b=honour-health_s=evergreen_vf=whiteboard.mp4` | honour-health | - | whiteboard |
| `b=huda-beauty_s=evergreen_vf=asmr_vf=unboxing.mp4` | huda-beauty | - | asmr + unboxing |
| `b=huel_s=evergreen_vf=explainer.mp4` | huel | - | explainer |
| `b=huel_s=evergreen_vf=letter.jpeg` | huel | - | letter |
| `b=hum-nutrition_s=evergreen_vf=web-search.jpg` | hum-nutrition | - | web-search |
| `b=hydrant_s=evergreen_vf=line-chart.jpg` | hydrant | - | line-chart |
| `b=hydrant_s=evergreen_vf=post-it.jpeg` | hydrant | - | post-it |
| `b=hydrant_s=evergreen_vf=unexpected-text-placement.jpg` | hydrant | - | unexpected-text-placement |
| `b=ilia-beauty_s=evergreen_vf=behind-the-scenes.mp4` | ilia-beauty | - | behind-the-scenes |
| `b=infinity-hoop_s=evergreen_vf=us-vs-them.jpeg` | infinity-hoop | - | us-vs-them |
| `b=instant-hydration_s=evergreen_vf=letter.jpeg` | instant-hydration | - | letter |
| `b=instant-hydration_s=evergreen_vf=skit.mp4` | instant-hydration | - | skit |
| `b=intelligent-change_s=evergreen_vf=instagram-text-overlay.jpeg` | intelligent-change | - | instagram-text-overlay |
| `b=javvy_s=evergreen_vf=comment-response_vf=behind-the-scenes.mp4` | javvy | - | comment-response + behind-the-scenes |
| `b=javvy_s=evergreen_vf=notes-app.jpg` | javvy | - | notes-app |
| `b=javvy_s=evergreen_vf=whiteboard.jpg` | javvy | - | whiteboard |
| `b=jcrew_s=evergreen_vf=flatlay.jpg` | jcrew | - | flatlay |
| `b=jenny-bird_s=evergreen_vf=instagram-text-overlay.jpeg` | jenny-bird | - | instagram-text-overlay |
| `b=jolie_s=evergreen_vf=statistic.jpg` | jolie | - | statistic |
| `b=jolie_s=evergreen_vf=statistic_n=2.jpg` | jolie | - | statistic |
| `b=jones-road-beauty_s=evergreen_vf=founder.mp4` | jones-road-beauty | - | founder |
| `b=jones-road-beauty_s=evergreen_vf=instagram-text-overlay.jpeg` | jones-road-beauty | - | instagram-text-overlay |
| `b=jones-road-beauty_s=evergreen_vf=letter.jpeg` | jones-road-beauty | - | letter |
| `b=juniper_s=evergreen_vf=ad-in-the-wild.jpg` | juniper | - | ad-in-the-wild |
| `b=kitsch_s=evergreen_vf=post-it.mp4` | kitsch | - | post-it |
| `b=kitsch_s=evergreen_vf=skit.mp4` | kitsch | - | skit |
| `b=kosas_s=evergreen_vf=founder.mp4` | kosas | - | founder |
| `b=laseraway_s=evergreen_vf=instagram-text-overlay.jpeg` | laseraway | - | instagram-text-overlay |
| `b=lemme_s=evergreen_vf=feature-benefit-callout.jpg` | lemme | - | feature-benefit-callout |
| `b=little-caesars_c=jaredbuccii_s=evergreen_vf=skit.mp4` | little-caesars | jaredbuccii | skit |
| `b=loop_s=evergreen_vf=comment-response.jpg` | loop | - | comment-response |
| `b=loop_s=evergreen_vf=flyer.jpg` | loop | - | flyer |
| `b=loop_s=evergreen_vf=greenscreen.mp4` | loop | - | greenscreen |
| `b=loop_s=evergreen_vf=instagram-text-overlay.jpg` | loop | - | instagram-text-overlay |
| `b=loop_s=evergreen_vf=meme.jpg` | loop | - | meme |
| `b=loop_s=evergreen_vf=street-interview.mp4` | loop | - | street-interview |
| `b=lume-deodorant_s=evergreen_vf=instagram-text-overlay.jpeg` | lume-deodorant | - | instagram-text-overlay |
| `b=lume-deodorant_s=evergreen_vf=letter.jpeg` | lume-deodorant | - | letter |
| `b=lyka_s=evergreen_vf=greenscreen.mp4` | lyka | - | greenscreen |
| `b=lyka_s=evergreen_vf=letter.jpg` | lyka | - | letter |
| `b=lyka_s=evergreen_vf=us-vs-them.jpeg` | lyka | - | us-vs-them |
| `b=made-in_s=evergreen_vf=bento-grid.jpg` | made-in | - | bento-grid |
| `b=made-in_s=evergreen_vf=product-grid.jpg` | made-in | - | product-grid |
| `b=magic-mind_s=evergreen_vf=sign.jpg` | magic-mind | - | sign |
| `b=marpipe_s=evergreen_vf=letter.jpeg` | marpipe | - | letter |
| `b=mejuri_s=evergreen_vf=product-grid.jpeg` | mejuri | - | product-grid |
| `b=meller_s=evergreen_vf=instagram-text-overlay.jpeg` | meller | - | instagram-text-overlay |
| `b=menofmanual_s=evergreen_vf=before-and-after.jpg` | menofmanual | - | before-and-after |
| `b=menofmanual_s=evergreen_vf=feature-benefit-pointout.jpeg` | menofmanual | - | feature-benefit-pointout |
| `b=merit_s=evergreen_vf=feature-benefit-callout.jpg` | merit | - | feature-benefit-callout |
| `b=misfits-market_s=evergreen_vf=founder.mp4` | misfits-market | - | founder |
| `b=misfits-market_s=evergreen_vf=instagram-text-overlay.jpeg` | misfits-market | - | instagram-text-overlay |
| `b=momcozy_s=evergreen_vf=yapper.mp4` | momcozy | - | yapper |
| `b=monday-haircare_s=evergreen_vf=press.jpeg` | monday-haircare | - | press |
| `b=moon-juice_s=evergreen_vf=before-and-after.jpg` | moon-juice | - | before-and-after |
| `b=moon-magic_s=evergreen_vf=comment-response.png` | moon-magic | - | comment-response |
| `b=moonbrew_s=evergreen_vf=founder.mp4` | moonbrew | - | founder |
| `b=mott-and-bow_s=evergreen_vf=comment-screenshot.jpg` | mott-and-bow | - | comment-screenshot |
| `b=mott-and-bow_s=evergreen_vf=post-it.jpeg` | mott-and-bow | - | post-it |
| `b=mous_s=evergreen_vf=high-production-edit.mp4` | mous | - | high-production-edit |
| `b=mud-wtr_s=evergreen_vf=founder.mp4` | mud-wtr | - | founder |
| `b=nanit_s=evergreen_vf=found-footage_vf=post-it.mp4` | nanit | - | found-footage + post-it |
| `b=native-pet_s=evergreen_vf=greenscreen.mp4` | native-pet | - | greenscreen |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_n=2.jpeg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_n=3.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_n=4.jpg` | natural-cycles | - | instagram-text-overlay |
| `b=natural-cycles_s=evergreen_vf=line-chart.jpg` | natural-cycles | - | line-chart |
| `b=nestig_s=evergreen_vf=comment-response.jpeg` | nestig | - | comment-response |
| `b=nutrafol-men_s=evergreen_vf=before-and-after.jpg` | nutrafol-men | - | before-and-after |
| `b=o-positiv_s=evergreen_vf=asmr_vf=unboxing.mp4` | o-positiv | - | asmr + unboxing |
| `b=o-positiv_s=evergreen_vf=feature-benefit-callout.jpg` | o-positiv | - | feature-benefit-callout |
| `b=o-positiv_s=evergreen_vf=post-it.jpg` | o-positiv | - | post-it |
| `b=o-positiv_s=evergreen_vf=review.jpg` | o-positiv | - | review |
| `b=oats-overnight_s=evergreen_vf=founder.mp4` | oats-overnight | - | founder |
| `b=obvi_s=evergreen_vf=whiteboard.jpg` | obvi | - | whiteboard |
| `b=olipop_s=evergreen_vf=asmr.mp4` | olipop | - | asmr |
| `b=olipop_s=evergreen_vf=meme.jpeg` | olipop | - | meme |
| `b=onnit_s=evergreen_vf=venn-diagram_vf=whiteboard.jpg` | onnit | - | venn-diagram + whiteboard |
| `b=orgain_s=evergreen_vf=toggle.jpg` | orgain | - | toggle |
| `b=our-place_s=evergreen_vf=letter.jpeg` | our-place | - | letter |
| `b=pehr_s=evergreen_vf=instagram-text-overlay.jpeg` | pehr | - | instagram-text-overlay |
| `b=pela-case_s=evergreen_vf=founder.mp4` | pela-case | - | founder |
| `b=primally-pure-skincare_s=evergreen_vf=before-and-after.jpg` | primally-pure-skincare | - | before-and-after |
| `b=prose_s=evergreen_vf=before-and-after_vf=listicle.mp4` | prose | - | before-and-after + listicle |
| `b=prose_s=evergreen_vf=letter.jpeg` | prose | - | letter |
| `b=purdy-and-figg_s=evergreen_vf=letter.jpg` | purdy-and-figg | - | letter |
| `b=purple_s=evergreen_vf=letter.jpeg` | purple | - | letter |
| `b=purple_s=evergreen_vf=us-vs-them.jpeg` | purple | - | us-vs-them |
| `b=rheal_s=evergreen_vf=post-it.mp4` | rheal | - | post-it |
| `b=rough-country_s=evergreen_vf=asmr_vf=unboxing.mp4` | rough-country | - | asmr + unboxing |
| `b=runna_s=evergreen_vf=post-it.mp4` | runna | - | post-it |
| `b=ryze_s=evergreen_vf=creative-parking-lot_vf=annotation.mp4` | ryze | - | creative-parking-lot + annotation |
| `b=saie-beauty_s=evergreen_vf=press.jpg` | saie-beauty | - | press |
| `b=scentbird_s=evergreen_vf=post-it.mp4` | scentbird | - | post-it |
| `b=seed_s=evergreen_vf=whiteboard.mp4` | seed | - | whiteboard |
| `b=smol_s=evergreen_vf=post-it.mp4` | smol | - | post-it |
| `b=solawave_s=evergreen_vf=yapper_vf=graphic-anchor.mp4` | solawave | - | yapper + graphic-anchor |
| `b=solderstick_s=evergreen_vf=instagram-text-overlay.jpeg` | solderstick | - | instagram-text-overlay |
| `b=solderstick_s=evergreen_vf=us-vs-them.jpeg` | solderstick | - | us-vs-them |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_n=2.jpg` | spacegoods | - | instagram-text-overlay |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_n=3.mp4` | spacegoods | - | instagram-text-overlay |
| `b=suri_s=evergreen_vf=instagram-text-overlay.jpeg` | suri | - | instagram-text-overlay |
| `b=suri_s=evergreen_vf=press.jpeg` | suri | - | press |
| `b=surreal_s=evergreen_vf=behind-the-scenes.mp4` | surreal | - | behind-the-scenes |
| `b=the-farmers-dog_s=evergreen_vf=feature-benefit-pointout.jpeg` | the-farmers-dog | - | feature-benefit-pointout |
| `b=the-farmers-dog_s=evergreen_vf=post-it.jpeg` | the-farmers-dog | - | post-it |
| `b=the-oodie_s=evergreen_vf=us-vs-them.jpg` | the-oodie | - | us-vs-them |
| `b=thrive-causemetics_s=evergreen_vf=comment-response.jpeg` | thrive-causemetics | - | comment-response |
| `b=thrive-causemetics_s=evergreen_vf=instagram-text-overlay.jpeg` | thrive-causemetics | - | instagram-text-overlay |
| `b=thrive-causemetics_s=evergreen_vf=post-it.jpeg` | thrive-causemetics | - | post-it |
| `b=timeline-longevity_s=evergreen_vf=instagram-text-overlay.mp4` | timeline-longevity | - | instagram-text-overlay |
| `b=timeline-longevity_s=evergreen_vf=press.jpeg` | timeline-longevity | - | press |
| `b=timeline-longevity_s=evergreen_vf=us-vs-them.jpeg` | timeline-longevity | - | us-vs-them |
| `b=trade_s=evergreen_vf=comment-response_vf=us-vs-them.jpg` | trade | - | comment-response + us-vs-them |
| `b=trade_s=evergreen_vf=instagram-text-overlay.jpeg` | trade | - | instagram-text-overlay |
| `b=viome_s=evergreen_vf=press.jpg` | viome | - | press |
| `b=vitable_s=evergreen_vf=post-it.jpeg` | vitable | - | post-it |
| `b=vrbo_s=evergreen_vf=whiteboard.mp4` | vrbo | - | whiteboard |
| `b=vuori_s=evergreen_vf=bento-grid.jpeg` | vuori | - | bento-grid |
| `b=wild-nutrition_s=evergreen_vf=us-vs-them.jpeg` | wild-nutrition | - | us-vs-them |
| `b=winona_s=evergreen_vf=comment-response.jpg` | winona | - | comment-response |
| `b=your-heights_s=evergreen_vf=sign.jpg` | your-heights | - | sign |
| `b=your-heights_s=evergreen_vf=us-vs-them.jpeg` | your-heights | - | us-vs-them |
| `b=your-heights_s=evergreen_vf=yapper.mp4` | your-heights | - | yapper |
