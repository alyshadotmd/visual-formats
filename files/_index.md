# Example files — index

This folder holds every example ad in the library, year-round and Black Friday together, in one place with one naming convention. The season lives in the file name (`s=evergreen` or `s=bfcm`). Format definitions are in `../formats/`. Each ad lives **once**, no duplicate files.

Merged on October 9th, 2026 from the old `evergreen/` and `bfcm/` folders. Black Friday files lost their Motion ID (`_id=`) at the same time, and a few brand names were respelled to match the rules (`everyday-dose`, `jones-road-beauty`, `magic-mind`, `o-positiv`, `our-place`, `the-farmers-dog`).

## Naming convention

```
[b=<brand>][_c=<creator>]_s=<season>_vf=<format>[_vf=<format2>]_ot=<offer type>[_ot=<offer type 2>][_tag=favorite][_n=<k>].<ext>
```

At least one of `b=` or `c=` is required. Order is brand, then creator, then season, then visual format(s), then offer type, then any special tag, then any collision number. Every file in this folder follows this one convention.

- **`b=`** brand, at most one. lowercase, dashes for spaces, strip punctuation, transliterate accents, `&` becomes `and`, keep the true spelling (`comfrt`, `mott-and-bow`, `the-farmers-dog`, `gruns`).
- **`c=`** creator handle, at most one. Same formatting rules as brand.
- **When to use which:**
  - Brand ad (no named creator): `b=<brand>` only.
  - Brand x creator partnership: include **both**, brand first: `b=<brand>_c=<creator>`.
  - Organic content or a creator-led post with no brand: `c=<creator>` only.
- **`s=`** season, one required: `evergreen` (year-round) or `bfcm` (Black Friday / Cyber Monday).
- **`vf=`** visual format, one required, **up to two** (a genuine dual-format ad repeats the `vf=` token). Value is the format folder name. **The primary (anchor) format goes first, the secondary format second.**
- **`ot=`** offer type, what the ad is giving you. Tokens and rules are in **Offer type (`ot=`)** below, the same for every season. Repeats for more than one offer; `none` when the ad shows no offer. Goes after the visual format(s) and before any `_n=`.
- **`tag=`** optional special tag, after offer type. Only value so far: `favorite` = one of Alysha's favorite ads ever. Favorites also get a same-name `.md` beside the file with the source, transcript, and creative analysis pre-read. Find them all by matching `_tag=favorite` (see Favorites below).
- Fields are separated by `_`; values use `-` inside a term; each field is prefixed with its tag and an `=`.
- Extension matches the media (`.jpg`, `.jpeg`, `.png`, `.mp4`).

> `=` is used instead of `:` because it is legal in filenames on Linux, macOS, and Windows, so the repo clones cleanly everywhere once the GitHub mirror is back.

### Offer type (`ot=`)

Set by Alysha (Sept 30 to Oct 6, 2026; moved into the naming rules Oct 9, 2026). Applies to every file in this folder. Lets people find offers that look like theirs and see how other brands position them. Offer type is the only offer tag.

| Token | Label | Meaning |
|---|---|---|
| amount-off | Amount off | a % or $ discount ("25% off", "up to 40% off", "$20 off", "spend $100, get 20% off") |
| free-gift | Free gift | a free product or gift with purchase |
| bundle | Bundle | a special set made for the promotion (for Black Friday, an exclusive Black Friday bundle). A brand's regular set, buy-more-save-more, or "$X of product for $Y" value framing is something else |
| tiered | Tiered | the deal grows in steps with how much you buy or spend (2+ steps): buy 1 get 10% off, buy 2 get 25% off; spend $50 save 15%, spend $100 save 20% |
| buy-x-get-y | Buy X, get Y | one buy-some-get-some deal on the same product: "buy 2, get 2 free", "buy one, get one 50% off" (matches Shopify's Buy X Get Y and Google Shopping's Buy M get N) |
| other | Other | an offer that fits none of the above (e.g. free shipping, gift card, donation) |
| none | None | the ad shows no offer; stands alone |

Judgment calls:
- One spend line ("spend $100+, get 20% off") is `amount-off`: there is only one step.
- Flat or "up to", sitewide or select products: all `amount-off`.
- A tiered deal is `tiered` only.
- A ladder of buy-X-get-Y deals is `tiered`; a different item thrown in is `free-gift`.
- "Free first box" / "X% off first box" is `amount-off`.
- Season says when, offer type says what. Subscription, first-order and creator-code deals are tagged by the deal itself (usually `amount-off`); the condition gets no tag.

### Collisions
If a new ad would produce a filename identical to an existing one (same brand/creator, season, format(s) and offer type), append `_n=2`, `_n=3`, and so on in the order added. Never overwrite or delete an existing file to resolve a collision without an explicit instruction on which to keep. Dedupe by bytes first (md5): an exact byte match is a true duplicate, skip it.

### Tag notes
A tagging note about one ad (for example why it's tagged `other`) goes in the Tag note column of Entries below. Black Friday notes carried over from the old Black Friday folder on October 9th, 2026.

### Finding examples
Match the token: all greenscreen examples are files containing `vf=greenscreen`; all Black Friday ads contain `s=bfcm`; all year-round ads contain `s=evergreen`. (Per-device example lists in the messaging-devices library were cleared on 2026-08-29 and are being rebuilt, so match by format token here for now.)

## ⭐ Favorites

Alysha's favorite ads ever, tagged `_tag=favorite`. Each has a same-name `.md` with the full breakdown. Newest first.

| File | Why it's a favorite |
|---|---|
| `b=panera-bread_c=jake-shane_s=evergreen_vf=comment-response_vf=signature-series_ot=none_tag=favorite.mp4` | Panera hired Jake Shane to make one more episode of his "can you do X finding out about Y" series, exactly the way he always does it. Panera requests it in the comments like a fan, Jake plays Soup testing a giant fur bed as the bread bowl, and the deal itself becomes the joke ("how are my splits gonna look?"). |
| `b=vella-studios_s=evergreen_vf=text-message_vf=cart-screenshot_ot=none_tag=favorite.jpg` | Organic post, not an ad (but she'd run it as one). Dad's "$281.15 for groceries" text matches the Pilates class pack total exactly. The price becomes the punchline and you work out the joke yourself. |
| `b=portland-leather-goods_c=heather-grace_s=evergreen_vf=comment-response_vf=yapper_ot=none_tag=favorite.mp4` | Replies to a real comment ("What size did you get?"), shows the proof in the first second, then answers each buyer question in order. "I'm really hard on bags" sells the durability. |

## Entries (493)

| File | Season | Brand | Creator | Visual format(s) | Offer type | Tag note |
|---|---|---|---|---|---|---|
| `b=actandacre_s=bfcm_vf=bento-grid_ot=amount-off.jpeg` | bfcm | actandacre | - | bento-grid | amount-off | - |
| `b=actandacre_s=bfcm_vf=bento-grid_ot=amount-off_n=2.jpeg` | bfcm | actandacre | - | bento-grid | amount-off | - |
| `b=actandacre_s=bfcm_vf=collage_ot=none.jpeg` | bfcm | actandacre | - | collage | none | - |
| `b=actandacre_s=bfcm_vf=collage_ot=none_n=2.jpeg` | bfcm | actandacre | - | collage | none | - |
| `b=actandacre_s=bfcm_vf=comment-response_ot=amount-off.mp4` | bfcm | actandacre | - | comment-response | amount-off | - |
| `b=actandacre_s=bfcm_vf=comment-response_ot=amount-off_n=2.mp4` | bfcm | actandacre | - | comment-response | amount-off | - |
| `b=actandacre_s=bfcm_vf=flatlay_ot=amount-off.jpeg` | bfcm | actandacre | - | flatlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=flatlay_ot=amount-off_n=2.jpeg` | bfcm | actandacre | - | flatlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=instagram-text-overlay_ot=amount-off.jpeg` | bfcm | actandacre | - | instagram-text-overlay | amount-off | - |
| `b=actandacre_s=bfcm_vf=other_ot=amount-off.jpeg` | bfcm | actandacre | - | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=actandacre_s=bfcm_vf=other_ot=amount-off_n=2.jpeg` | bfcm | actandacre | - | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=actandacre_s=bfcm_vf=shelfie_ot=amount-off.jpeg` | bfcm | actandacre | - | shelfie | amount-off | - |
| `b=actandacre_s=bfcm_vf=text-alert_ot=amount-off.mp4` | bfcm | actandacre | - | text-alert | amount-off | - |
| `b=actandacre_s=bfcm_vf=text-echo_ot=amount-off.jpeg` | bfcm | actandacre | - | text-echo | amount-off | - |
| `b=actandacre_s=bfcm_vf=transformation_ot=amount-off.mp4` | bfcm | actandacre | - | transformation | amount-off | - |
| `b=actandacre_s=evergreen_vf=case-study_ot=none.jpg` | evergreen | actandacre | - | case-study | none | - |
| `b=ag1_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift.mp4` | bfcm | ag1 | - | b-roll-overlay | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift.jpeg` | bfcm | ag1 | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | ag1 | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=3.jpeg` | bfcm | ag1 | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=4.jpeg` | bfcm | ag1 | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=instagram-text-overlay_ot=free-gift.jpeg` | bfcm | ag1 | - | instagram-text-overlay | free-gift | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | ag1 | - | offer-banner | amount-off | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | ag1 | - | offer-banner | amount-off | - |
| `b=ag1_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.jpeg` | bfcm | ag1 | - | offer-banner | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=product-animation_vf=offer-banner_ot=free-gift.mp4` | bfcm | ag1 | - | product-animation, offer-banner | free-gift | - |
| `b=ag1_s=bfcm_vf=product-grid_ot=free-gift.mp4` | bfcm | ag1 | - | product-grid | free-gift | - |
| `b=ag1_s=bfcm_vf=product-grid_ot=free-gift_n=2.jpeg` | bfcm | ag1 | - | product-grid | free-gift | - |
| `b=ag1_s=bfcm_vf=text-echo_ot=amount-off_ot=free-gift.jpeg` | bfcm | ag1 | - | text-echo | amount-off, free-gift | - |
| `b=ag1_s=bfcm_vf=ugc_ot=bundle_ot=free-gift.mp4` | bfcm | ag1 | - | ugc | bundle, free-gift | - |
| `b=agemate_s=evergreen_vf=post-it_ot=amount-off.jpeg` | evergreen | agemate | - | post-it | amount-off | - |
| `b=alo-yoga_s=evergreen_vf=bento-grid_ot=none.jpg` | evergreen | alo-yoga | - | bento-grid | none | - |
| `b=armra_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | evergreen | armra | - | ad-in-the-wild | none | - |
| `b=armra_s=evergreen_vf=web-search_ot=none.jpg` | evergreen | armra | - | web-search | none | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=amount-off.jpeg` | bfcm | arrae | - | instagram-text-overlay | amount-off | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=amount-off_n=2.jpeg` | bfcm | arrae | - | instagram-text-overlay | amount-off | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=none.mp4` | bfcm | arrae | - | instagram-text-overlay | none | - |
| `b=arrae_s=bfcm_vf=instagram-text-overlay_ot=none_n=2.mp4` | bfcm | arrae | - | instagram-text-overlay | none | - |
| `b=arrae_s=bfcm_vf=notes-app_vf=flatlay_ot=none.jpeg` | bfcm | arrae | - | notes-app, flatlay | none | - |
| `b=arrae_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | arrae | - | offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=offer-banner_ot=tiered.jpeg` | bfcm | arrae | - | offer-banner | tiered | Offer: tiered spend discount works for everyone; subscribing adds an extra 10%, so the condition is None (subscription is a bonus, not required). |
| `b=arrae_s=bfcm_vf=other_ot=amount-off.jpeg` | bfcm | arrae | - | other | amount-off | Was tagged product-image, a format Alysha retired on 2026-09-30; needs a format in her final pass. |
| `b=arrae_s=bfcm_vf=product-animation_ot=none.mp4` | bfcm | arrae | - | product-animation | none | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off.mp4` | bfcm | arrae | - | product-animation, offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_n=2.mp4` | bfcm | arrae | - | product-animation, offer-banner | amount-off | - |
| `b=arrae_s=bfcm_vf=product-animation_vf=offer-banner_ot=tiered.mp4` | bfcm | arrae | - | product-animation, offer-banner | tiered | Offer: tiered spend discount works for everyone; subscribing adds an extra 10%, so the condition is None (subscription is a bonus, not required). |
| `b=arrae_s=bfcm_vf=product-grid_ot=none.jpeg` | bfcm | arrae | - | product-grid | none | - |
| `b=arrae_s=bfcm_vf=shelfie_ot=none.jpeg` | bfcm | arrae | - | shelfie | none | - |
| `b=arrae_s=bfcm_vf=yapper_ot=amount-off.mp4` | bfcm | arrae | - | yapper | amount-off | - |
| `b=arrae_s=bfcm_vf=yapper_ot=amount-off_ot=bundle.mp4` | bfcm | arrae | - | yapper | amount-off, bundle | - |
| `b=arrae_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | arrae | - | instagram-text-overlay | none | - |
| `b=arrae_s=evergreen_vf=whiteboard_ot=none.jpg` | evergreen | arrae | - | whiteboard | none | - |
| `b=atlas-coffee-club_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | atlas-coffee-club | - | post-it | none | - |
| `b=atlas-coffee-club_s=evergreen_vf=text-message_ot=none.jpg` | evergreen | atlas-coffee-club | - | text-message | none | - |
| `b=babylist_s=evergreen_vf=comment-screenshot_ot=none.jpg` | evergreen | babylist | - | comment-screenshot | none | - |
| `b=barkbox_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | evergreen | barkbox | - | unexpected-text-placement | none | - |
| `b=barkbox_s=evergreen_vf=whiteboard_ot=none.jpg` | evergreen | barkbox | - | whiteboard | none | - |
| `b=beis_s=bfcm_vf=greenscreen_ot=amount-off.mp4` | bfcm | beis | - | greenscreen | amount-off | - |
| `b=betterhelp_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | betterhelp | - | post-it | none | - |
| `b=billie_s=bfcm_vf=collage_ot=amount-off.jpeg` | bfcm | billie | - | collage | amount-off | - |
| `b=billie_s=bfcm_vf=comment-response_ot=none.jpeg` | bfcm | billie | - | comment-response | none | - |
| `b=billie_s=bfcm_vf=product-grid_ot=none.jpeg` | bfcm | billie | - | product-grid | none | Alysha (Sept 30 2026): product-grid, but a very creative one; each product card is styled as a coupon with a barcode. |
| `b=billie_s=bfcm_vf=receipt_ot=amount-off.jpeg` | bfcm | billie | - | receipt | amount-off | - |
| `b=billie_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | evergreen | billie | - | feature-benefit-pointout | none | - |
| `b=billie_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | billie | - | instagram-text-overlay | none | - |
| `b=bobbie_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | evergreen | bobbie | - | ad-in-the-wild | none | - |
| `b=boll-and-branch_s=evergreen_vf=press_ot=none.jpeg` | evergreen | boll-and-branch | - | press | none | - |
| `b=boll-and-branch_s=evergreen_vf=web-search_ot=none.jpeg` | evergreen | boll-and-branch | - | web-search | none | - |
| `b=bonafide_s=evergreen_vf=greenscreen_ot=none.mp4` | evergreen | bonafide | - | greenscreen | none | - |
| `b=bonafide_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | bonafide | - | post-it | none | - |
| `b=brooklinen_s=evergreen_vf=press_ot=none.jpeg` | evergreen | brooklinen | - | press | none | - |
| `b=buoy_s=bfcm_vf=founder_ot=amount-off_ot=free-gift.mp4` | bfcm | buoy | - | founder | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift.jpeg` | bfcm | buoy | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | buoy | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=live-selling_ot=amount-off_ot=free-gift.mp4` | bfcm | buoy | - | live-selling | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | buoy | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.jpeg` | bfcm | buoy | - | offer-banner | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | buoy | - | offer-banner | amount-off, free-gift | Alysha (Sept 30 2026): torn with listicle because of the bundle list, but the offer ('The best deal on Buoy, ever / 43% off + 4 free gifts') is the hero, so offer-banner; the list supports the offer. |
| `b=buoy_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=3.jpeg` | bfcm | buoy | - | offer-banner | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift.jpeg` | bfcm | buoy | - | product-grid | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift.mp4` | bfcm | buoy | - | ugc-mashup | amount-off, free-gift | - |
| `b=buoy_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | buoy | - | ugc | amount-off | - |
| `b=buoy_s=evergreen_vf=founder_ot=none.mp4` | evergreen | buoy | - | founder | none | - |
| `b=buoy_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | evergreen | buoy | - | instagram-text-overlay | none | - |
| `b=buoy_s=evergreen_vf=podcast_ot=none.mp4` | evergreen | buoy | - | podcast | none | - |
| `b=buoy_s=evergreen_vf=taste-test_vf=yapper_ot=none.mp4` | evergreen | buoy | - | taste-test, yapper | none | - |
| `b=buoy_s=evergreen_vf=us-vs-them_ot=amount-off.jpg` | evergreen | buoy | - | us-vs-them | amount-off | - |
| `b=caraway_s=bfcm_vf=founder_ot=none.mp4` | bfcm | caraway | - | founder | none | - |
| `b=caraway_s=bfcm_vf=interview_ot=amount-off.mp4` | bfcm | caraway | - | interview | amount-off | - |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | caraway | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | caraway | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_n=3.jpeg` | bfcm | caraway | - | offer-banner | amount-off | Alysha (Sept 30 2026): not a flatlay (no real-life setting). Product in a frame with a big struck-through price ($446 / $800) under 'Black Friday Savings', so offer-banner by the hero test. |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_n=4.jpeg` | bfcm | caraway | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=offer-banner_ot=amount-off_n=5.jpeg` | bfcm | caraway | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=caraway_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off.mp4` | bfcm | caraway | - | product-animation, offer-banner | amount-off | - |
| `b=caraway_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off_n=2.mp4` | bfcm | caraway | - | product-animation, offer-banner | amount-off | - |
| `b=caraway_s=bfcm_vf=product-animation_vf=product-grid_ot=amount-off.mp4` | bfcm | caraway | - | product-animation, product-grid | amount-off | - |
| `b=caraway_s=bfcm_vf=stop-motion_ot=amount-off.mp4` | bfcm | caraway | - | stop-motion | amount-off | - |
| `b=caraway_s=bfcm_vf=street-interview_ot=amount-off.mp4` | bfcm | caraway | - | street-interview | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | caraway | - | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_n=2.mp4` | bfcm | caraway | - | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_n=3.mp4` | bfcm | caraway | - | ugc | amount-off | - |
| `b=caraway_s=bfcm_vf=ugc_ot=amount-off_n=4.mp4` | bfcm | caraway | - | ugc | amount-off | - |
| `b=caraway_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | caraway | - | instagram-text-overlay | none | - |
| `b=caraway_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | caraway | - | letter | none | - |
| `b=caraway_s=evergreen_vf=press_ot=none.jpeg` | evergreen | caraway | - | press | none | - |
| `b=caraway_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | caraway | - | us-vs-them | none | - |
| `b=cartablet_s=evergreen_vf=press_ot=none.jpeg` | evergreen | cartablet | - | press | none | - |
| `b=clickup_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | clickup | - | instagram-text-overlay | none | - |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none.mp4` | bfcm | comfrt | - | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none_n=2.mp4` | bfcm | comfrt | - | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_ot=none_n=3.mp4` | bfcm | comfrt | - | comment-response | none | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=comfrt_s=bfcm_vf=comment-response_vf=greenscreen_ot=amount-off.mp4` | bfcm | comfrt | - | comment-response, greenscreen | amount-off | Alysha review (Sept 30 2026): yapper changed to comment-response + greenscreen |
| `b=comfrt_s=evergreen_vf=comment-response_ot=none.mp4` | evergreen | comfrt | - | comment-response | none | - |
| `b=coterie-baby_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | evergreen | coterie-baby | - | feature-benefit-pointout | none | - |
| `b=dae_s=bfcm_vf=instagram-text-overlay_ot=amount-off.jpeg` | bfcm | dae | - | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): lifestyle photo with Instagram-style highlight text carrying the offer; suggested instagram-text-overlay instead of product-image. |
| `b=dae_s=bfcm_vf=offer-banner_vf=product-animation_ot=amount-off.mp4` | bfcm | dae | - | offer-banner, product-animation | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner + product-animation |
| `b=dae_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off.mp4` | bfcm | dae | - | product-animation, offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to product-animation + offer-banner |
| `b=dae_s=bfcm_vf=product-grid_ot=amount-off.mp4` | bfcm | dae | - | product-grid | amount-off | - |
| `b=dae_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | dae | - | us-vs-them | none | - |
| `b=dedcool_s=evergreen_vf=founder_ot=none.mp4` | evergreen | dedcool | - | founder | none | - |
| `b=dermalogica_s=evergreen_vf=product-animation_ot=none.mp4` | evergreen | dermalogica | - | product-animation | none | - |
| `b=dermalogica_s=evergreen_vf=review_ot=none.jpeg` | evergreen | dermalogica | - | review | none | - |
| `b=dermatica_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | dermatica | - | instagram-text-overlay | none | - |
| `b=divi_s=evergreen_vf=statistic_ot=none.jpg` | evergreen | divi | - | statistic | none | - |
| `b=dollar-shave-club_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | dollar-shave-club | - | instagram-text-overlay | none | - |
| `b=dose_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | evergreen | dose | - | feature-benefit-pointout | none | - |
| `b=dose_s=evergreen_vf=flyer_ot=none.jpg` | evergreen | dose | - | flyer | none | - |
| `b=dose_s=evergreen_vf=fortune-cookie_ot=none.jpg` | evergreen | dose | - | fortune-cookie | none | - |
| `b=dose_s=evergreen_vf=whiteboard_ot=none.jpg` | evergreen | dose | - | whiteboard | none | - |
| `b=dose_s=evergreen_vf=whiteboard_ot=none_n=2.mp4` | evergreen | dose | - | whiteboard | none | - |
| `b=eight-sleep_s=evergreen_vf=listicle_ot=none.mp4` | evergreen | eight-sleep | - | listicle | none | - |
| `b=ergobaby_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | ergobaby | - | us-vs-them | none | - |
| `b=everyday-dose_s=bfcm_vf=behind-the-scenes_ot=free-gift.mp4` | bfcm | everyday-dose | - | behind-the-scenes | free-gift | - |
| `b=everyday-dose_s=bfcm_vf=comment-response_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | comment-response | amount-off, free-gift | - |
| `b=everyday-dose_s=bfcm_vf=comment-response_vf=sign_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | comment-response, sign | amount-off, free-gift | Alysha review (Sept 30 2026): comment-response changed to comment-response + sign |
| `b=everyday-dose_s=bfcm_vf=comment-response_vf=whiteboard_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | comment-response, whiteboard | amount-off, free-gift | Alysha review (Sept 30 2026): whiteboard changed to comment-response + whiteboard |
| `b=everyday-dose_s=bfcm_vf=egc_vf=yapper_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | egc, yapper | amount-off, free-gift | Alysha review (Sept 30 2026): unboxing changed to egc + yapper |
| `b=everyday-dose_s=bfcm_vf=greenscreen_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | greenscreen | amount-off, free-gift | Alysha review (Sept 30 2026): yapper changed to greenscreen |
| `b=everyday-dose_s=bfcm_vf=high-production-edit_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | high-production-edit | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to high-production-edit |
| `b=everyday-dose_s=bfcm_vf=high-production-edit_ot=amount-off_ot=free-gift_n=2.mp4` | bfcm | everyday-dose | - | high-production-edit | amount-off, free-gift | Alysha review (Sept 30 2026): unboxing changed to high-production-edit |
| `b=everyday-dose_s=bfcm_vf=instagram-text-overlay_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | instagram-text-overlay | amount-off, free-gift | Alysha review (Sept 30 2026): feature-benefit-pointout changed to instagram-text-overlay |
| `b=everyday-dose_s=bfcm_vf=letter_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | letter | amount-off, free-gift | - |
| `b=everyday-dose_s=bfcm_vf=listicle_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | listicle | amount-off, free-gift | - |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | everyday-dose | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=amount-off_n=2.mp4` | bfcm | everyday-dose | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | everyday-dose | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): product-grid changed to offer-banner |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=3.jpeg` | bfcm | everyday-dose | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=free-gift.jpeg` | bfcm | everyday-dose | - | offer-banner | free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everyday-dose_s=bfcm_vf=offer-banner_ot=free-gift_n=2.jpeg` | bfcm | everyday-dose | - | offer-banner | free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=everyday-dose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | product-grid | amount-off, free-gift | - |
| `b=everyday-dose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | everyday-dose | - | product-grid | amount-off, free-gift | - |
| `b=everyday-dose_s=bfcm_vf=sign_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | sign | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to sign |
| `b=everyday-dose_s=bfcm_vf=text-message_ot=amount-off_ot=free-gift.jpeg` | bfcm | everyday-dose | - | text-message | amount-off, free-gift | Alysha review (Sept 30 2026): comment-screenshot changed to text-message |
| `b=everyday-dose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | ugc-mashup | amount-off, free-gift | Alysha review (Sept 30 2026): yapper changed to ugc-mashup |
| `b=everyday-dose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_n=2.mp4` | bfcm | everyday-dose | - | ugc-mashup | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=everyday-dose_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift_n=3.mp4` | bfcm | everyday-dose | - | ugc-mashup | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=everyday-dose_s=bfcm_vf=venn-diagram_ot=none.jpeg` | bfcm | everyday-dose | - | venn-diagram | none | Alysha review (Sept 30 2026): other changed to venn-diagram |
| `b=everyday-dose_s=bfcm_vf=whiteboard_vf=podcast_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | whiteboard, podcast | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to whiteboard + podcast |
| `b=everyday-dose_s=bfcm_vf=yapper_ot=amount-off_ot=free-gift.mp4` | bfcm | everyday-dose | - | yapper | amount-off, free-gift | - |
| `b=everyday-dose_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | everyday-dose | - | instagram-text-overlay | none | - |
| `b=everyday-dose_s=evergreen_vf=skit_ot=none.mp4` | evergreen | everyday-dose | - | skit | none | - |
| `b=everyday-dose_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | everyday-dose | - | yapper | none | - |
| `b=feel-goods_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | feel-goods | - | yapper | none | - |
| `b=finalputt_s=evergreen_vf=press_ot=none.jpeg` | evergreen | finalputt | - | press | none | - |
| `b=fiverr_s=evergreen_vf=before-and-after_ot=none.jpg` | evergreen | fiverr | - | before-and-after | none | - |
| `b=flakes_s=evergreen_vf=founder_ot=none.mp4` | evergreen | flakes | - | founder | none | - |
| `b=flakes_s=evergreen_vf=post-it_ot=amount-off.jpeg` | evergreen | flakes | - | post-it | amount-off | - |
| `b=girlfriend-collective_s=evergreen_vf=press_ot=none.jpeg` | evergreen | girlfriend-collective | - | press | none | - |
| `b=glossier_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | glossier | - | yapper | none | - |
| `b=gousto_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | gousto | - | instagram-text-overlay | none | - |
| `b=grove-collaborative_s=evergreen_vf=greenscreen_vf=listicle_ot=none.mp4` | evergreen | grove-collaborative | - | greenscreen, listicle | none | - |
| `b=grove-collaborative_s=evergreen_vf=news_ot=none.jpg` | evergreen | grove-collaborative | - | news | none | - |
| `b=gruns_s=bfcm_vf=b-roll-overlay_ot=amount-off.mp4` | bfcm | gruns | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=gruns_s=bfcm_vf=cart-screenshot_ot=amount-off.jpeg` | bfcm | gruns | - | cart-screenshot | amount-off | Alysha review (Sept 30 2026): other changed to creative-parking-lot + cart-screenshot |
| `b=gruns_s=bfcm_vf=collage_ot=amount-off.jpeg` | bfcm | gruns | - | collage | amount-off | Alysha review (Sept 30 2026): statistic changed to collage |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | gruns | - | offer-banner | amount-off | Says over 50% off so tagged sitewide Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | gruns | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_n=3.jpeg` | bfcm | gruns | - | offer-banner | amount-off | Alysha review (Sept 30 2026): statistic changed to offer-banner |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_n=4.jpeg` | bfcm | gruns | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=offer-banner_ot=amount-off_n=5.jpeg` | bfcm | gruns | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=gruns_s=bfcm_vf=press_ot=amount-off.mp4` | bfcm | gruns | - | press | amount-off | - |
| `b=gruns_s=bfcm_vf=street-interview_ot=amount-off.mp4` | bfcm | gruns | - | street-interview | amount-off | Alysha review (Sept 30 2026): other changed to street-interview |
| `b=gruns_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | gruns | - | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=gruns_s=bfcm_vf=us-vs-them_ot=none.jpeg` | bfcm | gruns | - | us-vs-them | none | - |
| `b=gruns_s=evergreen_vf=comment-response_ot=none.jpg` | evergreen | gruns | - | comment-response | none | - |
| `b=gruns_s=evergreen_vf=text-message_ot=none.jpg` | evergreen | gruns | - | text-message | none | - |
| `b=gruns_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | evergreen | gruns | - | unexpected-text-placement | none | - |
| `b=gruns_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | gruns | - | us-vs-them | none | - |
| `b=happy-mammoth_s=evergreen_vf=ai-animation_ot=none.mp4` | evergreen | happy-mammoth | - | ai-animation | none | - |
| `b=happy-mammoth_s=evergreen_vf=before-and-after_ot=none.jpg` | evergreen | happy-mammoth | - | before-and-after | none | - |
| `b=happy-mammoth_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | happy-mammoth | - | letter | none | - |
| `b=happy-mammoth_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | happy-mammoth | - | post-it | none | - |
| `b=happy-mammoth_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | evergreen | happy-mammoth | - | unexpected-text-placement | none | - |
| `b=harrys_s=evergreen_vf=comment-screenshot_ot=none.jpg` | evergreen | harrys | - | comment-screenshot | none | - |
| `b=headspace_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | evergreen | headspace | - | ad-in-the-wild | none | - |
| `b=hers_s=evergreen_vf=ad-in-the-wild_ot=amount-off.jpg` | evergreen | hers | - | ad-in-the-wild | amount-off | - |
| `b=hers_s=evergreen_vf=review_ot=none.jpg` | evergreen | hers | - | review | none | - |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | hexclad | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off_n=2.mp4` | bfcm | hexclad | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.mp4` | bfcm | hexclad | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none.jpeg` | bfcm | hexclad | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none_n=2.mp4` | bfcm | hexclad | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=hexclad_s=bfcm_vf=offer-banner_ot=none_n=3.mp4` | bfcm | hexclad | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=hexclad_s=bfcm_vf=post-it_ot=none.jpeg` | bfcm | hexclad | - | post-it | none | Runneth first pass (Sept 30 2026): a yellow sticky note reading 'Black Friday Sale' sits on the pan; suggested post-it instead of product-image. |
| `b=hexclad_s=bfcm_vf=text-alert_ot=amount-off.mp4` | bfcm | hexclad | - | text-alert | amount-off | - |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off.mp4` | bfcm | hexclad | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_n=2.mp4` | bfcm | hexclad | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_n=3.mp4` | bfcm | hexclad | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc-mashup_ot=amount-off_n=4.mp4` | bfcm | hexclad | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=hexclad_s=bfcm_vf=ugc_ot=none.mp4` | bfcm | hexclad | - | ugc | none | Alysha review (Sept 30 2026): unboxing changed to ugc |
| `b=hexclad_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | hexclad | - | post-it | none | - |
| `b=hims_s=evergreen_vf=comment-response_ot=none.jpg` | evergreen | hims | - | comment-response | none | - |
| `b=hinge_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | hinge | - | yapper | none | - |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_n=2.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_n=3.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_n=4.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_n=5.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=b-roll-overlay_ot=amount-off_n=6.mp4` | bfcm | hommey | - | b-roll-overlay | amount-off | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off.jpeg` | bfcm | hommey | - | bento-grid | amount-off | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off_n=2.jpeg` | bfcm | hommey | - | bento-grid | amount-off | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=hommey_s=bfcm_vf=bento-grid_ot=amount-off_n=3.mp4` | bfcm | hommey | - | bento-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off.jpeg` | bfcm | hommey | - | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): a personal note in story-style text over a lifestyle photo ('I almost missed this, but @hommey...'); suggested instagram-text-overlay instead of product-image. |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off_n=2.jpeg` | bfcm | hommey | - | instagram-text-overlay | amount-off | Alysha review (Sept 30 2026): other changed to instagram-text-overlay |
| `b=hommey_s=bfcm_vf=instagram-text-overlay_ot=amount-off_n=3.jpeg` | bfcm | hommey | - | instagram-text-overlay | amount-off | Runneth first pass (Sept 30 2026): a personal note in story-style text over a lifestyle photo ('I almost missed this, but @hommey...'); suggested instagram-text-overlay instead of product-image. |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | hommey | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | hommey | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_n=3.mp4` | bfcm | hommey | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_n=4.mp4` | bfcm | hommey | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner. Images swap at an even pace under a fixed offer (slideshow); slideshow is parked as a candidate format |
| `b=hommey_s=bfcm_vf=offer-banner_ot=amount-off_n=5.jpeg` | bfcm | hommey | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=hommey_s=bfcm_vf=press_ot=amount-off.jpeg` | bfcm | hommey | - | press | amount-off | - |
| `b=hommey_s=bfcm_vf=product-animation_ot=amount-off.mp4` | bfcm | hommey | - | product-animation | amount-off | Alysha review (Sept 30 2026): product-grid changed to product-animation |
| `b=hommey_s=bfcm_vf=product-animation_ot=none.mp4` | bfcm | hommey | - | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=hommey_s=bfcm_vf=product-animation_ot=none_n=2.mp4` | bfcm | hommey | - | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=hommey_s=bfcm_vf=product-grid_ot=amount-off.jpeg` | bfcm | hommey | - | product-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=product-grid_ot=amount-off_n=2.jpeg` | bfcm | hommey | - | product-grid | amount-off | - |
| `b=hommey_s=bfcm_vf=review_ot=amount-off.jpeg` | bfcm | hommey | - | review | amount-off | - |
| `b=hommey_s=bfcm_vf=shelfie_ot=amount-off.jpeg` | bfcm | hommey | - | shelfie | amount-off | - |
| `b=hommey_s=bfcm_vf=swatch-picker_ot=amount-off.mp4` | bfcm | hommey | - | swatch-picker | amount-off | Alysha review (Sept 30 2026): other changed to creative-parking-lot + swatch-picker |
| `b=honeylove_s=bfcm_vf=before-and-after_ot=amount-off.mp4` | bfcm | honeylove | - | before-and-after | amount-off | Alysha review (Sept 30 2026): other changed to before-and-after |
| `b=honeylove_s=bfcm_vf=comment-response_vf=ugc-mashup_ot=amount-off.mp4` | bfcm | honeylove | - | comment-response, ugc-mashup | amount-off | Alysha review (Sept 30 2026): comment-response changed to comment-response + ugc-mashup |
| `b=honeylove_s=bfcm_vf=flatlay_ot=amount-off.jpeg` | bfcm | honeylove | - | flatlay | amount-off | - |
| `b=honeylove_s=bfcm_vf=flatlay_vf=offer-banner_ot=amount-off.mp4` | bfcm | honeylove | - | flatlay, offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to flatlay + offer-banner |
| `b=honeylove_s=bfcm_vf=graphic-anchor_ot=amount-off.mp4` | bfcm | honeylove | - | graphic-anchor | amount-off | Alysha review (Sept 30 2026): other changed to graphic-anchor |
| `b=honeylove_s=bfcm_vf=letter_ot=free-gift.jpeg` | bfcm | honeylove | - | letter | free-gift | - |
| `b=honeylove_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | honeylove | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=honeylove_s=bfcm_vf=product-animation_vf=offer-banner_ot=none.mp4` | bfcm | honeylove | - | product-animation, offer-banner | none | Alysha review (Sept 30 2026): offer-banner changed to product-animation + offer-banner |
| `b=honeylove_s=bfcm_vf=review_ot=amount-off.jpeg` | bfcm | honeylove | - | review | amount-off | Alysha review (Sept 30 2026): other changed to review |
| `b=honeylove_s=bfcm_vf=split-screen_ot=amount-off.mp4` | bfcm | honeylove | - | split-screen | amount-off | Alysha review (Sept 30 2026): other changed to split-screen |
| `b=honeylove_s=bfcm_vf=split-screen_ot=amount-off_n=2.mp4` | bfcm | honeylove | - | split-screen | amount-off | Alysha review (Sept 30 2026): listicle changed to split-screen |
| `b=honeylove_s=bfcm_vf=ugc-mashup_ot=amount-off.mp4` | bfcm | honeylove | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): whiteboard changed to ugc-mashup |
| `b=honeylove_s=bfcm_vf=ugc-mashup_ot=amount-off_n=2.mp4` | bfcm | honeylove | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=honeylove_s=bfcm_vf=unboxing_ot=amount-off.mp4` | bfcm | honeylove | - | unboxing | amount-off | - |
| `b=honeylove_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | evergreen | honeylove | - | ad-in-the-wild | none | - |
| `b=honeylove_s=evergreen_vf=ai-animation_ot=none.mp4` | evergreen | honeylove | - | ai-animation | none | - |
| `b=honeylove_s=evergreen_vf=comment-response_ot=none.jpg` | evergreen | honeylove | - | comment-response | none | - |
| `b=honeylove_s=evergreen_vf=flowchart_ot=none.jpg` | evergreen | honeylove | - | flowchart | none | - |
| `b=honeylove_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | evergreen | honeylove | - | instagram-text-overlay | none | - |
| `b=honeylove_s=evergreen_vf=matching-chart_ot=none.jpg` | evergreen | honeylove | - | matching-chart | none | - |
| `b=honour-health_s=evergreen_vf=whiteboard_ot=none.mp4` | evergreen | honour-health | - | whiteboard | none | - |
| `b=huda-beauty_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | evergreen | huda-beauty | - | asmr, unboxing | none | - |
| `b=huel_s=evergreen_vf=explainer_ot=none.mp4` | evergreen | huel | - | explainer | none | - |
| `b=huel_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | huel | - | letter | none | - |
| `b=hum-nutrition_s=evergreen_vf=web-search_ot=none.jpg` | evergreen | hum-nutrition | - | web-search | none | - |
| `b=hydrant_s=evergreen_vf=line-chart_ot=buy-x-get-y.jpg` | evergreen | hydrant | - | line-chart | buy-x-get-y | - |
| `b=hydrant_s=evergreen_vf=point-to-screen_ot=buy-x-get-y.mp4` | evergreen | hydrant | - | point-to-screen | buy-x-get-y | - |
| `b=hydrant_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | hydrant | - | post-it | none | - |
| `b=hydrant_s=evergreen_vf=unexpected-text-placement_ot=none.jpg` | evergreen | hydrant | - | unexpected-text-placement | none | - |
| `b=ilia-beauty_s=evergreen_vf=behind-the-scenes_ot=none.mp4` | evergreen | ilia-beauty | - | behind-the-scenes | none | - |
| `b=infinity-hoop_s=evergreen_vf=us-vs-them_ot=amount-off_ot=free-gift.jpeg` | evergreen | infinity-hoop | - | us-vs-them | amount-off, free-gift | - |
| `b=instant-hydration_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | instant-hydration | - | letter | none | - |
| `b=instant-hydration_s=evergreen_vf=skit_ot=none.mp4` | evergreen | instant-hydration | - | skit | none | - |
| `b=intelligent-change_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | intelligent-change | - | instagram-text-overlay | none | - |
| `b=javvy_s=bfcm_vf=asmr_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | asmr | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to asmr |
| `b=javvy_s=bfcm_vf=asmr_ot=free-gift.mp4` | bfcm | javvy | - | asmr | free-gift | Alysha review (Sept 30 2026): other changed to asmr |
| `b=javvy_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | b-roll-overlay | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=javvy_s=bfcm_vf=challenge_ot=amount-off.mp4` | bfcm | javvy | - | challenge | amount-off | Alysha review (Sept 30 2026): other changed to challenge |
| `b=javvy_s=bfcm_vf=found-footage_vf=whiteboard_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | found-footage, whiteboard | amount-off, free-gift | Alysha review (Sept 30 2026): skit changed to found-footage + whiteboard |
| `b=javvy_s=bfcm_vf=greenscreen_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | greenscreen | amount-off, free-gift | - |
| `b=javvy_s=bfcm_vf=letter_ot=amount-off_ot=free-gift.jpeg` | bfcm | javvy | - | letter | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to letter |
| `b=javvy_s=bfcm_vf=skit_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | skit | amount-off, free-gift | - |
| `b=javvy_s=bfcm_vf=ugc_ot=amount-off_ot=free-gift.mp4` | bfcm | javvy | - | ugc | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to ugc |
| `b=javvy_s=bfcm_vf=ugc_ot=amount-off_ot=free-gift_n=2.mp4` | bfcm | javvy | - | ugc | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to ugc |
| `b=javvy_s=evergreen_vf=comment-response_vf=behind-the-scenes_ot=none.mp4` | evergreen | javvy | - | comment-response, behind-the-scenes | none | - |
| `b=javvy_s=evergreen_vf=notes-app_ot=none.jpg` | evergreen | javvy | - | notes-app | none | - |
| `b=javvy_s=evergreen_vf=whiteboard_ot=none.jpg` | evergreen | javvy | - | whiteboard | none | - |
| `b=jcrew_s=evergreen_vf=flatlay_ot=none.jpg` | evergreen | jcrew | - | flatlay | none | - |
| `b=jenny-bird_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | jenny-bird | - | instagram-text-overlay | none | - |
| `b=jolie_s=bfcm_vf=letter_ot=none.jpeg` | bfcm | jolie | - | letter | none | Alysha review (Sept 30 2026): other changed to letter |
| `b=jolie_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | jolie | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jolie_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | jolie | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jolie_s=evergreen_vf=statistic_ot=none.jpg` | evergreen | jolie | - | statistic | none | - |
| `b=jolie_s=evergreen_vf=statistic_ot=none_n=2.jpg` | evergreen | jolie | - | statistic | none | - |
| `b=jones-road-beauty_s=bfcm_vf=b-roll-overlay_ot=none.mp4` | bfcm | jones-road-beauty | - | b-roll-overlay | none | Alysha review (Sept 30 2026): ad-in-the-wild changed to b-roll-overlay |
| `b=jones-road-beauty_s=bfcm_vf=b-roll-overlay_ot=none_n=2.mp4` | bfcm | jones-road-beauty | - | b-roll-overlay | none | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=jones-road-beauty_s=bfcm_vf=comment-response_ot=amount-off.mp4` | bfcm | jones-road-beauty | - | comment-response | amount-off | Alysha review (Sept 30 2026): yapper changed to comment-response |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=amount-off.mp4` | bfcm | jones-road-beauty | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | jones-road-beauty | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=none.jpeg` | bfcm | jones-road-beauty | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=none_n=2.jpeg` | bfcm | jones-road-beauty | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=none_n=3.jpeg` | bfcm | jones-road-beauty | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=none_n=4.jpeg` | bfcm | jones-road-beauty | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=jones-road-beauty_s=bfcm_vf=offer-banner_ot=none_n=5.jpeg` | bfcm | jones-road-beauty | - | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=jones-road-beauty_s=bfcm_vf=product-animation_ot=none.mp4` | bfcm | jones-road-beauty | - | product-animation | none | Alysha review (Sept 30 2026): offer-banner changed to product-animation |
| `b=jones-road-beauty_s=bfcm_vf=product-grid_ot=amount-off.jpeg` | bfcm | jones-road-beauty | - | product-grid | amount-off | - |
| `b=jones-road-beauty_s=bfcm_vf=product-grid_ot=none.jpeg` | bfcm | jones-road-beauty | - | product-grid | none | Alysha review (Sept 30 2026): flatlay changed to product-grid |
| `b=jones-road-beauty_s=bfcm_vf=split-screen_ot=tiered.mp4` | bfcm | jones-road-beauty | - | split-screen | tiered | Alysha review (Sept 30 2026): other changed to split-screen |
| `b=jones-road-beauty_s=bfcm_vf=text-echo_ot=none.jpeg` | bfcm | jones-road-beauty | - | text-echo | none | Runneth first pass (Sept 30 2026): 'SALE' repeated eight times with products laid through the type; suggested text-echo instead of product-image. |
| `b=jones-road-beauty_s=bfcm_vf=ugc-mashup_ot=amount-off.mp4` | bfcm | jones-road-beauty | - | ugc-mashup | amount-off | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=jones-road-beauty_s=bfcm_vf=yapper_ot=tiered.mp4` | bfcm | jones-road-beauty | - | yapper | tiered | - |
| `b=jones-road-beauty_s=evergreen_vf=founder_ot=none.mp4` | evergreen | jones-road-beauty | - | founder | none | - |
| `b=jones-road-beauty_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | jones-road-beauty | - | instagram-text-overlay | none | - |
| `b=jones-road-beauty_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | jones-road-beauty | - | letter | none | - |
| `b=juniper_s=evergreen_vf=ad-in-the-wild_ot=none.jpg` | evergreen | juniper | - | ad-in-the-wild | none | - |
| `b=kitsch_s=bfcm_vf=before-and-after_vf=ugc_ot=amount-off.mp4` | bfcm | kitsch | - | before-and-after, ugc | amount-off | Alysha review (Sept 30 2026): before-and-after changed to before-and-after + ugc |
| `b=kitsch_s=bfcm_vf=bento-grid_ot=amount-off.jpeg` | bfcm | kitsch | - | bento-grid | amount-off | Alysha review (Sept 30 2026): product-grid changed to bento-grid |
| `b=kitsch_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | kitsch | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=kitsch_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | kitsch | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=kitsch_s=bfcm_vf=shelfie_ot=amount-off.jpeg` | bfcm | kitsch | - | shelfie | amount-off | - |
| `b=kitsch_s=bfcm_vf=testimonial_vf=ugc_ot=amount-off.mp4` | bfcm | kitsch | - | testimonial, ugc | amount-off | Alysha review (Sept 30 2026): testimonial changed to testimonial + ugc |
| `b=kitsch_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | kitsch | - | ugc | amount-off | Alysha review (Sept 30 2026): flatlay changed to ugc |
| `b=kitsch_s=bfcm_vf=ugc_ot=amount-off_n=2.mp4` | bfcm | kitsch | - | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=kitsch_s=evergreen_vf=post-it_ot=amount-off.mp4` | evergreen | kitsch | - | post-it | amount-off | - |
| `b=kitsch_s=evergreen_vf=skit_ot=none.mp4` | evergreen | kitsch | - | skit | none | - |
| `b=kosas_s=evergreen_vf=founder_ot=none.mp4` | evergreen | kosas | - | founder | none | - |
| `b=laseraway_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | laseraway | - | instagram-text-overlay | none | - |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | lemme | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off_n=2.mp4` | bfcm | lemme | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=lemme_s=bfcm_vf=offer-banner_ot=amount-off_n=3.mp4` | bfcm | lemme | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=lemme_s=evergreen_vf=comment-response_ot=none.jpeg` | evergreen | lemme | - | comment-response | none | - |
| `b=lemme_s=evergreen_vf=comment-screenshot_ot=none.jpeg` | evergreen | lemme | - | comment-screenshot | none | - |
| `b=lemme_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | evergreen | lemme | - | feature-benefit-callout | none | - |
| `b=little-caesars_c=jaredbuccii_s=evergreen_vf=skit_ot=none.mp4` | evergreen | little-caesars | jaredbuccii | skit | none | - |
| `b=loop_s=evergreen_vf=comment-response_ot=none.jpg` | evergreen | loop | - | comment-response | none | - |
| `b=loop_s=evergreen_vf=flyer_ot=amount-off.jpg` | evergreen | loop | - | flyer | amount-off | - |
| `b=loop_s=evergreen_vf=greenscreen_ot=none.mp4` | evergreen | loop | - | greenscreen | none | - |
| `b=loop_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | evergreen | loop | - | instagram-text-overlay | none | - |
| `b=loop_s=evergreen_vf=meme_ot=none.jpg` | evergreen | loop | - | meme | none | - |
| `b=loop_s=evergreen_vf=street-interview_ot=none.mp4` | evergreen | loop | - | street-interview | none | - |
| `b=lume-deodorant_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | lume-deodorant | - | instagram-text-overlay | none | - |
| `b=lume-deodorant_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | lume-deodorant | - | letter | none | - |
| `b=lyka_s=evergreen_vf=greenscreen_ot=none.mp4` | evergreen | lyka | - | greenscreen | none | - |
| `b=lyka_s=evergreen_vf=letter_ot=none.jpg` | evergreen | lyka | - | letter | none | - |
| `b=lyka_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | lyka | - | us-vs-them | none | - |
| `b=made-in_s=evergreen_vf=bento-grid_ot=none.jpg` | evergreen | made-in | - | bento-grid | none | - |
| `b=made-in_s=evergreen_vf=product-grid_ot=amount-off.jpg` | evergreen | made-in | - | product-grid | amount-off | - |
| `b=magic-mind_s=bfcm_vf=ad-in-the-wild_ot=amount-off_ot=free-gift.jpeg` | bfcm | magic-mind | - | ad-in-the-wild | amount-off, free-gift | - |
| `b=magic-mind_s=bfcm_vf=doodle_ot=amount-off_ot=free-gift.mp4` | bfcm | magic-mind | - | doodle | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to creative-parking-lot + doodle. Not meme: an original drawing with a relatable caption is not a recognizable meme template |
| `b=magic-mind_s=bfcm_vf=letter_ot=amount-off_ot=free-gift.jpeg` | bfcm | magic-mind | - | letter | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to letter |
| `b=magic-mind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.mp4` | bfcm | magic-mind | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=magic-mind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | magic-mind | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=magic-mind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=3.jpeg` | bfcm | magic-mind | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=magic-mind_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=4.jpeg` | bfcm | magic-mind | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=magic-mind_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift.mp4` | bfcm | magic-mind | - | product-animation | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=magic-mind_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift_n=2.mp4` | bfcm | magic-mind | - | product-animation | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=magic-mind_s=bfcm_vf=ugc-mashup_ot=amount-off_ot=free-gift.mp4` | bfcm | magic-mind | - | ugc-mashup | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to ugc-mashup |
| `b=magic-mind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift.mp4` | bfcm | magic-mind | - | ugc, graphic-anchor | amount-off, free-gift | Alysha review (Sept 30 2026): yapper changed to ugc + graphic-anchor |
| `b=magic-mind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift_n=2.mp4` | bfcm | magic-mind | - | ugc, graphic-anchor | amount-off, free-gift | Alysha review (Sept 30 2026): graphic-anchor changed to ugc + graphic-anchor |
| `b=magic-mind_s=bfcm_vf=ugc_vf=graphic-anchor_ot=amount-off_ot=free-gift_n=3.mp4` | bfcm | magic-mind | - | ugc, graphic-anchor | amount-off, free-gift | Alysha review (Sept 30 2026): testimonial changed to ugc + graphic-anchor |
| `b=magic-mind_s=evergreen_vf=sign_ot=none.jpg` | evergreen | magic-mind | - | sign | none | - |
| `b=marpipe_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | marpipe | - | letter | none | - |
| `b=mejuri_s=evergreen_vf=product-grid_ot=none.jpeg` | evergreen | mejuri | - | product-grid | none | - |
| `b=meller_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | meller | - | instagram-text-overlay | none | - |
| `b=menofmanual_s=evergreen_vf=before-and-after_ot=none.jpg` | evergreen | menofmanual | - | before-and-after | none | - |
| `b=menofmanual_s=evergreen_vf=feature-benefit-pointout_ot=amount-off.jpeg` | evergreen | menofmanual | - | feature-benefit-pointout | amount-off | - |
| `b=merit_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | evergreen | merit | - | feature-benefit-callout | none | - |
| `b=misfits-market_s=evergreen_vf=founder_ot=none.mp4` | evergreen | misfits-market | - | founder | none | - |
| `b=misfits-market_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | misfits-market | - | instagram-text-overlay | none | - |
| `b=momcozy_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | momcozy | - | yapper | none | - |
| `b=monday-haircare_s=evergreen_vf=press_ot=none.jpeg` | evergreen | monday-haircare | - | press | none | - |
| `b=moon-juice_s=evergreen_vf=before-and-after_ot=none.jpg` | evergreen | moon-juice | - | before-and-after | none | - |
| `b=moon-magic_s=evergreen_vf=comment-response_ot=none.png` | evergreen | moon-magic | - | comment-response | none | - |
| `b=moonbrew_s=evergreen_vf=founder_ot=none.mp4` | evergreen | moonbrew | - | founder | none | - |
| `b=mott-and-bow_s=evergreen_vf=comment-screenshot_ot=none.jpg` | evergreen | mott-and-bow | - | comment-screenshot | none | - |
| `b=mott-and-bow_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | mott-and-bow | - | post-it | none | - |
| `b=mous_s=evergreen_vf=high-production-edit_ot=none.mp4` | evergreen | mous | - | high-production-edit | none | - |
| `b=mud-wtr_s=evergreen_vf=founder_ot=none.mp4` | evergreen | mud-wtr | - | founder | none | - |
| `b=nanit_s=evergreen_vf=found-footage_vf=post-it_ot=none.mp4` | evergreen | nanit | - | found-footage, post-it | none | - |
| `b=native-pet_s=evergreen_vf=greenscreen_ot=none.mp4` | evergreen | native-pet | - | greenscreen | none | - |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=amount-off_ot=free-gift_n=4.jpg` | evergreen | natural-cycles | - | instagram-text-overlay | amount-off, free-gift | - |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | evergreen | natural-cycles | - | instagram-text-overlay | none | - |
| `b=natural-cycles_s=evergreen_vf=instagram-text-overlay_ot=none_n=3.jpg` | evergreen | natural-cycles | - | instagram-text-overlay | none | - |
| `b=natural-cycles_s=evergreen_vf=line-chart_ot=none.jpg` | evergreen | natural-cycles | - | line-chart | none | - |
| `b=nestig_s=evergreen_vf=comment-response_ot=none.jpeg` | evergreen | nestig | - | comment-response | none | - |
| `b=nutrafol-men_s=evergreen_vf=before-and-after_ot=none.jpg` | evergreen | nutrafol-men | - | before-and-after | none | - |
| `b=o-positiv_s=bfcm_vf=instagram-text-overlay_ot=bundle_ot=amount-off.jpeg` | bfcm | o-positiv | - | instagram-text-overlay | bundle, amount-off | - |
| `b=o-positiv_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | o-positiv | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=o-positiv_s=bfcm_vf=offer-banner_ot=none.mp4` | bfcm | o-positiv | - | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=o-positiv_s=bfcm_vf=testimonial_vf=ugc_ot=amount-off.mp4` | bfcm | o-positiv | - | testimonial, ugc | amount-off | Alysha review (Sept 30 2026): testimonial changed to testimonial + ugc |
| `b=o-positiv_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | evergreen | o-positiv | - | asmr, unboxing | none | - |
| `b=o-positiv_s=evergreen_vf=feature-benefit-callout_ot=none.jpg` | evergreen | o-positiv | - | feature-benefit-callout | none | - |
| `b=o-positiv_s=evergreen_vf=post-it_ot=none.jpg` | evergreen | o-positiv | - | post-it | none | - |
| `b=o-positiv_s=evergreen_vf=review_ot=none.jpg` | evergreen | o-positiv | - | review | none | - |
| `b=oats-overnight_s=evergreen_vf=founder_ot=none.mp4` | evergreen | oats-overnight | - | founder | none | - |
| `b=obvi_s=evergreen_vf=whiteboard_ot=none.jpg` | evergreen | obvi | - | whiteboard | none | - |
| `b=olipop_s=evergreen_vf=asmr_ot=none.mp4` | evergreen | olipop | - | asmr | none | - |
| `b=olipop_s=evergreen_vf=meme_ot=none.jpeg` | evergreen | olipop | - | meme | none | - |
| `b=onnit_s=evergreen_vf=venn-diagram_vf=whiteboard_ot=none.jpg` | evergreen | onnit | - | venn-diagram, whiteboard | none | - |
| `b=orgain_s=evergreen_vf=toggle_ot=none.jpg` | evergreen | orgain | - | toggle | none | - |
| `b=our-place_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | our-place | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=our-place_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | our-place | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=our-place_s=bfcm_vf=offer-banner_ot=amount-off_n=3.jpeg` | bfcm | our-place | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=our-place_s=bfcm_vf=offer-banner_ot=amount-off_n=4.jpeg` | bfcm | our-place | - | offer-banner | amount-off | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=our-place_s=bfcm_vf=offer-banner_ot=amount-off_n=5.jpeg` | bfcm | our-place | - | offer-banner | amount-off | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=our-place_s=bfcm_vf=offer-banner_ot=none.mp4` | bfcm | our-place | - | offer-banner | none | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). Video: check whether it should also get product-animation. |
| `b=our-place_s=bfcm_vf=offer-banner_ot=none_n=2.jpeg` | bfcm | our-place | - | offer-banner | none | Alysha review (Sept 30 2026): other changed to offer-banner |
| `b=our-place_s=bfcm_vf=press_ot=none.jpeg` | bfcm | our-place | - | press | none | - |
| `b=our-place_s=bfcm_vf=product-animation_ot=none.mp4` | bfcm | our-place | - | product-animation | none | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=our-place_s=bfcm_vf=product-animation_vf=offer-banner_ot=amount-off.mp4` | bfcm | our-place | - | product-animation, offer-banner | amount-off | Alysha review (Sept 30 2026): offer-banner changed to product-animation + offer-banner |
| `b=our-place_s=bfcm_vf=product-grid_ot=amount-off.jpeg` | bfcm | our-place | - | product-grid | amount-off | Said 'over 45% off' so tagged sitewide |
| `b=our-place_s=bfcm_vf=product-grid_ot=amount-off_n=2.jpeg` | bfcm | our-place | - | product-grid | amount-off | Said 'over 35% off sitewide' so tagged sitewide |
| `b=our-place_s=bfcm_vf=product-grid_vf=product-animation_ot=amount-off.mp4` | bfcm | our-place | - | product-grid, product-animation | amount-off | Alysha review (Sept 30 2026): product-grid changed to product-grid + product-animation |
| `b=our-place_s=bfcm_vf=ugc_ot=none.mp4` | bfcm | our-place | - | ugc | none | Alysha review (Sept 30 2026): other changed to ugc |
| `b=our-place_s=bfcm_vf=ugc_ot=none_n=2.mp4` | bfcm | our-place | - | ugc | none | Alysha review (Sept 30 2026): other changed to ugc |
| `b=our-place_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | our-place | - | letter | none | - |
| `b=panera-bread_c=jake-shane_s=evergreen_vf=comment-response_vf=signature-series_ot=none_tag=favorite.mp4` | evergreen | panera-bread | jake-shane | comment-response, signature-series | none | - |
| `b=pehr_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | pehr | - | instagram-text-overlay | none | - |
| `b=pela-case_s=evergreen_vf=founder_ot=none.mp4` | evergreen | pela-case | - | founder | none | - |
| `b=portland-leather-goods_c=heather-grace_s=evergreen_vf=comment-response_vf=yapper_ot=none_tag=favorite.mp4` | evergreen | portland-leather-goods | heather-grace | comment-response, yapper | none | - |
| `b=primally-pure-skincare_s=evergreen_vf=before-and-after_ot=amount-off.jpg` | evergreen | primally-pure-skincare | - | before-and-after | amount-off | - |
| `b=prose_s=bfcm_vf=b-roll-overlay_ot=amount-off_ot=free-gift.mp4` | bfcm | prose | - | b-roll-overlay | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to b-roll-overlay |
| `b=prose_s=bfcm_vf=bento-grid_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | bento-grid | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to bento-grid |
| `b=prose_s=bfcm_vf=feature-benefit-pointout_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | feature-benefit-pointout | amount-off, free-gift | Runneth first pass (Sept 30 2026): the free pouch with callout labels (plush terry exterior, waterproof lining...) is the hero; suggested feature-benefit-pointout instead of product-image. |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=2.jpeg` | bfcm | prose | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=3.mp4` | bfcm | prose | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=4.jpeg` | bfcm | prose | - | offer-banner | amount-off, free-gift | Alysha review (Sept 30 2026): flatlay changed to offer-banner |
| `b=prose_s=bfcm_vf=offer-banner_ot=amount-off_ot=free-gift_n=5.jpeg` | bfcm | prose | - | offer-banner | amount-off, free-gift | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=prose_s=bfcm_vf=product-animation_ot=amount-off_ot=free-gift.mp4` | bfcm | prose | - | product-animation | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to product-animation |
| `b=prose_s=bfcm_vf=product-grid_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | product-grid | amount-off, free-gift | Alysha review (Sept 30 2026): other changed to product-grid |
| `b=prose_s=bfcm_vf=receipt_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | receipt | amount-off, free-gift | Tagged receipt by Runneth to match Alysha's new receipt format (Billie); not yet reviewed by her. |
| `b=prose_s=bfcm_vf=shelfie_ot=amount-off_ot=free-gift.jpeg` | bfcm | prose | - | shelfie | amount-off, free-gift | - |
| `b=prose_s=evergreen_vf=before-and-after_vf=listicle_ot=none.mp4` | evergreen | prose | - | before-and-after, listicle | none | - |
| `b=prose_s=evergreen_vf=letter_ot=amount-off.jpeg` | evergreen | prose | - | letter | amount-off | - |
| `b=purdy-and-figg_s=evergreen_vf=letter_ot=none.jpg` | evergreen | purdy-and-figg | - | letter | none | - |
| `b=purple_s=evergreen_vf=letter_ot=none.jpeg` | evergreen | purple | - | letter | none | - |
| `b=purple_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | purple | - | us-vs-them | none | - |
| `b=rheal_s=evergreen_vf=handwritten_ot=amount-off_ot=free-gift_ot=other.jpeg` | evergreen | rheal | - | handwritten | amount-off, free-gift, other | - |
| `b=rheal_s=evergreen_vf=notes-app_vf=listicle_ot=none.jpeg` | evergreen | rheal | - | notes-app, listicle | none | - |
| `b=rheal_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | rheal | - | post-it | none | - |
| `b=rough-country_s=evergreen_vf=asmr_vf=unboxing_ot=none.mp4` | evergreen | rough-country | - | asmr, unboxing | none | - |
| `b=runna_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | runna | - | post-it | none | - |
| `b=ryze_s=evergreen_vf=annotation_ot=none.mp4` | evergreen | ryze | - | annotation | none | - |
| `b=saie-beauty_s=evergreen_vf=press_ot=none.jpg` | evergreen | saie-beauty | - | press | none | - |
| `b=sans_s=evergreen_vf=feature-benefit-callout_ot=none.jpeg` | evergreen | sans | - | feature-benefit-callout | none | - |
| `b=sans_s=evergreen_vf=live-demo_ot=none.mp4` | evergreen | sans | - | live-demo | none | - |
| `b=scentbird_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | scentbird | - | post-it | none | - |
| `b=seed_c=bobby-parrish_s=evergreen_vf=explainer_ot=amount-off_ot=free-gift.mp4` | evergreen | seed | bobby-parrish | explainer | amount-off, free-gift | - |
| `b=seed_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | seed | - | offer-banner | amount-off | Runneth first pass (Sept 30 2026): product-image changed to offer-banner under Alysha's hero test (the offer or sale headline is what you read first). |
| `b=seed_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | seed | - | ugc | amount-off | Alysha review (Sept 30 2026): other changed to ugc |
| `b=seed_s=evergreen_vf=faq_ot=none.jpeg` | evergreen | seed | - | faq | none | - |
| `b=seed_s=evergreen_vf=text-echo_ot=amount-off.jpeg` | evergreen | seed | - | text-echo | amount-off | - |
| `b=seed_s=evergreen_vf=whiteboard_ot=none.mp4` | evergreen | seed | - | whiteboard | none | - |
| `b=smol_s=evergreen_vf=post-it_ot=none.mp4` | evergreen | smol | - | post-it | none | - |
| `b=solawave_s=evergreen_vf=yapper_vf=graphic-anchor_ot=none.mp4` | evergreen | solawave | - | yapper, graphic-anchor | none | - |
| `b=solderstick_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | solderstick | - | instagram-text-overlay | none | - |
| `b=solderstick_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | solderstick | - | us-vs-them | none | - |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=amount-off_n=2.jpg` | evergreen | spacegoods | - | instagram-text-overlay | amount-off | - |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=amount-off_n=3.mp4` | evergreen | spacegoods | - | instagram-text-overlay | amount-off | - |
| `b=spacegoods_s=evergreen_vf=instagram-text-overlay_ot=none.jpg` | evergreen | spacegoods | - | instagram-text-overlay | none | - |
| `b=suri_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | suri | - | instagram-text-overlay | none | - |
| `b=suri_s=evergreen_vf=press_ot=none.jpeg` | evergreen | suri | - | press | none | - |
| `b=surreal_s=evergreen_vf=behind-the-scenes_ot=none.mp4` | evergreen | surreal | - | behind-the-scenes | none | - |
| `b=the-farmers-dog_s=bfcm_vf=bento-grid_ot=amount-off.jpeg` | bfcm | the-farmers-dog | - | bento-grid | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=bfcm_vf=instagram-text-overlay_ot=amount-off.jpeg` | bfcm | the-farmers-dog | - | instagram-text-overlay | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=bfcm_vf=offer-banner_ot=amount-off.jpeg` | bfcm | the-farmers-dog | - | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=bfcm_vf=offer-banner_ot=amount-off_n=2.jpeg` | bfcm | the-farmers-dog | - | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=bfcm_vf=offer-banner_ot=amount-off_n=3.jpeg` | bfcm | the-farmers-dog | - | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=bfcm_vf=offer-banner_ot=amount-off_n=4.jpeg` | bfcm | the-farmers-dog | - | offer-banner | amount-off | Formats picked by Alysha (Oct 1 2026). Cyber Monday: 80% off your first box, flat, no stated condition |
| `b=the-farmers-dog_s=bfcm_vf=ugc_ot=amount-off.mp4` | bfcm | the-farmers-dog | - | ugc | amount-off | Formats picked by Alysha (Oct 1 2026). Free first box (100% off the first order, which the video states outright) tagged % off + sitewide; first-box/new-customer only is not a condition per the offer taxonomy |
| `b=the-farmers-dog_s=evergreen_vf=feature-benefit-pointout_ot=none.jpeg` | evergreen | the-farmers-dog | - | feature-benefit-pointout | none | - |
| `b=the-farmers-dog_s=evergreen_vf=post-it_ot=amount-off.jpeg` | evergreen | the-farmers-dog | - | post-it | amount-off | - |
| `b=the-oodie_s=evergreen_vf=us-vs-them_ot=none.jpg` | evergreen | the-oodie | - | us-vs-them | none | - |
| `b=thrive-causemetics_s=evergreen_vf=comment-response_ot=none.jpeg` | evergreen | thrive-causemetics | - | comment-response | none | - |
| `b=thrive-causemetics_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | thrive-causemetics | - | instagram-text-overlay | none | - |
| `b=thrive-causemetics_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | thrive-causemetics | - | post-it | none | - |
| `b=timeline-longevity_s=evergreen_vf=instagram-text-overlay_ot=amount-off.mp4` | evergreen | timeline-longevity | - | instagram-text-overlay | amount-off | - |
| `b=timeline-longevity_s=evergreen_vf=press_ot=none.jpeg` | evergreen | timeline-longevity | - | press | none | - |
| `b=timeline-longevity_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | timeline-longevity | - | us-vs-them | none | - |
| `b=trade_s=evergreen_vf=comment-response_vf=us-vs-them_ot=none.jpg` | evergreen | trade | - | comment-response, us-vs-them | none | - |
| `b=trade_s=evergreen_vf=instagram-text-overlay_ot=none.jpeg` | evergreen | trade | - | instagram-text-overlay | none | - |
| `b=vella-studios_s=evergreen_vf=text-message_vf=cart-screenshot_ot=none_tag=favorite.jpg` | evergreen | vella-studios | - | text-message, cart-screenshot | none | - |
| `b=viome_s=evergreen_vf=press_ot=none.jpg` | evergreen | viome | - | press | none | - |
| `b=vitable_s=evergreen_vf=post-it_ot=none.jpeg` | evergreen | vitable | - | post-it | none | - |
| `b=vrbo_s=evergreen_vf=whiteboard_ot=none.mp4` | evergreen | vrbo | - | whiteboard | none | - |
| `b=vuori_s=evergreen_vf=bento-grid_ot=none.jpeg` | evergreen | vuori | - | bento-grid | none | - |
| `b=wild-nutrition_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | wild-nutrition | - | us-vs-them | none | - |
| `b=winona_s=evergreen_vf=comment-response_ot=none.jpg` | evergreen | winona | - | comment-response | none | - |
| `b=your-heights_s=evergreen_vf=sign_ot=none.jpg` | evergreen | your-heights | - | sign | none | - |
| `b=your-heights_s=evergreen_vf=us-vs-them_ot=none.jpeg` | evergreen | your-heights | - | us-vs-them | none | - |
| `b=your-heights_s=evergreen_vf=yapper_ot=none.mp4` | evergreen | your-heights | - | yapper | none | - |
