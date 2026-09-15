# Narration and media delivery status

Released app main `8121c11e16c65d06ae29163e452c8ea661d8e921` (0.1.17) includes the following bounded capabilities. Automatic deployment succeeded on September 15 at 18:46:24.150 UTC. Independent public verification at 18:47:18.933663 UTC matched all 462 distribution files by bytes and SHA-256.

- Media quality defaults to Medium, with Original available. The catalog contains 362 qualified derivatives; 32 unsuccessful preparations retain originals. The three timed English Scripture recordings retain their original audio. Representative native playback and image checks supplement per-file integrity and decoding checks; this does not claim every recording was heard.
- Narration defaults to Aquifer + AI fallback, with Aquifer only and AI only alternatives. Twenty-one English and two Spanish key-term recordings have exact source and asset bindings. Aquifer is a source label, not a claim about human production. Unmatched resources remain unavailable in Aquifer-only mode. Fresh-load failure may fall back to AI only in the fallback mode; restored checkpoints preserve recording identity.
- Verified offline saves follow the selected narration and quality, with explicit byte comparisons and atomic replacement. Shared resource layouts leave the final row accessible above the floating controls.

The active Spanish manifest contains 205 recordings, including eight descriptive visual narrations translated from accepted English descriptions and bound to the exact original images. Seven former title-only recordings remain historical assets. Three published Spanish Scripture editions remain available. English map labels are identified honestly in the Spanish descriptions. A bounded language-owned search found a candidate with English map labels; it did not establish a localized replacement or global absence.

Concise settings disclosure and automatic page completion marks are released. The shared Offline dialog uses the existing studio background across its entire light-theme surface and retains its original dark-theme backing. Preferences and saved status remain distinct without a redundant outer card.

Completion marks automatically follow ordinary playback completion of every referenced playable part on the current page, including the selected Scripture edition. A compact heading check button sets or clears a persistent manual override. Both states use the normal glass treatment; the check and pressed state distinguish completion. This supersedes the earlier manual-only bottom control. Seeking to the end follows ordinary player completion; the marks represent playback progress, not proof that anyone listened. Earlier visits do not become completion evidence. Navigation and existing Finish behavior remain unchanged.

All eight new visual recordings passed text, hash and decoding checks, with representative native playback checks. Direct auditory review remains unverified. The eight new recordings have qualified Medium alternatives totaling 380,149 bytes, compared with 2,948,698 bytes for their originals (87.11% smaller). Dedicated default-Medium playback and offline tests verified exact cached bytes, exclusion of unselected originals, and retention of the prior saved pack after a corrupt update.

A validation receipt initially reported three affected unit tests passing; its output actually showed two passes and one failure. The corrected assertion in `55f2acd` passed a fresh three-test run, independently repeated by the coordinator. The earlier receipt is superseded; native playback and asset qualification evidence are unaffected.

A separately discovered external BSB chapter-audio filename remains a candidate only. Current narrator and audio-specific rights are unverified, and boundaries for the selected passage have not been established. It is not integrated or labeled as Aquifer.

Source, validation limits and exact private receipts remain in the [authorized coordination journal](https://github.com/klappy/kitchen/blob/main/journal/2026-09-11-fia-functional-poc-cook.tsv). Earlier dated snapshots are historical.
