# CHARACTER LOCK — v_do_stuff

**Lock version: v1.1 — locked 2026-10-21 by Vibhor Tayal (owner).**
(v1.1 adds the mandatory generation + lettering pipeline in the Design System
section below — owner instruction 2026-10-21: "all future strips should adhere
to these." The v1.0 character locks are unchanged.)
Rule zero: the characters CANNOT drift. Continuity across every strip depends on this file.
Any change to a canonical file below requires the owner's explicit approval, a new lock
version, and a changelog entry. No agent may silently re-lock, substitute, or "improve"
a canonical reference.

## Canonical references (verify SHA-256 before every use — see docs/HASHES.txt)

| File | Subject | SHA-256 |
|---|---|---|
| characters/refs/wife-styleA-lock-v2.webp | Wife — canonical sheet | 2f9ca69bc7fc121ca1c4f8197a7219c04370ad3ab011b6e9490d1b02a394bfd9 |
| characters/refs/vibhor-styleA-lock-v1.webp | Vibhor — canonical sheet | 806bc814078811358152f3e443f02b4bdd9e1f455ece237a37c99f4b52ca430f |
| characters/refs/pair-styleA-slide1.webp | Pair in-scene reference | 67b9096066657b33da5603c500df38c7b45907db0f1c85444b6f9e096e5ee1a3 |

Source photos the sheets were built from live in characters/source/ (owner-supplied).
Rejected/superseded versions live in characters/archive/ with the reason in the filename —
never promote an archive file back to canonical without a new lock version.

## House style (owner decision 2026-10-21, A/B tested)

**Style A** — warm semi-realistic painterly illustration, matching the existing published
v_do_stuff strips. (A softer flat comic style was built and retired the same night;
see archive. Do not revive it for strips without the owner's word.)

## Design system — MANDATORY pipeline for every strip (owner, 2026-10-21)

All future strips are produced exactly this way. Deviations need the owner's word.

**Style target:** cartoon illustration, warm semi-realistic animated style, soft
cinematic lighting, NO photo-realism. (Photo-real generation was attempted and is
not available; flat watercolor "sketch" renders were rejected by the owner as
drift. The approved reference look is the published strips: warm palette, cinematic
indoor warmth, bold clean rendering.)

**Mandatory attachments for every panel generation:**
1. The approved couple strip — characters/refs/pair-styleA-slide1.webp — faces come
   from here (plus the canonical sheets above); keep both faces identical to it.
2. A published strip photo for palette/style — characters/refs/
   published-style-ref-kitchen.jpg (hosting/chores panel) or
   published-style-ref-fineprint.jpg.

**Base prompt (owner-supplied, use verbatim as the style block):**
"Cartoon illustration, warm semi-realistic animated style, soft cinematic lighting,
no photo-realism. Use the attached reference images for the two main characters
and keep their faces identical. Vertical 1080x1250, white caption band below,
rounded sans-serif text, short understated caption. Check for extra hands, odd
fingers, mirrored errors."

**Process rules:**
- Generate the SCENE ONLY — no text, no speech bubbles, no letters baked into the
  art. One panel at a time; for edits, reference the panel and edit only that
  vignette.
- LETTERING IS A SEPARATE STEP, done by the agent (never the image generator):
  speech bubbles + caption band added in post. This is law — generator lettering
  produced typos ("untuched") and baked-in header lines on 2026-10-21.
- Format: vertical panel with a white caption band below (target 1080x1250);
  caption short and understated.
- QC before presenting: faces identical to the approved strip; extra hands; odd
  fingers; mirrored errors; spelling (trivially guaranteed by separate lettering);
  heights/proportions per the rules below.

## Vibhor — locked traits

- Short STRAIGHT black hair, neatly cropped, grey at temples. NEVER curly/voluminous.
- Short trimmed beard + moustache, grey flecks on chin.
- Round thin metal glasses. Broad toothy grin. Medium build.
- Black smartwatch on LEFT wrist. Default outfit: navy crew-neck sweater, dark jeans.
- Height 5'10" (178 cm).

## Wife — locked traits

- Long STRAIGHT black hair, slightly OFF-CENTRE part, low volume, past shoulders.
  NEVER wavy, curly, or brown.
- Soft oval face — full but NOT too round (owner rejected both the too-round v1 and the
  over-slimmed v3; v2's balance is correct — do not slim or round her further).
- Straight FLAT brows (not arched). Medium almond eyes, minimal makeup, no glam.
- Medium straight nose, slightly broader base. Warm medium skin.
- Signature smile: wide, upper teeth, cheeks up, eyes crinkling, DIMPLES in both cheeks.
  Even laughing: NO deep smile lines, nasolabial folds, crow's feet, or under-eye bags —
  she must always read pretty, fresh, rested.
- Small hoop earrings. Default outfit: sage green sweater/top, light trousers.
- Height 5'6" (168 cm).

## Proportions & heights (both, every panel)

- Only 4 inches between them: her crown reaches his EYE/NOSE level, never chin/shoulder.
  Generators default her to ~5'1" next to him — calibrate her UP on purpose.
- Natural adult proportions: head ≈ 1/7 of body height. No big-head/chibi framing.
- Frame waist-up or wider by default.

## Anti-drift workflow (mandatory for every generation)

1. Start from the canonical sheet files in this repo — verify hashes first.
   NEVER redraw a character from a text description alone.
2. Build panels by editing/anchoring on the canonical refs and the scene's prior slide;
   keep seats, outfits, and scene consistent within a strip.
3. Before presenting any panel, check both faces against the canonical sheets trait by
   trait. If a face fails, regenerate the panel — never present a drifted face as final.
4. Finished strips are committed under strips/<nnn-name>/ with script + final panels,
   and their hashes appended to docs/HASHES.txt.
5. If a generation session starts returning drifted strangers/wrong styles repeatedly,
   stop and retry in a fresh session rather than forcing more calls.

## Changelog

- v1.0 — 2026-10-21: Initial lock. Wife sheet v2 (photo-built, owner: "this is the
  closest"). Vibhor sheet v1 (photo-built). Style A adopted. Heights/proportions rules
  recorded. Strip 012 "Said Out Loud" committed as the reference strip.
- v1.1 — 2026-10-21: Design system added per owner's instruction ("all future strips
  should adhere to these"): warm semi-realistic animated style (no photo-realism),
  mandatory refs (approved couple strip + published strip photo), scene-only
  generation, lettering as a separate agent step, vertical format with caption band,
  QC checklist. Two published panels added to characters/refs/ as style references.
  Strip 013 is the first strip rebuilt under this pipeline.
