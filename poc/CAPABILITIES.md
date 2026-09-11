# Capability register

Original delivery result 2026-09-11: **usable partial PoC**, English Mark 1:1–13 only. Implementation validated at private app commit67b2d704b952c20b3cda953a60b07b2b4c4138a9. The [private delivery evidence](https://github.com/klappy/fia-functional-poc/blob/main/evidence/DELIVERY.md) and authorized kitchen receipts bind exact tests and subsequent documentation revisions. Private links require access; their existence is not public access to voice media or source evidence.

The current user-authorized implementation uses prepared ElevenLabs synthetic recordings. This supersedes the planning-stage browser-speech implementation choice; browser voices remain optional fallback. No runtime provider key or synthesis call is needed. **Human-heard online/offline quality remains unverified**, so the mandatory narration acceptance row and overall result are partial despite successful media playback.

| Action | Current status | Evidence boundary / limitation |
|---|---|---|
| Open selected guide | Working | All six steps,130 source units;117 ordinary units in guided flow. Canonical source comparison and fresh clean-checkout execution pass. |
| Select Scripture | Working | Three English versions each contain13 verses; selected version and source position persist locally. No translated-language coverage. |
| Stop/discuss/continue | Working |39source-bound stops; independent117 unit browser traversal, all six steps. Explicit Continue; no inferred group participation or learning. |
| Examples | Working |13 example units excluded from automatic navigation/narration; explicit source-example reveal preserves original text. |
| Resources | Working |32 associations:21 terms,4 maps,4 photos,3 online video links. Eight actual images decoded/read back offline; full map detail preserves source aspect and legends. No expert geographic certification. |
| Synthetic playback online | Working media behavior; mandatory heard quality untested | Selected source/hash/MIME/bytes verified before playback. Actual play/pause/resume/end/cancel observed. No agent-heard or human-quality claim. |
| Save passage | Working |137local files, about 48.3 MB, complete transfer and cached readback before Saved. Failed replacement preserves previous valid pack. |
| Offline content and playback | Working tested behavior; heard quality untested | Fresh-page offline reload verifies every required file, displays source/resources and plays prepared audio. Full browser/OS restart and physical phones untested. |
| Pause/reload/resume | Working bounded behavior | In-recording pause/resume; reload restores guide unit/version, not sample-accurate audio position. |
| Saved-version update | Working | Ordinary reload upgrades prior saved shell; position and old pack remain until verified explicit replacement. |
| Finish | Working | Explicit finish after visiting all six steps. It certifies no understanding, participation or translation quality. |
| Full design-system composition | Working within tested desktop views | Complete pinned shared CSS and actual components; aurora/glass and FIA identity. Source/event/accessibility wrappers retain useful guide/Scripture/resources structure. |
| Failure fixtures | Simulated | Quota, missing/corrupt transfer and injected media cases are failure tests, not evidence of heard speech or field reliability. |
| Browser fallback | Optional, separately bounded | Device speech behavior varies and is not the selected quality acceptance. |
| Original recordings / video playback | Unsupported in this slice | Synthesized recordings are labeled. Video descriptions and external links only; no downloaded or observed-playback claim. |
| Microphone / translation / sync / AI answers | Unsupported in this selected slice | Spoken app-driving remains an unresolved broader requirement, not a governing-scope exclusion. No microphone commands, recording, translation checking/upload, synchronized sessions or generated answers are implemented here. |
| Physical phones / assistive technology / field use | Untested | Desktop responsive and keyboard evidence does not validate iOS/Android, screen readers, group learning or oral-audience usability. |

Independent fresh validation used Node 22.16.0/npm 10.9.2 on macOS 26.2 build 25C5048a with Playwright Chromium 153.0.8010.12. Separate coordinator headed-Chrome 152.0.7977.83 observations are distinguished in private evidence. Responsive widths 320/390px, keyboard/focus and CSS 200% large-text checks pass; CSS zoom is not a new native-zoom observation.

The original eight image assets ship; a compression experiment was not adopted. Optional network fonts and videos are not cached. Full stylesheet inclusion does not imply unavailable font binaries shipped; rendered local fallback is observed. Per-item [source notices](SOURCE-PACK.md) remain authoritative, with unresolved holder metadata preserved. No blanket legal, geographic, theological or whole-corpus claim.

Broader source-local extraction, audience assessment and history remain open. The governing scope review covers the available recordings with private coverage limits; it cannot prove unrecorded material did not exist. See [validation](VALIDATION.md) and [source access](../SOURCES.md).

The [subsequent contextual playback correction](CONTEXTUAL-PLAYBACK.md) records the expanded term narration and explicit exploration-continuity supersession. The original numerical test/pack totals above describe the historical delivery, not the latest candidate. Exact final correction results remain bound to the private delivery record.
