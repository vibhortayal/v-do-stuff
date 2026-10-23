# CHARACTER LOCK — v_do_stuff

**Lock version: v1.3 — revised 2026-10-23 per Vibhor's instruction to lock the strip 013 characters and update the prompt/reference.**
(v1.1 added the generation + lettering pipeline; v1.2 adds the house design canon; v1.3 updates the shared character descriptions and adds strip 013 visual references.)
Rule zero: the characters CANNOT drift. Continuity across every strip depends on this file.
Any change to a canonical file below requires the owner's explicit approval, a new lock
version, and a changelog entry. No agent may silently re-lock, substitute, or "improve"
a canonical reference.

## Canonical references (verify SHA-256 before every use — see docs/HASHES.txt)

| File | Subject | SHA-256 |
|---|---|---|
| characters/refs/wife-styleA-lock-v2.webp | Existing wife canonical sheet | 2f9ca69bc7fc121ca1c4f8197a7219c04370ad3ab011b6e9490d1b02a394bfd9 |
| characters/refs/vibhor-styleA-lock-v1.webp | Existing Vibhor canonical sheet | 806bc814078811358152f3e443f02b4bdd9e1f455ece237a37c99f4b52ca430f |
| characters/refs/pair-styleA-slide1.webp | Existing pair in-scene reference | 67b9096066657b33da5603c500df38c7b45907db0f1c85444b6f9e096e5ee1a3 |
| strips/013-exhibit-a/013-s1.png | Strip 013 final visual reference — Vibhor | 772e003ed657815f567d6f523981ad4ebeab00d3833579b143f220050dd979cd |
| strips/013-exhibit-a/013-s2.png | Strip 013 final visual reference — pair | 64af306ba436076800fd1e6bb5d3032322f9a2254fef03b2d6b9b3905314cf56 |
| strips/013-exhibit-a/013-s3.png | Strip 013 final visual reference — pair | 5c8d176b5a095e679ce1788ea5ac212e6242a207c65b0162bfc8dd3aa1375e80 |

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

**House design (canon — owner 2026-10-21, "consistency in the house design"):**
The apartment is ONE house across all strips; interiors must not change between
panels or strips.
- Kitchen cabinets: WHITE (uppers and lowers), simple round knobs. (Generator
  defaulted to wood in strips 013 slides 1–2 — corrected; slide 3 already white.)
- Kitchen: light stone countertops, stainless sink, warm under-cabinet light.
- More house details get added here as the owner calls them — when he names a
  house feature, it becomes canon.

**Process rules:**
- Generate the SCENE ONLY — no text, no speech bubbles, no letters baked into the
  art. One panel at a time; for edits, reference the panel and edit only that
  vignette.
- LETTERING IS A SEPARATE STEP, done by the agent (never the image generator):
  speech bubbles + caption band added in post. This is law — generator lettering
  produced typos ("untuched") and baked-in header lines on 2026-10-21.
  Placement rule (owner 2026-10-21: "the bubbles are blocking the faces"):
  bubbles live in negative space only (cabinets, walls, window, counter) and
  NEVER cover a face — eyes, glasses, nose, mouth stay fully visible. Tails
  point to the speaker and may touch a hairline or shoulder edge only. Check
  every lettered panel for face coverage before presenting.
  Corollary (owner 2026-10-21, after a bad pass): a bubble wedged BETWEEN the
  two heads, resting on hair or jabbing a tail at glasses, is a FAIL even if
  no facial feature is technically covered. Corners and edges of the frame
  first; when in doubt, move the bubble to the counter/sink zone. The agent's
  own pass is not sufficient evidence — when the owner asks, an independent
  review checks placement, and its fails get fixed, not argued.
- Format: vertical panel with a white caption band below (target 1080x1250);
  caption short and understated.
- QC before presenting: faces identical to the approved strip; extra hands; odd
  fingers; mirrored errors; spelling (trivially guaranteed by separate lettering);
  heights/proportions per the rules below.

## Vibhor — locked traits (v1.3)

- Age-appropriate face (41), medium-brown skin, slight tired lines.
- Thin round wire glasses; short neat dark hair, close on the sides, only slightly wavy on top, with a few gray flecks. NOT curly, thick, or voluminous.
- Short trimmed stubble beard. Lean, natural build.
- Outfit changes with scene; in strip 013 he wears an olive henley.
- Use the strip 013 final panels above as current visual examples, alongside established identity references.

## Kajal — locked traits (v1.3)

- Dark black-brown hair just past the shoulders, straight with a slight wave and a side part.
- Warm medium skin; soft, dimpled smile; minimal makeup.
- Small stud earrings. Side characters must look clearly distinct from her.
- Outfit changes with scene; in strip 013 she wears a soft blue top.
- Use the strip 013 final panels above as current visual examples, alongside owner-supplied identity photos when available.

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

- v1.3 — 2026-10-23: Shared character descriptions updated per Vibhor's explicit instruction to lock these characters and update the prompt/reference. Vibhor: age-appropriate 41-year-old face, thin round wire glasses, short neat dark hair only slightly wavy, short trimmed stubble, lean build. Kajal: dark hair past shoulders with slight wave and side part, soft dimpled smile, small studs. Strip 013 final panels added as visual references. Outfit may change by scene.

- v1.0 — 2026-10-21: Initial lock. Wife sheet v2 (photo-built, owner: "this is the
  closest"). Vibhor sheet v1 (photo-built). Style A adopted. Heights/proportions rules
  recorded. Strip 012 "Said Out Loud" committed as the reference strip.
- v1.1 — 2026-10-21: Design system added per owner's instruction ("all future strips
  should adhere to these"): warm semi-realistic animated style (no photo-realism),
  mandatory refs (approved couple strip + published strip photo), scene-only
  generation, lettering as a separate agent step, vertical format with caption band,
  QC checklist. Two published panels added to characters/refs/ as style references.
  Strip 013 is the first strip rebuilt under this pipeline.
- v1.2 — 2026-10-21: House Design canon added (owner: "consistency in the house
  design. cabinets white"). Kitchen cabinets are WHITE in canon; strip 013 slides
  1–2 corrected to match slide 3.

