# Deployed asset provenance

Licence record for every third-party-derived asset served from `kilted.scot`, **keyed by the
filename as deployed here**, not by whatever it was called upstream.

Created 06/09/2026 after a real gap: a grep for `skye-hero-1280.jpg` found no licence record in
either this project's tree or the originating series', because the file is **renamed on
deployment** and the rename destroyed the provenance signal. Just Along Here holds it as
`brand\skye-pixabay-nocredit-1280.jpg` — a name carrying both the source and the
attribution-not-required fact — and it arrives here as `skye-hero-1280.jpg`, with both signals gone.
The record existed and was complete; it simply was not findable under the name this side uses.

That is the point of this file. **A rename across trees is a silent deletion of compliance
evidence, and nothing flags it.** See `VISUAL-SOURCING-STANDARD.md` §11.

Each entry records the **upstream alias** so a search on either name lands here.

---

## just-along-here/skye-hero-1280.jpg

- **Upstream alias:** `Just Along Here\brand\skye-pixabay-nocredit-1280.jpg` (byte-identical,
  md5 `33fdbd3c32fae6666ebfd91bb273cd32`, verified 06/09/2026)
- **Source:** https://pixabay.com/photos/landscape-scotland-isle-of-skye-540115/
- **Licence:** Pixabay Content License — commercial use permitted, **attribution not required**
- **Acquired:** 02/09/2026 by Just Along Here
- **Used on:** that series' page hero, and the homepage series card
- **Note:** it replaced a Glencoe CC BY-SA 4.0 photograph *specifically* to avoid the credit-line
  placement problem. "No attribution needed" was the reason it was chosen — worth knowing before
  anyone swaps it for something that reintroduces the requirement.

## just-along-here/culross-palace.jpg, culross-townhouse.jpg, culross-mercat-cross.jpg, culross-biscuit-cafe.jpg, culross-tanhouse-brae.jpg, culross-boat-house.jpg, culross-low-causeway.jpg

- **Upstream alias:** none — downloaded directly from source and renamed on arrival (no prior copy
  existed in any project tree). Self-hosted **not by convention but by necessity**: both source hosts
  (Wikimedia Commons' `Special:FilePath`, geograph.org.uk) block cross-origin `<img>` embedding by
  referrer/hotlink policy — confirmed live 27/09/2026 (each URL loads fine on direct navigation,
  fails silently as an embedded image on this site's own origin). Hotlinking these was never a viable
  option, not just a best-practice violation.
- **Source / licence, per image (all CC BY-SA, attribution required, given in the notes page's own
  Image credits section):**
  - `culross-palace.jpg` — Wikimedia Commons, "Culross Palace from the west", Michael Garlick, CC BY-SA
    4.0. md5 `682ae9caad801c154e2e3e95158c164a`.
  - `culross-townhouse.jpg` — geograph.org.uk photo 2947206, kim traynor, CC BY-SA 2.0. md5
    `c8539a8aec3936bd77ef4b09eca30cb0`.
  - `culross-mercat-cross.jpg` — Wikimedia Commons, "Mercat Cross and The Study, Culross", Calumsmith0308,
    CC BY-SA 4.0. md5 `360bbca66023f1412d4264a8b792eb64`.
  - `culross-biscuit-cafe.jpg` — geograph.org.uk photo 6856615, Richard Sutcliffe, CC BY-SA 2.0. md5
    `4ece40decb06a1632929627d6391d317`.
  - `culross-tanhouse-brae.jpg` — geograph.org.uk photo 8153066, Anne Burgess, CC BY-SA 2.0. md5
    `bf6e8495f4d9172a5d1959996eda69f5`.
  - `culross-boat-house.jpg` — geograph.org.uk photo 6301598, David Rogers, CC BY-SA 2.0. md5
    `510aec53474bd789619ff2fd4a8d6619`.
  - `culross-low-causeway.jpg` — geograph.org.uk photo 7987371, Richard Sutcliffe, CC BY-SA 2.0. md5
    `1987c6a1b3f22e70bd1dec6673fed18d`.
- **Acquired:** 27/09/2026, kilted.scot — same photos/photographers/licences already vetted in Just
  Along Here's own `episodes\01-culross\assets.md` for the video itself; this is their first use on
  the notes page, a separate publication per this file's own rule below.
- **Used on:** the Just Along Here Episode 1 (Culross) notes page stop images — linked from
  `episodes.json` 27/09/2026 after Just Along Here approved the pilot.

## just-along-here/dunbar-harbour-hero.jpg, dunbar-harbour-old-harbour-boats.jpg, dunbar-harbour-castle.jpg, dunbar-harbour-propeller.jpg, dunbar-harbour-creels.jpg

- **Upstream alias:** none. Each file was downloaded directly from Wikimedia Commons (the Commons
  API's 1280px rendition), downscaled to 1200px wide, re-saved as JPEG q85 and renamed on arrival.
  No earlier copy exists in any project tree. They are self-hosted **because they have to be**, not
  out of habit: Wikimedia Commons and geograph.org.uk both block cross-origin `<img>` embedding.
  That was confirmed live on the Culross pilot, 27/09/2026.
- **Source / licence for each image.** All five are geograph.org.uk photos mirrored on Wikimedia
  Commons under CC BY-SA 2.0. Attribution is required. It is given under each image (`pic-credit`)
  and again in the notes page's own Image credits section:
  - `dunbar-harbour-hero.jpg`: "Hundreds of Creels at Dunbar Harbour", geograph.org.uk photo
    5747138, Jennifer Petrie, CC BY-SA 2.0. Source:
    https://commons.wikimedia.org/wiki/File:Hundreds_of_Creels_at_Dunbar_Harbour_-_geograph.org.uk_-_5747138.jpg
    Deployed at 1200×900. md5 `6ab0dbb42843d6d6b9ed39561c68dab1`.
    **No credit is burned in.** The page hero renders no credit line of its own. Attribution lives in
    the Image credits section (`VISUAL-SOURCING-STANDARD.md` §14). If this is ever promoted to a
    homepage `cardImage`, it needs a `cardImageCredit` field.
  - `dunbar-harbour-old-harbour-boats.jpg`: "Fishing Boats sheltering in the Old Harbour Dunbar",
    geograph.org.uk photo 6322808, Jennifer Petrie, CC BY-SA 2.0. Source:
    https://commons.wikimedia.org/wiki/File:Fishing_Boats_sheltering_in_the_Old_Harbour_Dunbar_-_geograph.org.uk_-_6322808.jpg
    md5 `f5f36432f1894f071f3f640f8bab60cd`.
  - `dunbar-harbour-castle.jpg`: "Dunbar Harbour and Castle remains", geograph.org.uk photo 2530438,
    M J Richardson, CC BY-SA 2.0. Source:
    https://commons.wikimedia.org/wiki/File:Dunbar_Harbour_and_Castle_remains_-_geograph.org.uk_-_2530438.jpg
    md5 `f6a4e258970e4f3037b0beb287933401`.
  - `dunbar-harbour-propeller.jpg`: "Wilson's Propeller at Dunbar Harbour", geograph.org.uk photo
    6534254, Jennifer Petrie, CC BY-SA 2.0. Source:
    https://commons.wikimedia.org/wiki/File:Wilson%27s_Propeller_at_Dunbar_Harbour_-_geograph.org.uk_-_6534254.jpg
    md5 `54c09c810dd9c4b7f64bace0bfb953f6`.
  - `dunbar-harbour-creels.jpg`: "A pile of Creels at Old Harbour Dunbar", geograph.org.uk photo
    6248351, Jennifer Petrie, CC BY-SA 2.0. Source:
    https://commons.wikimedia.org/wiki/File:A_pile_of_Creels_at_Old_Harbour_Dunbar_-_geograph.org.uk_-_6248351.jpg
    md5 `a77b36e78754a30097cb0c3a05b81b7b`.
- **Licence and author metadata** were read from each file's Commons `extmetadata` (the Artist and
  LicenseShortName fields) on 27/09/2026. None of these five photos are Just Along Here's own
  footage, so this is a first publication for each of them, per the rule at the foot of ASSETS.md.
- **Acquired:** 27/09/2026 by kilted.scot.
- **Used on:** the Just Along Here Episode 2 (Dunbar Harbour) notes page,
  `just-along-here/08-dunbar-harbour/`, for the hero and four stop thumbnails. Linked from
  `episodes.json` 27/09/2026.

## just-along-here/pittencrieff-hero.jpg, pittencrieff-gates.jpg, pittencrieff-statue.jpg, pittencrieff-house.jpg, pittencrieff-tower.jpg, pittencrieff-tower-bridge.jpg, pittencrieff-wallace-well.jpg

- **Upstream alias:** none — downloaded directly from Wikimedia Commons (via the Commons API, full file
  or a Commons-rendered thumbnail) and renamed on arrival; no prior copy existed in any project tree.
  Downscaled to at most 1200px wide (hero 1280px) and re-saved as JPEG q85 with Pillow. Self-hosted
  **by necessity**, same as the Culross set: Commons and geograph.org.uk block cross-origin `<img>`
  embedding.
- **Source / licence, per image (all CC BY-SA, attribution required, given as text in the notes
  page's own pic-credit lines and Image credits section — no credit is burned into any file):**
  - `pittencrieff-hero.jpg` — Wikimedia Commons, "Gardens in Pittencrieff Park.jpg"
    (https://commons.wikimedia.org/wiki/File:Gardens_in_Pittencrieff_Park.jpg), Dkardokas, CC BY-SA
    3.0. 2000×1333 original → 1280×853. md5 `6580c50706b7bdf15cab337908928044`.
  - `pittencrieff-gates.jpg` — geograph.org.uk photo 7659558 via Wikimedia Commons, "Entrance to
    Pittencrieff Park, Dunfermline"
    (https://commons.wikimedia.org/wiki/File:Entrance_to_Pittencrieff_Park,_Dunfermline_-_geograph.org.uk_-_7659558.jpg),
    Jim Barton, CC BY-SA 2.0. 1600×1060 → 1200×795. md5 `f0781b53f9aca5ebb4717a122b475f71`.
  - `pittencrieff-statue.jpg` — geograph.org.uk photo 7659565 via Wikimedia Commons, "Andrew
    Carnegie's statue, Dunfermline"
    (https://commons.wikimedia.org/wiki/File:Andrew_Carnegie%27s_statue,_Dunfermline_-_geograph.org.uk_-_7659565.jpg),
    Jim Barton, CC BY-SA 2.0. 1600×1200 → 1200×900. md5 `03a888dc39e0e53e65ba89699a70abad`.
  - `pittencrieff-house.jpg` — Wikimedia Commons, "Pittencrieff House, Dunfermline Fife.jpg"
    (https://commons.wikimedia.org/wiki/File:Pittencrieff_House,_Dunfermline_Fife.jpg), Kim Traynor,
    CC BY-SA 3.0. 2557×1801 → 1200×846. md5 `9323aff3068dfd91155b458965aa46e6`.
  - `pittencrieff-tower.jpg` — Wikimedia Commons, "The Malcolm Canmore's Tower ruins, Pittencrieff
    Park, Dunfermline.jpg"
    (https://commons.wikimedia.org/wiki/File:The_Malcolm_Canmore%27s_Tower_ruins,_Pittencrieff_Park,_Dunfermline.jpg),
    Rosser1954, CC BY-SA 4.0. 1920×1080 → 1200×675. md5 `da63b2f4b7391421919ebb74f2672540`.
  - `pittencrieff-tower-bridge.jpg` — geograph.org.uk photo 2673045 via Wikimedia Commons, "Double
    bridge in Pittencrieff Glen"
    (https://commons.wikimedia.org/wiki/File:Double_bridge_in_Pittencrieff_Glen_-_geograph.org.uk_-_2673045.jpg),
    kim traynor, CC BY-SA 2.0. 480×640, not resized (re-encoded only). md5
    `8ad9bd04c80740f2b3a60f38379fac2f`.
  - `pittencrieff-wallace-well.jpg` — Wikimedia Commons, "Wallace Spa Well entrance, Pittencrieff Glen,
    Dunfermline.jpg"
    (https://commons.wikimedia.org/wiki/File:Wallace_Spa_Well_entrance,_Pittencrieff_Glen,_Dunfermline.jpg),
    Rosser1954, CC BY-SA 4.0. 1920×1080 → 1200×675. md5 `bbe23c88e09bc38c131bf81e01f4745d`.
- **Acquired:** 27/09/2026, kilted.scot. Licence and author read from each file's Commons
  `extmetadata` (LicenseShortName / Artist) at download time. These are NOT the photos used in the
  video itself (the video used the owner's own 16/09/2026 footage); first and only use is this notes
  page.
- **Not used:** no free-licensed photo positively identified as the Italian Garden was found, so
  Stop 7 has no thumb rather than a guessed one.
- **Used on:** Just Along Here Episode 4 (Pittencrieff Park) notes page, hero and stop images. Linked from
  `episodes.json` 27/09/2026.

## just-along-here/card-culross-1280x720.jpg

- **Upstream alias:** none — **deliberately deployed under its own name**,
  `Just Along Here\episodes\01-culross\card-culross-1280x720.jpg`. Byte-identical, md5
  `357aa1865f174a7358d9944ad39476a4`, verified on copy. Not renamed, applying the lesson from the
  Skye photo above: a rename across trees silently deletes the provenance signal.
- **Source:** a 16:9 crop of the episode's own hook/establishing photo, from the 4000×3000 original
  — a genuine downscale, no upscaling. Same photo as the video's opening beat, already logged in
  Just Along Here's own `assets.md`. No new source and no new licence question.
- **Licence:** CC BY-SA 4.0 — **attribution required, and it is burned into the image**
  ("Photo: Palickap, CC BY-SA 4.0, Wikimedia Commons", credit box bottom-left).
- **Supplied:** 06/09/2026 by Just Along Here, as the `cardImage` override for Culross.
- **⚠ DO NOT CROP THIS IMAGE, and do not strip the credit box.** The attribution travels *inside*
  the image; the card markup renders no credit line of its own. It is 16:9 exactly, so the card's
  `object-fit: cover` shows all of it — any future treatment that crops must either guarantee the
  credit survives or render its own.
  Legibility under the card's `.42` navy scrim verified rather than assumed: credit fill 25,
  text 118, delta 93.
- **Why it exists:** the `oar2.jpg` auto-frame for this episode cropped out its own burned-in credit
  and lost the monument's finial. See the note in `index.html` beside the disabled `oar2` path.

## unsolved-scotland/nls-glenforsa-mull-1956-ink.png

- **Derived here** 06/09/2026 from Unsolved Scotland's
  `brand\assets\nls-glenforsa-mull-crop-1956-hires.jpg`, via their own
  `brand\_panel-renders\_decompose_ink.py` (downscaled to 1600px first, then decomposed).
- **Source:** Ordnance Survey one-inch, Glen Forsa and the Sound of Mull, 1956
- **Licence:** National Library of Scotland, maps.nls.uk, **CC BY** — attribution required, and
  given in the Episode 2 notes page footer
- **Used on:** the Episode 2 notes page ground

## unsolved-scotland/ukho-iona-sound-2617-1860-ink.png

- **Upstream alias:** `Unsolved Scotland\brand\assets\ukho-iona-sound-2617-1860-ink.png`
  (byte-identical, md5 `41f8906be86857028eb868009fac317a`, copied 20/09/2026 — same filename both
  sides)
- **Source:** Admiralty Chart No. 2617, Sound of Iona, published 1860 (E. J. Bedford, Hydrographic
  Office) —
  https://commons.wikimedia.org/wiki/File:Admiralty_Chart_No_2617_Sound_of_Iona,_Published_1860.jpg
- **Licence:** public domain (UK government work, Crown copyright expired), per the individual
  Commons file page, re-verified by Unsolved Scotland (`episodes\04-netta-fornario\assets.md`)
- **Used on:** the Episode 4 notes page ground (also the episode thumbnail's ground)

## unsolved-scotland/os-overtoun-bridge-dumbarton-ink.png

- **Upstream alias:** `Unsolved Scotland\brand\assets\os-overtoun-bridge-dumbarton-ink.png`
  (byte-identical, md5 `4945a1bdd2856c57d775812949293a17`, copied 27/09/2026 — same filename both
  sides)
- **Source:** Ordnance Survey 25 inch 2nd edition, Dumbartonshire Sheet XXII.3, surveyed/published
  1898, National Library of Scotland (maps.nls.uk) — covers the Overtoun estate, showing the
  waterfall and footbridge (F.B.) the episode is about
- **Licence:** public domain (Crown Copyright expired — NLS's own copyright page states OS map
  Crown Copyright runs 50 years from publication; verified 27/09/2026 via maps.nls.uk/copyright.html).
  Attribution not legally required, but NLS's site convention is credited anyway (matches this
  project's existing house style for its other NLS/OS ground-ink assets) — no footer credit exists
  yet on either side as of this entry; add "Reproduced with the permission of the National Library
  of Scotland" to the Episode 5 notes page footer before it goes live, matching Episode 1/2's pattern.
- **Used on:** the Episode 5 (Overtoun Bridge) notes page ground — **not yet live**: staged by
  Unsolved Scotland (`INBOX-episode-05-ready-for-staging-unsolved-scotland.md`, 27/09/2026), asset
  verified and placed here ahead of the actual page copy-over, which is still pending a separate
  staging-ownership decision.
- **Visual check:** composited against a light background and inspected directly (not just a pixel
  range check, which misleadingly reads as flat since the real ink pattern lives entirely in the
  alpha channel, not RGB) — a real, legible 1898 map clearly labelled "Overtoun," matching the
  episode's subject.

## unsolved-scotland/nls-scotland-west-coast-1886-band.jpg · -ink.png

- **Source:** "Scotland: West Coast," Admiralty Chart 2635, Hydrographic Office, surveyed 1846–65,
  published 1886
- **Licence:** reproduced with the permission of the **National Library of Scotland**. Credit is
  rendered on the series index page and the Episode 1 notes page footer.
- **⚠ Needs confirming:** the exact licence label (CC BY vs a permission grant) is not recorded
  anywhere I can find — the pages say "reproduced with the permission of", which is a credit line
  rather than a licence name. Attribution is being given either way, so nothing is at risk; the
  record is incomplete rather than the usage. Unsolved Scotland owns the original sourcing.

## fonts/ — fraunces-variable, spectral-300/400/600

- **⚠ No licence record found** in either tree as of 06/09/2026. Both are widely distributed under
  the SIL Open Font License, which permits web embedding, but that has **not been verified against
  the actual files shipped here** and no record of where they were obtained exists. Self-hosted
  webfonts are exactly the case where a licence matters, so this should be confirmed and recorded
  rather than assumed.

---

## Rule for adding to this file

Any third-party-derived asset added to `site/assets/` gets an entry **before** it is referenced by a
page, recording: deployed filename, upstream alias if renamed, source URL, licence, whether
attribution is required, and where that attribution is rendered if so.

Publishing an asset that already exists elsewhere onto a new surface counts as a new publication and
needs the same check — that is `VISUAL-SOURCING-STANDARD.md` §11, written after this project shipped
the Skye photo to the homepage without checking its provenance first.

**Homepage `cardImage` needing attribution: prefer `episodes.json`'s `cardImageCredit` field over a
burned-in credit, decided 06/09/2026** (`VISUAL-SOURCING-STANDARD.md` §14). A burned-in credit
remains acceptable only when this file records an explicit do-not-crop guarantee for it, as the
Culross entry above does — that entry is grandfathered, not wrong, but any *new* `cardImage` needing
attribution should carry `cardImageCredit` instead, so a future re-treatment can't silently delete it.
