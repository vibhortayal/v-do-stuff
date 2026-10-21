# v_do_stuff — comic series vault

Canonical storage for the v_do_stuff Instagram comic series: locked characters,
source photos, strip scripts and final panels.

**Start here: [characters/LOCK.md](characters/LOCK.md)** — the character lock spec
(version, canonical files + SHA-256 hashes, locked traits, anti-drift workflow).
The characters cannot drift; any lock change needs the owner's explicit approval
and a new lock version.

Layout:
- `characters/refs/` — canonical character sheets (locked)
- `characters/source/` — owner-supplied identity reference photos
- `characters/archive/` — rejected/superseded versions, kept for the record
- `strips/` — one folder per strip: script + final panels
- `docs/` — profile audit + hash registry
