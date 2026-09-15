# Guide completion — proposed plan

Planning only. Kitchen order `2026-09-15-fia-guide-completion-planning`, planning6 (author3/root2/coordinator1), does not authorize implementation. Source baseline app `8ef31b2c05b5907a6e01f15c05708174dae57479`; cookbook main `5ff8b9a`; Glass main `8d6b48dd93b6efa43305724a0cf320a85feabe5b`. Existing PR28 and resource-clearance work remain independent.

## Outcome and explicit semantic delta

Show an inline check for completed sections in the section index and for completed steps in the existing Guide step dropdown, in English and Spanish. A check means the facilitator explicitly marked that section complete on this device. It does not certify learning, participation or translation quality.

Current cookbook `poc/PLAN.md` defines Finish session after visiting six steps. The user now asks for actual completion rather than visits. Proposed supersession: opening, visiting, scrolling, choosing Next, reaching an audio end, seeking to the end, or opening a resource never creates a completion record. Add an explicit **Mark complete and continue** action to the shared guide presentation. It records the current section and advances to the next ordinary section. At the last section its label is **Mark section complete**. A completed section displays **Completed · Undo**, allowing correction without navigation. Existing Previous/Next remain navigation only. Group discussion cannot be established by a media event; a facilitator acknowledgement supports silent reading and offline use equally.

A step is complete only when every required ordinary section in that step has an accepted completion record. Session Finish becomes enabled only after all required sections across six steps are marked; it remains an explicit final action. Never backfill section checkmarks from historical `visited`, `visitedSections`, `finished`, audio offset or `completed` flags. Preserve reading position/version and existing legacy data; old finished status is historical, not evidence for new checkmarks. This tightening of Finish is a named plan change for root acceptance.

## Shared contract

One pure completion module/reducer, one storage boundary, one shared guide action/check presentation. Language adapters supply `{language, passageId, sections:[{id, stepId, sourceDigest}]}`. English uses `activeUnits`: hidden example region, attached pause aliases and metadata-only aliases do not become separate required checkboxes. An attached discussion is part of its primary section, not bypassed by an audio ending. Spanish uses `spanishGuideView(...).guide.groups.filter(ordinaryQueue)`; merged heading aliases resolve to their canonical group before lookup. Optional examples, Scripture editions, term recordings and resources do not add obligations or mutate guide completion.

Record schema1: `{passageId, language, records:[{sectionId, sourceDigest}]}` under a new completion-only local key. `sourceDigest` covers the ordered source body plus interaction/cue semantics used by that section; it is independent of narration provider, quality, playback checkpoint and Scripture edition. Require exact current ID+digest and the same language; invalid, duplicate or unknown records are dropped. Bound records to the current manifest's finite section count. On source revision, retain only exact matching section identities/digests. No inference from position, hashes belonging to another language or whole-pack revision. Existing checkpoint keys are not rewritten by marking completion.

Storage read errors produce empty progress with a concise persistence notice while preserving usable reading. Write failure may show the current session's explicit mark but must identify that it was not saved; reload cannot claim persistence. Removing an offline download preserves completion, as it preserves reading position. Undo removes only the chosen mark and derived step/session completion; it does not erase other progress or restart narration. No bulk-reset feature in this dish.

## Existing UI and design authority

Use the existing shared `GuideScreen`, GlassSelect and CatalogRow primitives. Native select option labels use a plain check plus accessible completion text (for example `✓ 2/6 · title · completed`); avoid fake rich HTML inside option elements. Section-index rows carry the same check and `Completed` accessible text. The current-location indication stays separate, so a checked row can be revisited without losing its check. Unchecked means not marked complete, not failed. Checks must remain legible without color in both themes.

The DS FIA kit explicitly proposes a Progress screen and `check` navigation icon, but its README says its structure is a proposal until the cookbook is available. Its example tracks books/chapters and includes invented sample readiness text; the current app is one passage with no corresponding completion data. Recommend **no new Progress page/tab now**: the requested inline surfaces answer “what have we completed?” beside the navigation used to continue. A later authorized summary may reuse this ledger and a distinct check icon; it needs a separate navigation/driver review. Do not duplicate English and Spanish screens or modify the independent FloatingDock clearance implementation.

## Bounded implementation proposal, not fire

One implementation dish proposed12: author7/root3/coordinator2, subject to coordinator allocation and root acceptance. It owns the shared completion reducer/storage, source adapters, shared mark/undo presentation, dropdown/index check labels and truthful Finish migration. Coordinate App/SpanishSession integration after the clearance worker freezes; no shared active-file writes. No DS core fork, new tab, backend, telemetry, recording, synchronization or assessment model.

Acceptance gates:
1. Pure state tests: visit/next/audio end/seek do not mark; explicit mark/undo derives exact step completion; final-step jump cannot finish; all required sections can finish; optional/alias sections do not inflate denominator.
2. Persistence: old visited/finished values produce zero new marks; exact marks survive reload/offline and language roundtrip; another language/digest/unknown ID cannot mark; corrupt/quota-denied storage is truthful and preserves position.
3. Shared native English/Spanish: mark→continue, checked dropdown/index, revisit→undo, current-row distinction, keyboard/focus, 319/390/726 widths, both themes. Retain playback owner/paused offset while inspecting index and undoing; advancing uses existing navigation's stop behavior, no automatic audio play.
4. Independent root source and actual screenshot review, applicable existing tests/content/build checks and exact-head CI/Bugbot/release gates. Planning acceptance is not implementation PASS.

Return if authoritative source grouping cannot produce stable ID+digest, if a migration would fabricate completion, or if root rejects explicit facilitator acknowledgement semantics. Do not substitute visit/audio heuristics. Expected benefit: visible section/step completion without a second tracking screen or a new navigation habit; measure by native ability to identify completed work and resume an unmarked section in the same index, not by invented time-saved figures.
