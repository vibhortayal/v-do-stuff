# CHARACTER LOCK — v_do_stuff

**Lock version: v1.0 — locked 2026-10-21 by Vibhor Tayal (owner).**
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
