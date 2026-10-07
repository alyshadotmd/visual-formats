# BFCM example files — index

This folder holds every **Black Friday / Cyber Monday** example creative, tagged `s=bfcm`. Year-round examples live in
`../evergreen/`. Both use the same format definitions in `../../formats/`. Each ad lives **once**. Launch date, media URL and Meta ad ID
for each ad are in the brand's `creative-ids.md` in the swipe file; tag notes are in the table below.

Moved here on 2026-09-30 from the Black Friday swipe file project (`/agent/brain/black-friday-swipe-file/`), which keeps
the project docs: brand tracker, offer taxonomy (the `ot` offer-type rules; one offer tag only since 2026-10-01), per-brand notes, creative ids, and the tagging tool.

**Tag status:** formats for Act + Acre, AG1, Arrae, Beis, Billie, Buoy and Caraway are approved. Alysha is doing the final
pass on the rest, so treat their `vf=` tags as not final yet.

## Naming convention

```
b=<brand>_s=bfcm_vf=<format>[_vf=<format2>]_ot=<offer type>[...]_dt=<discount type>[...]_oc=<offer condition>[...]_id=<Motion creative ID>.<ext>
```

- `b=` brand, `s=bfcm` season, `vf=` 1-2 formats (primary first; value is the format folder name, or `other` with a Tag note).
- `ot=` / `dt=` / `oc=` offer tags, rules in the swipe file's `offer-taxonomy.md`. `ot=none` carries no `dt`/`oc`.
- `id=` Motion creative ID, which keeps names unique.
- To change tags, use the swipe file's `_pipeline/apply-tags.py`; it renames the media and rebuilds this table (tag notes are kept here).

## Files (272)

| File | Brand | Visual format(s) | Offer type | Tag note |
|---|---|---|---|---|
| `b=actandacre_s=bfcm_vf=bento-grid_ot=amount-off_id=691d891ee400180cbdafd3f0.jpeg` | actandacre | bento-grid | amount-off | - |
| `b=actandacre_s=bfcm_vf=bento-grid_ot=amount-off_id=691d891ee400180cbdafd407.jpeg` | actandacre | bento-grid | amount-off | - |
| `b=actandacre_s=bfcm_vf=collage_ot=none_id=691d891ee400180cbdafd3ec.jpeg` | actandacre | collage | none | - |
| `b=actandacre_s=bfcm_vf=collage_ot=none_id=691d891ee400180cbdafd3fb.jpeg` | actandacre | collage | none | - |
| `b=actandacre_s=bfcm_vf=comment-response_ot=amount-off_id=69252630e400180cbd9ac923.mp4` | actandacre | comment-response | amount-off | - |
| `b=actandacre_s=bfcm_vf=comment-response_ot=amount-off_id=69252630e400180cbd9ac933.mp4` | actandacre | comment-response | amount-off | - |
| `b=actandacre_s=bfcm_vf=flatlay_ot=amount-off_id=691d891ee400180cbdafd3fd.jpeg` | actandacre | flatlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=flatlay_ot=amount-off_id=691d891ee400180cbdafd41a.jpeg` | actandacre | flatlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=69252630e400180cbd9ac927.jpeg` | actandacre | instagram-text-overlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=other_ot=amount-off_id=69252630e400180cbd9ac924.jpeg` | actandacre | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=actandacre_s=bfcm_vf=other_ot=amount-off_id=69252630e400180cbd9ac93b.jpeg` | actandacre | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=actandacre_s=bfcm_vf=shelfie_ot=amount-off_id=691d891ee400180cbdafd406.jpeg` | actandacre | shelfie | amount-off | - |
| `b=actandacre_s=bfcm_vf=text-alert_ot=amount-off_id=691d891ee400180cbdafd413.mp4` | actandacre | text-alert | amount-off | - |
| `b=actandacre_s=bfcm_vf=text-echo_ot=amount-off_id=691d891ee400180cbdafd41b.jpeg` | actandacre | text-echo | amount-off | - |
| `b=actandacre_s=bfcm_vf=transformation_ot=amount-off_id=691e35f1e400180cbdb19e07.mp4` | actandacre | transformation | amount-off | - |
| `b=ag1_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift_id=6921ed02e400180cbda854a1.mp4` | ag1 | b-roll-overlay | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=69208b63e400180cbd743280.jpeg` | ag1 | instagram-text-overlay | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=69286620e400180cbdc262c8.jpeg` | ag1 | instagram-text-overlay | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=6929d226e400180cbd2a502f.jpeg` | ag1 | instagram-text-overlay | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=692d8d1be400180cbdbd205b.jpeg` | ag1 | instagram-text-overlay | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=free-gift_id=69260255e400180cbdfc278c.jpeg` | ag1 | instagram-text-overlay | free-gift | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off_id=69286620e400180cbdc262b0.jpeg` | ag1 | offer-banner | amount-off | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off_id=692bf41be400180cbdd93ee8.jpeg` | ag1 | offer-banner | amount-off | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=69209b28e400180cbda9e641.jpeg` | ag1 | offer-banner | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=product-animation_vf=offer-banner_ot=free-gift_id=6921ed02e400180cbda854d8.mp4` | ag1 | product-animation + offer-banner | free-gift | - |
| `b=ag1_s=bfcm_vf=product-grid_ot=free-gift_id=6921ed02e400180cbda854da.mp4` | ag1 | product-grid | free-gift | - |
| `b=ag1_s=bfcm_vf=product-grid_ot=free-gift_id=692bf41be400180cbdd93eef.jpeg` | ag1 | product-grid | free-gift | - |
| `b=ag1_s=bfcm_vf=text-echo_ot=amount-off_ot=free-gift_id=691f0936e400180cbd03351b.jpeg` | ag1 | text-echo | amount-off + free-gift | - |
| `b=ag1_s=bfcm_vf=ugc_ot=bundle_ot=free-gift_id=69286620e400180cbdc262e7.mp4` | ag1 | ugc | bundle + free-gift | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=692066cce400180cbd052f10.jpeg` | arrae | instagram-text-overlay | amount-off | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=692bac48e400180cbd4cb61e.jpeg` | arrae | instagram-text-overlay | amount-off | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=none_id=69231bb9e400180cbd8963bf.mp4` | arrae | instagram-text-overlay | none | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=none_id=69281ec9e400180cbd09c5c5.mp4` | arrae | instagram-text-overlay | none | - |
| `b=arrae_s=bfcm_vf=notes-app_vf=flatlay_ot=none_id=69231bb9e400180cbd8963be.jpeg` | arrae | notes-app + flatlay | none | - |
| `b=arrae_s=bfcm_vf=offer-banner_ot=amount-off_id=692066cce400180cbd052f1b.jpeg` | arrae | offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=offer-banner_ot=tiered_id=6929a995e400180cbd82741d.jpeg` | arrae | offer-banner | tiered | Offer: tiered spend discount works for everyone; subscribing adds an extra 10%, so the condition is None (subscription is a bonus, not required). |
| `b=arrae_s=bfcm_vf=other_ot=amount-off_id=692066cce400180cbd052f2d.jpeg` | arrae | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=arrae_s=bfcm_vf=product-animation_ot=none_id=6929a995e400180cbd8273fb.mp4` | arrae | product-animation | none | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=692066cce400180cbd052f2b.mp4` | arrae | product-animation + offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=692bac48e400180cbd4cb631.mp4` | arrae | product-animation + offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=tiered_id=6929a995e400180cbd82740d.mp4` | arrae | product-animation + offer-banner | tiered | Offer: tiered spend discount works for everyone; subscribing adds an extra 10%, so the condition is None (subscription is a bonus, not required). |
| `b=arrae_s=bfcm_vf=product-grid_ot=none_id=6929a995e400180cbd827413.jpeg` | arrae | product-grid | none | - |
| `b=arrae_s=bfcm_vf=shelfie_ot=none_id=6929a995e400180cbd827409.jpeg` | arrae | shelfie | none | - |
| `b=arrae_s=bfcm_vf=yapper_ot=amount-off_id=692bac48e400180cbd4cb62e.mp4` | arrae | yapper | amount-off | - |
| `b=arrae_s=bfcm_vf=yapper_ot=amount-off_ot=bundle_id=692bac48e400180cbd4cb62d.mp4` | arrae | yapper | amount-off + bundle | - |
| `b=beis_s=bfcm_vf=greenscreen_ot=amount-off_id=692aa31be400180cbdcef162.mp4` | beis | greenscreen | amount-off | - |
| `b=billie_s=bfcm_vf=collage_ot=amount-off_id=6927a54ce400180cbdee973e.jpeg` | billie | collage | amount-off | - |
| `b=billie_s=bfcm_vf=comment-response_ot=none_id=6927a54ce400180cbdee9742.jpeg` | billie | comment-response | none | - |
| `b=billie_s=bfcm_vf=product-grid_ot=none_id=6915fcace4c6e2f6bc572be8.jpeg` | billie | product-grid | none | Alysha (Sept 30 2026): product-grid, but a very creative one; each product card is styled as a coupon with a barcode. |
| `b=billie_s=bfcm_vf=receipt_ot=amount-off_id=6915fcace4c6e2f6bc572bef.jpeg` | billie | receipt | amount-off | - |
| `b=buoy_s=bfcm_vf=founder_ot=amount-off_ot=free-gift_id=6927448ee400180cbd97c4d6.mp4` | buoy | founder | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=69213b25e400180cbd943e38.jpeg` | buoy | instagram-text-overlay | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=692cdd41e400180cbdd4a044.jpeg` | buoy | instagram-text-overlay | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=live-selling_ot=amount-off_ot=free-gift_id=692cdd42e400180cbdd4a050.mp4` | buoy | live-selling | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_id=691fcbf0e400180cbd75794b.jpeg` | buoy | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=69137d102d77ca559d69a66d.jpeg` | buoy | offer-banner | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=69137d102d77ca559d69a673.jpeg` | buoy | offer-banner | amount-off + free-gift | Alysha (Sept 30 2026): torn with listicle because of the bundle list, but the offer ('The best deal on Buoy, ever / 43% off + 4 free gifts') is the hero, so offer-banner; the list supports the offer. |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=692cdd42e400180cbdd4a04b.jpeg` | buoy | offer-banner | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift_id=692adc02e400180cbd5e7a14.jpeg` | buoy | product-grid | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_id=69255af8e400180cbd0c87f7.mp4` | buoy | ugc-mashup | amount-off + free-gift | - |
| `b=buoy_s=bfcm_vf=ugc_ot=amount-off_id=69293da2e400180cbdca6f7f.mp4` | buoy | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=founder_ot=none_id=6925db91e400180cbd5ea57a.mp4` | caraway | founder | none | - |
| `b=caraway_s=bfcm_vf=interview_ot=amount-off_id=6927e604e400180cbd8cd3c2.mp4` | caraway | interview | amount-off | - |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_id=6925db92e400180cbd5ea66a.jpeg` | caraway | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_id=692988d1e400180cbd02f096.jpeg` | caraway | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_id=692b71dfe400180cbd99463e.jpeg` | caraway | offer-banner | amount-off | Alysha (Sept 30 2026): not a flatlay (no real-life setting). Product in a frame with a big struck-through price ($446 / $800) under 'Black Friday Savings', so offer-banner by the hero test. |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_id=692d387ae400180cbdc1c8c1.jpeg` | caraway | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_id=692eedcce400180cbd18c768.jpeg` | caraway | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=692988d1e400180cbd02f098.mp4` | caraway | product-animation + offer-banner | amount-off | - |
| `b=caraway_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=692eedcce400180cbd18c766.mp4` | caraway | product-animation + offer-banner | amount-off | - |
| `b=caraway_s=bfcm_vf=product-animation_vf=product-grid_ot=amount-off_id=6925db92e400180cbd5ea67b.mp4` | caraway | product-animation + product-grid | amount-off | - |
| `b=caraway_s=bfcm_vf=stop-motion_ot=amount-off_id=6925db92e400180cbd5ea679.mp4` | caraway | stop-motion | amount-off | - |
| `b=caraway_s=bfcm_vf=street-interview_ot=amount-off_id=6927e604e400180cbd8cd3ca.mp4` | caraway | street-interview | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_id=6925db91e400180cbd5ea146.mp4` | caraway | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_id=6925db91e400180cbd5ea555.mp4` | caraway | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_id=6925db92e400180cbd5ea67e.mp4` | caraway | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_id=6927e604e400180cbd8cd3d4.mp4` | caraway | ugc | amount-off | - |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none_id=691085292d77ca559ddafbc1.mp4` | comfrt | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none_id=6911bf4e2d77ca559d126fb5.mp4` | comfrt | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none_id=6916c0c6e4c6e2f6bc9b6e2a.mp4` | comfrt | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_vf=greenscreen_ot=amount-off_id=691085292d77ca559ddafbc0.mp4` | comfrt | comment-response + greenscreen | amount-off | Alysha review (Sept 30 2026): yapper changed to comment-response + greenscreen |
| `b=dae_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=691ec926e400180cbd629d23.jpeg` | dae | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): lifestyle photo with Instagram-style highlight text carrying the offer; suggested instagram-text-overlay instead of product-image. |
| `b=dae_s=bfcm_vf=offer-banner_vf=product-animation_ot=amount-off_id=69201cbfe400180cbd3d4342.mp4` | dae | offer-banner + product-animation | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner + product-animation |
| `b=dae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=69201cbfe400180cbd3d4346.mp4` | dae | product-animation + offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to product-animation + offer-banner |
| `b=dae_s=bfcm_vf=product-grid_ot=amount-off_id=6926eebfe400180cbd9ebe7e.mp4` | dae | product-grid | amount-off | - |
| `b=everydaydose_s=bfcm_vf=behind-the-scenes_ot=free-gift_id=6923a93ee400180cbd7ea1d9.mp4` | everydaydose | behind-the-scenes | free-gift | - |
| `b=everydaydose_s=bfcm_vf=comment-response_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae3a.mp4` | everydaydose | comment-response | amount-off + free-gift | - |
| `b=everydaydose_s=bfcm_vf=comment-response_vf=sign_ot=amount-off_ot=free-gift_id=6926a1e9e400180cbde2213f.mp4` | everydaydose | comment-response + sign | amount-off + free-gift | Alysha review (Sept 30 2026): comment-response changed to comment-response + sign |
| `b=everydaydose_s=bfcm_vf=comment-response_vf=whiteboard_ot=amount-off_ot=free-gift_id=6926ba0ee400180cbd185e2a.mp4` | everydaydose | comment-response + whiteboard | amount-off + free-gift | Alysha review (Sept 30 2026): whiteboard changed to comment-response + whiteboard |
| `b=everydaydose_s=bfcm_vf=egc_vf=yapper_ot=amount-off_ot=free-gift_id=6926ba0ee400180cbd185e31.mp4` | everydaydose | egc + yapper | amount-off + free-gift | Alysha review (Sept 30 2026): unboxing changed to egc + yapper |
| `b=everydaydose_s=bfcm_vf=greenscreen_ot=amount-off_ot=free-gift_id=6928fd06e400180cbde3e64b.mp4` | everydaydose | greenscreen | amount-off + free-gift | Alysha review (Sept 30 2026): yapper changed to greenscreen |
| `b=everydaydose_s=bfcm_vf=high-production-edit_ot=amount-off_ot=free-gift_id=6926ba0ee400180cbd185e1e.mp4` | everydaydose | high-production-edit | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to high-production-edit |
| `b=everydaydose_s=bfcm_vf=high-production-edit_ot=amount-off_ot=free-gift_id=6926ba0ee400180cbd185e2e.mp4` | everydaydose | high-production-edit | amount-off + free-gift | Alysha review (Sept 30 2026): unboxing changed to high-production-edit |
| `b=everydaydose_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_id=6926ba0ee400180cbd185e1b.jpeg` | everydaydose | instagram-text-overlay | amount-off + free-gift | Alysha review (Sept 30 2026): feature-benefit-pointout changed to instagram-text-overlay |
| `b=everydaydose_s=bfcm_vf=letter_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae52.jpeg` | everydaydose | letter | amount-off + free-gift | - |
| `b=everydaydose_s=bfcm_vf=listicle_ot=amount-off_ot=free-gift_id=6928fd06e400180cbde3e618.jpeg` | everydaydose | listicle | amount-off + free-gift | - |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=amount-off_id=6926a1e9e400180cbde22145.jpeg` | everydaydose | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=amount-off_id=6928fd06e400180cbde3e655.mp4` | everydaydose | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=6924fe23e400180cbd24b9af.jpeg` | everydaydose | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae19.jpeg` | everydaydose | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): product-grid changed to offer-banner |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae22.jpeg` | everydaydose | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=free-gift_id=692a59b1e400180cbd1fae27.jpeg` | everydaydose | offer-banner | free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everydaydose_s=bfcm_vf=offer-banner_ot=free-gift_id=692a59b1e400180cbd1fae48.jpeg` | everydaydose | offer-banner | free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everydaydose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift_id=6925071de400180cbd3db0ac.jpeg` | everydaydose | product-grid | amount-off + free-gift | - |
| `b=everydaydose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift_id=6926ba0de400180cbd185e10.jpeg` | everydaydose | product-grid | amount-off + free-gift | - |
| `b=everydaydose_s=bfcm_vf=sign_ot=amount-off_ot=free-gift_id=6926a1e9e400180cbde22138.mp4` | everydaydose | sign | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to sign |
| `b=everydaydose_s=bfcm_vf=text-message_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae4b.jpeg` | everydaydose | text-message | amount-off + free-gift | Alysha review (Sept 30 2026): comment-screenshot changed to text-message |
| `b=everydaydose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_id=6926ba0de400180cbd185e18.mp4` | everydaydose | ugc-mashup | amount-off + free-gift | Alysha review (Sept 30 2026): yapper changed to ugc-mashup |
| `b=everydaydose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_id=6928fd06e400180cbde3e637.mp4` | everydaydose | ugc-mashup | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=everydaydose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_id=692a59b1e400180cbd1fae2c.mp4` | everydaydose | ugc-mashup | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=everydaydose_s=bfcm_vf=venn-diagram_ot=none_id=6928fd06e400180cbde3e66a.jpeg` | everydaydose | venn-diagram | none | Alysha review (Sept 30 2026): other changed to venn-diagram |
| `b=everydaydose_s=bfcm_vf=whiteboard_vf=podcast_ot=amount-off_ot=free-gift_id=692c85fee400180cbd3295bd.mp4` | everydaydose | whiteboard + podcast | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to whiteboard + podcast |
| `b=everydaydose_s=bfcm_vf=yapper_ot=amount-off_ot=free-gift_id=692ffc9ce400180cbd2e753d.mp4` | everydaydose | yapper | amount-off + free-gift | - |
| `b=gruns_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=691fe6a3e400180cbdba8ff9.mp4` | gruns | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=gruns_s=bfcm_vf=cart-screenshot_ot=amount-off_id=69298e8be400180cbd193ba8.jpeg` | gruns | cart-screenshot | amount-off | Alysha review (Sept 30 2026): other changed to creative-parking-lot + cart-screenshot |
| `b=gruns_s=bfcm_vf=collage_ot=amount-off_id=6927f0d3e400180cbda3c1e0.jpeg` | gruns | collage | amount-off | Alysha review (Sept 30 2026): statistic changed to collage |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_id=690e97b52d77ca559ddfc10a.jpeg` | gruns | offer-banner | amount-off | Says over 50% off so tagged sitewide Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_id=691fe6a3e400180cbdba9003.jpeg` | gruns | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_id=69270ccae400180cbde96a3a.jpeg` | gruns | offer-banner | amount-off | Alysha review (Sept 30 2026): statistic changed to offer-banner |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_id=69270ccae400180cbde96a3f.jpeg` | gruns | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_id=6927f0d3e400180cbda3c1e1.jpeg` | gruns | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=press_ot=amount-off_id=69270ccae400180cbde96a3b.mp4` | gruns | press | amount-off | - |
| `b=gruns_s=bfcm_vf=street-interview_ot=amount-off_id=691e9505e400180cbdd53a65.mp4` | gruns | street-interview | amount-off | Alysha review (Sept 30 2026): other changed to street-interview |
| `b=gruns_s=bfcm_vf=ugc_ot=amount-off_id=69298e8be400180cbd193bbe.mp4` | gruns | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=gruns_s=bfcm_vf=us-vs-them_ot=none_id=69096fe42d77ca559da55cb0.jpeg` | gruns | us-vs-them | none | - |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off_id=6923517ce400180cbde17f4d.jpeg` | hexclad | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off_id=692dc91ee400180cbd6ae65b.mp4` | hexclad | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=692a016de400180cbdeb8457.mp4` | hexclad | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none_id=691736c9e4c6e2f6bcbe49bf.jpeg` | hexclad | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none_id=691736c9e4c6e2f6bcbe49e2.mp4` | hexclad | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none_id=691736cae4c6e2f6bcbe4a03.mp4` | hexclad | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=hexclad_s=bfcm_vf=post-it_ot=none_id=6921ffe6e400180cbdc5b2f2.jpeg` | hexclad | post-it | none | Runneth first pass (Sept 30 2026): a yellow sticky note reading 'Black Friday Sale' sits on the pan; suggested post-it instead of product-image. |
| `b=hexclad_s=bfcm_vf=text-alert_ot=amount-off_id=691736c9e4c6e2f6bcbe49d2.mp4` | hexclad | text-alert | amount-off | - |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_id=691736c8e4c6e2f6bcbe46d1.mp4` | hexclad | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_id=69208fd9e400180cbd84ef45.mp4` | hexclad | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_id=6924a4fbe400180cbdedef4d.mp4` | hexclad | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_id=692c38fee400180cbd7bd341.mp4` | hexclad | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc_ot=none_id=6928aeb5e400180cbdb720fe.mp4` | hexclad | ugc | none | Alysha review (Sept 30 2026): unboxing changed to ugc |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=690be4fd2d77ca559debe0a7.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=691e5cbae400180cbd3828cf.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=691fc12de400180cbd5059db.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=692720a8e400180cbd21e2cb.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=692abd20e400180cbd0df083.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_id=692abd20e400180cbd0df0af.mp4` | hommey | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off_id=690801b252ed4a2ffcd06b28.jpeg` | hommey | bento-grid | amount-off | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off_id=690801b252ed4a2ffcd06b2d.jpeg` | hommey | bento-grid | amount-off | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off_id=69292ee7e400180cbd968b87.mp4` | hommey | bento-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=692720a8e400180cbd21e25a.jpeg` | hommey | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): a personal note in story-style text over a lifestyle photo ('I almost missed this, but @hommey...'); suggested instagram-text-overlay instead of product-image. |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=69292ee7e400180cbd968b32.jpeg` | hommey | instagram-text-overlay | amount-off | Alysha review (Sept 30 2026): other changed to instagram-text-overlay |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=692ccb47e400180cbdb1a194.jpeg` | hommey | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): a personal note in story-style text over a lifestyle photo ('I almost missed this, but @hommey...'); suggested instagram-text-overlay instead of product-image. |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_id=6911011f2d77ca559dadbe53.jpeg` | hommey | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_id=692720a8e400180cbd21e258.jpeg` | hommey | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_id=69292ee7e400180cbd968b2b.mp4` | hommey | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_id=69292ee7e400180cbd968b40.mp4` | hommey | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner. Images swap at an even pace under a fixed offer (slideshow); slideshow is parked as a candidate format |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_id=692ccb47e400180cbdb1a1a3.jpeg` | hommey | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hommey_s=bfcm_vf=press_ot=amount-off_id=690be4fd2d77ca559debe059.jpeg` | hommey | press | amount-off | - |
| `b=hommey_s=bfcm_vf=product-animation_ot=amount-off_id=692ccb47e400180cbdb1a1a2.mp4` | hommey | product-animation | amount-off | Alysha review (Sept 30 2026): product-grid changed to product-animation |
| `b=hommey_s=bfcm_vf=product-animation_ot=none_id=6916a459e4c6e2f6bc5d5602.mp4` | hommey | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=hommey_s=bfcm_vf=product-animation_ot=none_id=6916a459e4c6e2f6bc5d5605.mp4` | hommey | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=hommey_s=bfcm_vf=product-grid_ot=amount-off_id=692abd20e400180cbd0df09b.jpeg` | hommey | product-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=product-grid_ot=amount-off_id=69306e3fe400180cbd5788b3.jpeg` | hommey | product-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=review_ot=amount-off_id=692abd20e400180cbd0df08a.jpeg` | hommey | review | amount-off | - |
| `b=hommey_s=bfcm_vf=shelfie_ot=amount-off_id=69306e3fe400180cbd5788ad.jpeg` | hommey | shelfie | amount-off | - |
| `b=hommey_s=bfcm_vf=swatch-picker_ot=amount-off_id=690e7c902d77ca559d6f9fc9.mp4` | hommey | swatch-picker | amount-off | Alysha review (Sept 30 2026): other changed to creative-parking-lot + swatch-picker |
| `b=honeylove_s=bfcm_vf=before-and-after_ot=amount-off_id=6921bee4e400180cbd669c7d.mp4` | honeylove | before-and-after | amount-off | Alysha review (Sept 30 2026): other changed to before-and-after |
| `b=honeylove_s=bfcm_vf=comment-response_vf=ugc-mashup_ot=amount-off_id=6929a4dfe400180cbd7073b3.mp4` | honeylove | comment-response + ugc-mashup | amount-off | Alysha review (Sept 30 2026): comment-response changed to comment-response + ugc-mashup |
| `b=honeylove_s=bfcm_vf=flatlay_ot=amount-off_id=691cef08e400180cbd464094.jpeg` | honeylove | flatlay | amount-off | - |
| `b=honeylove_s=bfcm_vf=flatlay_vf=offer-banner_ot=amount-off_id=6921beb3e400180cbd667b9f.mp4` | honeylove | flatlay + offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to flatlay + offer-banner |
| `b=honeylove_s=bfcm_vf=graphic-anchor_ot=amount-off_id=692954d6e400180cbd29b534.mp4` | honeylove | graphic-anchor | amount-off | Alysha review (Sept 30 2026): other changed to graphic-anchor |
| `b=honeylove_s=bfcm_vf=letter_ot=free-gift_id=69147c87101fc64da30aa483.jpeg` | honeylove | letter | free-gift | - |
| `b=honeylove_s=bfcm_vf=offer-banner_ot=amount-off_id=692d4874e400180cbdf61bec.jpeg` | honeylove | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=honeylove_s=bfcm_vf=product-animation_vf=offer-banner_ot=none_id=69205541e400180cbdcfdd74.mp4` | honeylove | product-animation + offer-banner | none | Alysha review (Sept 30 2026): offer-banner changed to product-animation + offer-banner |
| `b=honeylove_s=bfcm_vf=review_ot=amount-off_id=69277e88e400180cbd6042f9.jpeg` | honeylove | review | amount-off | Alysha review (Sept 30 2026): other changed to review |
| `b=honeylove_s=bfcm_vf=split-screen_ot=amount-off_id=6921bee4e400180cbd669c7b.mp4` | honeylove | split-screen | amount-off | Alysha review (Sept 30 2026): other changed to split-screen |
| `b=honeylove_s=bfcm_vf=split-screen_ot=amount-off_id=692954d6e400180cbd29b558.mp4` | honeylove | split-screen | amount-off | Alysha review (Sept 30 2026): listicle changed to split-screen |
| `b=honeylove_s=bfcm_vf=ugc-mashup_ot=amount-off_id=691eb276e400180cbd19aa89.mp4` | honeylove | ugc-mashup | amount-off | Alysha review (Sept 30 2026): whiteboard changed to ugc-mashup |
| `b=honeylove_s=bfcm_vf=ugc-mashup_ot=amount-off_id=6921beb3e400180cbd667ba1.mp4` | honeylove | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=honeylove_s=bfcm_vf=unboxing_ot=amount-off_id=692b0c5be400180cbdc52a4e.mp4` | honeylove | unboxing | amount-off | - |
| `b=javvy_s=bfcm_vf=asmr_ot=amount-off_ot=free-gift_id=692bb675e400180cbd63f3eb.mp4` | javvy | asmr | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to asmr |
| `b=javvy_s=bfcm_vf=asmr_ot=free-gift_id=692d64cee400180cbd468731.mp4` | javvy | asmr | free-gift | Alysha review (Sept 30 2026): other changed to asmr |
| `b=javvy_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift_id=692826d5e400180cbd20d6e7.mp4` | javvy | b-roll-overlay | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=javvy_s=bfcm_vf=challenge_ot=amount-off_id=6929aec0e400180cbd976c79.mp4` | javvy | challenge | amount-off | Alysha review (Sept 30 2026): other changed to challenge |
| `b=javvy_s=bfcm_vf=found-footage_vf=whiteboard_ot=amount-off_ot=free-gift_id=692bb675e400180cbd63f3a6.mp4` | javvy | found-footage + whiteboard | amount-off + free-gift | Alysha review (Sept 30 2026): skit changed to found-footage + whiteboard |
| `b=javvy_s=bfcm_vf=greenscreen_ot=amount-off_ot=free-gift_id=692d64cee400180cbd468509.mp4` | javvy | greenscreen | amount-off + free-gift | - |
| `b=javvy_s=bfcm_vf=letter_ot=amount-off_ot=free-gift_id=692d64cee400180cbd468825.jpeg` | javvy | letter | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to letter |
| `b=javvy_s=bfcm_vf=skit_ot=amount-off_ot=free-gift_id=692826d5e400180cbd20d6e9.mp4` | javvy | skit | amount-off + free-gift | - |
| `b=javvy_s=bfcm_vf=ugc_ot=amount-off_ot=free-gift_id=692826d5e400180cbd20d7be.mp4` | javvy | ugc | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to ugc |
| `b=javvy_s=bfcm_vf=ugc_ot=amount-off_ot=free-gift_id=692bb675e400180cbd63f49f.mp4` | javvy | ugc | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to ugc |
| `b=jolie_s=bfcm_vf=letter_ot=none_id=692abc5ee400180cbd0b9828.jpeg` | jolie | letter | none | Alysha review (Sept 30 2026): other changed to letter |
| `b=jolie_s=bfcm_vf=offer-banner_ot=amount-off_id=69198482e4c6e2f6bcd21302.jpeg` | jolie | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jolie_s=bfcm_vf=offer-banner_ot=amount-off_id=692abc5ee400180cbd0b988d.jpeg` | jolie | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=b-roll-overlay_ot=none_id=691b9391e400180cbd67dcc7.mp4` | jonesroadbeauty | b-roll-overlay | none | Alysha review (Sept 30 2026): ad-in-the-wild changed to b-roll-overlay |
| `b=jonesroadbeauty_s=bfcm_vf=b-roll-overlay_ot=none_id=691e13bfe400180cbd707269.mp4` | jonesroadbeauty | b-roll-overlay | none | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=jonesroadbeauty_s=bfcm_vf=comment-response_ot=amount-off_id=69291267e400180cbd39654d.mp4` | jonesroadbeauty | comment-response | amount-off | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=amount-off_id=6922744de400180cbd8f408b.mp4` | jonesroadbeauty | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=amount-off_id=69252a3be400180cbda4ed43.jpeg` | jonesroadbeauty | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=none_id=691e13bde400180cbd70640e.jpeg` | jonesroadbeauty | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=none_id=6922744de400180cbd8f407e.jpeg` | jonesroadbeauty | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=none_id=6923c7afe400180cbdc4b215.jpeg` | jonesroadbeauty | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=none_id=6923c7afe400180cbdc4b21b.jpeg` | jonesroadbeauty | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jonesroadbeauty_s=bfcm_vf=offer-banner_ot=none_id=69291267e400180cbd396560.jpeg` | jonesroadbeauty | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=jonesroadbeauty_s=bfcm_vf=product-animation_ot=none_id=692ca8f6e400180cbd7412f9.mp4` | jonesroadbeauty | product-animation | none | Alysha review (Sept 30 2026): offer-banner changed to product-animation |
| `b=jonesroadbeauty_s=bfcm_vf=product-grid_ot=amount-off_id=69291267e400180cbd39656d.jpeg` | jonesroadbeauty | product-grid | amount-off | - |
| `b=jonesroadbeauty_s=bfcm_vf=product-grid_ot=none_id=692e46d2e400180cbd191100.jpeg` | jonesroadbeauty | product-grid | none | Alysha review (Sept 30 2026): flatlay changed to product-grid |
| `b=jonesroadbeauty_s=bfcm_vf=split-screen_ot=tiered_id=6923c7afe400180cbdc4b210.mp4` | jonesroadbeauty | split-screen | tiered | Alysha review (Sept 30 2026): other changed to split-screen |
| `b=jonesroadbeauty_s=bfcm_vf=text-echo_ot=none_id=6922744de400180cbd8f4012.jpeg` | jonesroadbeauty | text-echo | none | Runneth first pass (Sept 30 2026): 'SALE' repeated eight times with products laid through the type; suggested text-echo instead of product-image. |
| `b=jonesroadbeauty_s=bfcm_vf=ugc-mashup_ot=amount-off_id=6926db78e400180cbd6f10d7.mp4` | jonesroadbeauty | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=jonesroadbeauty_s=bfcm_vf=yapper_ot=tiered_id=69268f62e400180cbdba2c72.mp4` | jonesroadbeauty | yapper | tiered | - |
| `b=kitsch_s=bfcm_vf=before-and-after_vf=ugc_ot=amount-off_id=6929ba21e400180cbdc555e9.mp4` | kitsch | before-and-after + ugc | amount-off | Alysha review (Sept 30 2026): before-and-after changed to before-and-after + ugc |
| `b=kitsch_s=bfcm_vf=bento-grid_ot=amount-off_id=69295adce400180cbd4034ef.jpeg` | kitsch | bento-grid | amount-off | Alysha review (Sept 30 2026): product-grid changed to bento-grid |
| `b=kitsch_s=bfcm_vf=offer-banner_ot=amount-off_id=6925cabfe400180cbd2e96c3.jpeg` | kitsch | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=kitsch_s=bfcm_vf=offer-banner_ot=amount-off_id=692b19b1e400180cbde281f1.jpeg` | kitsch | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=kitsch_s=bfcm_vf=shelfie_ot=amount-off_id=6925cabfe400180cbd2e96d7.jpeg` | kitsch | shelfie | amount-off | - |
| `b=kitsch_s=bfcm_vf=testimonial_vf=ugc_ot=amount-off_id=692b19b1e400180cbde281ea.mp4` | kitsch | testimonial + ugc | amount-off | Alysha review (Sept 30 2026): testimonial changed to testimonial + ugc |
| `b=kitsch_s=bfcm_vf=ugc_ot=amount-off_id=69283c45e400180cbd5ace06.mp4` | kitsch | ugc | amount-off | Alysha review (Sept 30 2026): flatlay changed to ugc |
| `b=kitsch_s=bfcm_vf=ugc_ot=amount-off_id=692bca66e400180cbd8f6c5d.mp4` | kitsch | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off_id=6917bc4fe4c6e2f6bc571c43.jpeg` | lemme | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off_id=6917bc4fe4c6e2f6bc571c49.mp4` | lemme | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off_id=6917bc4fe4c6e2f6bc571c4b.mp4` | lemme | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=magicmind_s=bfcm_vf=ad-in-the-wild_ot=amount-off_ot=free-gift_id=692cad6ee400180cbd7c70d3.jpeg` | magicmind | ad-in-the-wild | amount-off + free-gift | - |
| `b=magicmind_s=bfcm_vf=doodle_ot=amount-off_ot=free-gift_id=692916c2e400180cbd478b96.mp4` | magicmind | doodle | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to creative-parking-lot + doodle. Not meme: an original drawing with a relatable caption is not a recognizable meme template |
| `b=magicmind_s=bfcm_vf=letter_ot=amount-off_ot=free-gift_id=692916c2e400180cbd478b82.jpeg` | magicmind | letter | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to letter |
| `b=magicmind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=691d8a76e400180cbdb395db.mp4` | magicmind | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=magicmind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=691f9c09e400180cbdc8fdd0.jpeg` | magicmind | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=magicmind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=6923cfcce400180cbdd631cd.jpeg` | magicmind | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=magicmind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=692cad6ee400180cbd7c70dd.jpeg` | magicmind | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=magicmind_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift_id=6923cec5e400180cbdd457d5.mp4` | magicmind | product-animation | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=magicmind_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift_id=692cad6ee400180cbd7c70d4.mp4` | magicmind | product-animation | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=magicmind_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_id=692e4a01e400180cbd25618c.mp4` | magicmind | ugc-mashup | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=magicmind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift_id=691bb07de400180cbdcbbaa4.mp4` | magicmind | ugc + graphic-anchor | amount-off + free-gift | Alysha review (Sept 30 2026): yapper changed to ugc + graphic-anchor |
| `b=magicmind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift_id=691df98ae400180cbd0d2726.mp4` | magicmind | ugc + graphic-anchor | amount-off + free-gift | Alysha review (Sept 30 2026): graphic-anchor changed to ugc + graphic-anchor |
| `b=magicmind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift_id=692cad6ee400180cbd7c70dc.mp4` | magicmind | ugc + graphic-anchor | amount-off + free-gift | Alysha review (Sept 30 2026): testimonial changed to ugc + graphic-anchor |
| `b=opositiv_s=bfcm_vf=instagram-text-overlay_ot=bundle_ot=amount-off_id=6915b870e4c6e2f6bca22463.jpeg` | opositiv | instagram-text-overlay | bundle + amount-off | - |
| `b=opositiv_s=bfcm_vf=offer-banner_ot=amount-off_id=6919de47e4c6e2f6bc5d0944.jpeg` | opositiv | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=opositiv_s=bfcm_vf=offer-banner_ot=none_id=692ab2dde400180cbdf2447f.mp4` | opositiv | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=opositiv_s=bfcm_vf=testimonial_vf=ugc_ot=amount-off_id=6926eba1e400180cbd971d0b.mp4` | opositiv | testimonial + ugc | amount-off | Alysha review (Sept 30 2026): testimonial changed to testimonial + ugc |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=amount-off_id=6908c93052ed4a2ffc71eb61.jpeg` | ourplace | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=amount-off_id=69097dea2d77ca559dceb0fb.jpeg` | ourplace | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=amount-off_id=690af52a2d77ca559dd96494.jpeg` | ourplace | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=amount-off_id=690e2f962d77ca559d175f90.jpeg` | ourplace | offer-banner | amount-off | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=amount-off_id=69195203e4c6e2f6bc8b43e0.jpeg` | ourplace | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=none_id=6912bc7d2d77ca559dde314c.mp4` | ourplace | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=ourplace_s=bfcm_vf=offer-banner_ot=none_id=691eec7ee400180cbdb7f9e1.jpeg` | ourplace | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=ourplace_s=bfcm_vf=press_ot=none_id=691c4f90e400180cbd7c1e5b.jpeg` | ourplace | press | none | - |
| `b=ourplace_s=bfcm_vf=product-animation_ot=none_id=69157705e4c6e2f6bcdfe3c9.mp4` | ourplace | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=ourplace_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_id=690af52a2d77ca559dd96496.mp4` | ourplace | product-animation + offer-banner | amount-off | Alysha review (Sept 30 2026): offer-banner changed to product-animation + offer-banner |
| `b=ourplace_s=bfcm_vf=product-grid_ot=amount-off_id=6912bc7d2d77ca559dde3139.jpeg` | ourplace | product-grid | amount-off | Said 'over 45% off' so tagged sitewide |
| `b=ourplace_s=bfcm_vf=product-grid_ot=amount-off_id=691f161ae400180cbd230ad9.jpeg` | ourplace | product-grid | amount-off | Said 'over 35% off sitewide' so tagged sitewide |
| `b=ourplace_s=bfcm_vf=product-grid_vf=product-animation_ot=amount-off_id=690f72792d77ca559d1024b7.mp4` | ourplace | product-grid + product-animation | amount-off | Alysha review (Sept 30 2026): product-grid changed to product-grid + product-animation |
| `b=ourplace_s=bfcm_vf=ugc_ot=none_id=692818d7e400180cbdfa4b93.mp4` | ourplace | ugc | none | Alysha review (Sept 30 2026): other changed to ugc |
| `b=ourplace_s=bfcm_vf=ugc_ot=none_id=692818d7e400180cbdfa4bb4.mp4` | ourplace | ugc | none | Alysha review (Sept 30 2026): other changed to ugc |
| `b=prose_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift_id=6925ab64e400180cbdddbc94.mp4` | prose | b-roll-overlay | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=prose_s=bfcm_vf=bento-grid_ot=amount-off_ot=free-gift_id=69276d34e400180cbd237503.jpeg` | prose | bento-grid | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=prose_s=bfcm_vf=feature-benefit-pointout_ot=amount-off_ot=free-gift_id=690c57b12d77ca559d30f53e.jpeg` | prose | feature-benefit-pointout | amount-off + free-gift | Runneth first pass (Sept 30 2026): the free pouch with callout labels (plush terry exterior, waterproof lining...) is the hero; suggested feature-benefit-pointout instead of product-image. |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=690bcc5f2d77ca559d9d63fe.jpeg` | prose | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=6925ab63e400180cbdddbc7f.jpeg` | prose | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=6925ab63e400180cbdddbc89.mp4` | prose | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=69276d34e400180cbd237502.jpeg` | prose | offer-banner | amount-off + free-gift | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_id=69294b52e400180cbd016e6c.jpeg` | prose | offer-banner | amount-off + free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift_id=6925ab63e400180cbdddbc8e.mp4` | prose | product-animation | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=prose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift_id=6925ab64e400180cbdddbc9d.jpeg` | prose | product-grid | amount-off + free-gift | Alysha review (Sept 30 2026): other changed to product-grid |
| `b=prose_s=bfcm_vf=receipt_ot=amount-off_ot=free-gift_id=690bcc5f2d77ca559d9d63f6.jpeg` | prose | receipt | amount-off + free-gift | Tagged receipt by Runneth to match Alysha's new receipt format (Billie); not yet reviewed by her. |
| `b=prose_s=bfcm_vf=shelfie_ot=amount-off_ot=free-gift_id=690bcc5f2d77ca559d9d6402.jpeg` | prose | shelfie | amount-off + free-gift | - |
| `b=seed_s=bfcm_vf=offer-banner_ot=amount-off_id=692d8609e400180cbdaa421e.jpeg` | seed | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=seed_s=bfcm_vf=ugc_ot=amount-off_id=692d8609e400180cbdaa4227.mp4` | seed | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=thefarmersdog_s=bfcm_vf=bento-grid_ot=amount-off_id=692959ebe400180cbd3ced96.jpeg` | thefarmersdog | bento-grid | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=thefarmersdog_s=bfcm_vf=instagram-text-overlay_ot=amount-off_id=692959ebe400180cbd3cedba.jpeg` | thefarmersdog | instagram-text-overlay | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=thefarmersdog_s=bfcm_vf=offer-banner_ot=amount-off_id=692959ebe400180cbd3cece8.jpeg` | thefarmersdog | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=thefarmersdog_s=bfcm_vf=offer-banner_ot=amount-off_id=692959ebe400180cbd3ced53.jpeg` | thefarmersdog | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=thefarmersdog_s=bfcm_vf=offer-banner_ot=amount-off_id=692959ebe400180cbd3cee77.jpeg` | thefarmersdog | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=thefarmersdog_s=bfcm_vf=offer-banner_ot=amount-off_id=692ea951e400180cbd32e565.jpeg` | thefarmersdog | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Cyber Monday: 80% off your first box, flat, no stated condition |
| `b=thefarmersdog_s=bfcm_vf=ugc_ot=amount-off_id=692b16ace400180cbddce1d2.mp4` | thefarmersdog | ugc | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
