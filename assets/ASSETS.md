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
