# Capability register

The September 14 section below is the current status. Earlier dated snapshots, including unavailable-narration statements and distribution totals, are historical evidence.

Original delivery result 2026-09-11: **usable partial PoC**, English Mark 1:1–13 only. Implementation validated at private app commit67b2d704b952c20b3cda953a60b07b2b4c4138a9. The [private delivery evidence](https://github.com/klappy/fia-functional-poc/blob/main/evidence/DELIVERY.md) and authorized kitchen receipts bind exact tests and subsequent documentation revisions. Private links require access; their existence is not public access to voice media or source evidence.

The current user-authorized implementation uses prepared ElevenLabs synthetic recordings. This supersedes the planning-stage browser-speech implementation choice; browser voices remain optional fallback. No runtime provider key or synthesis call is needed. **Human-heard online/offline quality remains unverified**, so the mandatory narration acceptance row and overall result are partial despite successful media playback.

| Historical delivery action | Historical status | Evidence boundary / limitation |
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

## Current merged implementation

Release-state snapshot, 2026-09-12 UTC: shared inset controls, resource reading-order corrections and install support are released at app main `97cd571`. At that historical revision, HTTP readback verified five critical release assets; the new whole-distribution result is recorded below. Spanish text/media is released at app main `e4a040fef5c5ba4dc8cfb711f4943dcd632ca1d9`. Deployment succeeded on 2026-09-12 at 14:35:54.513 UTC; HTTP readback matched all 210 distribution files byte-for-byte and by SHA-256 (102,177,627 bytes), including the Spanish pack, five media assets and offline manifest. The English required pack contains 200 files (93,643,276 bytes). Selectable Spanish text/media is available through Languages; narration remains unavailable. Nested Guide navigation is released at `5eb1fec`; bounded secondary-control contrast corrections are merged at `1eadcbd`.

The [contextual playback record](CONTEXTUAL-PLAYBACK.md) supersedes the historical numerical and reload behavior above. The current bounded pack has 111 visible activities preserving 130 source units / 39 raw stops, three English Scripture versions, 32 resources and 172 stored recordings. The current English required pack contains 200 files, including install metadata and icons; exact bytes and released revision are bound in private delivery receipts.

| Action | Current capability | Remaining limit |
|---|---|---|
| Guide, Scripture and resource playback | Source/output-verified prepared audio, 0.95× rate, 750 ms automatic guide gap, explicit discussion stops; 171 recordings unchanged by the latest single-map correction | One revised map clip accepted by a listener; representative whole-guide/Scripture and offline heard quality remain untested |
| Local workspace restoration | Theme, view, source position/version, resource query/filter/selection and verified unfinished audio checkpoint restore; audio remains paused until explicit Resume | Last successful local checkpoint, not exact crash-time recovery or account sync; invalid/stale/storage-denied data handled explicitly |
| Contextual controls | Guide/Scripture shared inset controls; resource rows follow source/keyboard order, with a shared floating transport; full card surfaces open details while Play/Restart remain independent | Discussion and Finish stay at the end of source content; completion is an explicit choice, not inferred learning |
| Offline pack | 200 English required files verified before Saved, with atomic replacement and real local cold-offline playback tests | Public live browser/offline check unavailable because its policy check could not complete; historical HTTP 195-hash verification is narrower and does not verify the newly merged revision |
| Public hosting | Automatic GitHub-main Cloudflare deployment at [fia.klappy.dev](https://fia.klappy.dev), static reviewed bundle only | Build completion and HTTP verification are distinct from browser, heard-quality and physical-device acceptance |
| Install support | Installable app metadata/icons and browser-dependent install guidance; installing the app and saving a passage are separate actions | Physical OS installation remains unverified; a saved shell does not imply its passage or audio is saved |
| Second language | Selectable Spanish text/media, six guide steps, reviewed sources and labeled supplements; release receipt above | Spanish narration remains unavailable; complete audio-first acceptance remains pending |

The current result remains **usable and partial**. No retrospective weakening of the [original validation contract](https://github.com/klappy/fia-app-cookbook/blob/2d90436c80b0c5aa2f18bc7594347b1d6244e704/poc/VALIDATION.md) is implied.

## September 14 verified release

The earlier publicly verified app main `51e653bc` provided 34 Spanish resources, two original Scripture editions and 191 prepared Spanish recordings. Original source records and item-specific rights remain intact. Three proposed AI-derived Scripture editions were withdrawn, not added to the authorized recording set. Maps retain their original image pixels; videos remain explicit external links. Natural spoken reference replacements preserve the displayed source text.

Released app main `62d28f5` adds published Door43 Spanish ULB v1.4 with provenance, attribution and 13 prepared verse recordings: three authentic Spanish editions and 204 recordings in total. Version 0.1.9 passes the exact 418-file build audit; deployment and independent HTTP readback verify all 418 files (216,682,503 bytes) at the final main revision. The existing unchanged deployment pipeline was invoked manually once after the final automatic build did not appear.

The released app uses shared Guide, Scripture, Resources and full language-picker components. Current-language confirmation returns to content without a fetch or autoplay. Failed optional audio loading retains accessible text and truthful availability. Resource previews stay concise; details retain one attribution section, contextual description and external-video body. Source video links open separately without leaving the passage; empty source anchors are excluded. Native dropdown option styling has bounded checks; native OS popup rendering remains unverified.

Actual clip identities drive released highlighting. Spanish verse clips support verse-level highlighting; full-passage English recordings retain passage-level highlighting. The September 15 candidate described below adds English timing; it is not yet a verified public capability. Automatic synthetic introductions are disabled by operator policy, while unseen source-specific notices remain distinct. Explicit Info replay preserves paused content progress.

## September 15 alignment candidate

Candidate `c93e29d` (version 0.1.10) adds source-bound English word and verse timing for BSB, ULT and UST in the shared Scripture view. Three initial forced-alignment requests completed after upload permission was enabled; no retries or replacement recordings were needed. Exact build verification passes 421 distribution files and 203 required English offline files. Release gates and public readback remain pending; the public release above remains the verified baseline.
