# Capability register

Primary runtime target: headed Google Chrome 152.0.7977.83 on macOS 26.2 build 25C5048a; responsive widths 320/390 pixels. Playwright Chromium is separate automation. Installed versions are reobserved at B3; physical-phone coverage remains untested. Current tools provide no proven audio capture/perception path: B3 probes early, and an unobservable mandatory audible result remains untested/partial without blocking implementation.

Status at planning: no app exists in the proposed home. “Planned / untested” is not working. The following statuses must be replaced only with observed results bound to an app commit, browser/version, date and evidence path. A mock or injected test is always labeled simulated.

| Action | Current evidence / status | Required actual behavior and fallback | Disconfirmer / limit |
|---|---|---|---|
| Open selected guide | Real source body returned; app untested | All six sections and source attribution visible; source failure is explicit | Missing/altered section, source mismatch or hidden required content fails |
| Select Scripture | BSB/ULT/UST each returned 13 verses; app untested | Exact selected source/version changes displayed and narrated Scripture; no silent language fallback | Wrong verse/version, fabricated text or unseen rights fails |
| Guided stop and continue | Full guide read; 130 unit hashes and 39 pauses bound; app untested | Every question/activity cue stops, shows applicable resource and requires explicit Continue | Linear autoplay through discussion, example-answer leak, stale cue hash fails |
| Resource exploration | 32 one-hop bodies/associations identified; 8 image HEADs 200; app untested | Real images/maps, all 21 terms and video descriptions/links accessible; Close returns to preserved guide context | Placeholder image, guessed map alias or browser media failure fails required item |
| Synthetic narration online | Browser API proposed; actual voice/events/audibility untested | User-triggered real SpeechSynthesis narrates exact selected source, labeled synthetic; pause/replay/cancel work | API presence/events alone do not prove audible output. No voice/error => unavailable, readable fallback; mandatory narration remains incomplete |
| Spoken commands / microphone | Outside bounded build; unresolved broader requirement | No microphone or speech-command claim; keyboard/touch navigation works | Typed/scripted intents cannot be marked successful speech; later inclusion requires actual mic action, ambiguity/denial/unavailable tests |
| Save passage | Finite source set identified; actual download/cache untested | Progress uses actual bytes/items; complete hash-verified pack alone earns Saved | Fake progress, partial pack, missing image or localStorage-only status fails |
| Use saved content offline | Planned / untested | Cold offline reload delivers shell, exact texts and all 8 images with saved position; video link says connection required | Online requests masking misses, open-tab-only success or single-item test fails |
| Synthetic narration offline | Planned / untested separately from data | Actual local voice speaks the saved source without a network connection | `localService=true` is an indicator, not audible proof. Failure leaves this required selected behavior partial |
| Pause / reload / resume | Planned / untested | In-session pause/resume at supported browser granularity; reload restarts same unit with explicit wording | Claiming exact audio position, losing selected version or running stale speech fails |
| Finish session | Planned / untested | Explicit Finish after all six steps visited; progress stored only on device | Does not establish understanding, participation, correctness or usability |
| Original guide recordings | Not included / untested | Website MP3 listings are references; synthesis is labeled | No original-audio, human-recording or timecode claim |
| Video playback | Online-only external links; HEAD success only | Clearly labeled destination and offline restriction | No video bytes downloaded/cached; playback remains untested unless independently observed |
| Physical phone / assistive technology | Untested | Responsive layout and keyboard paths tested in named desktop browser/viewport | Desktop emulation does not prove iOS/Android voice, storage, screen reader or field usability |
| Translation production / sync / AI answers | Excluded | No recording/upload/checking, shared-session service or generated answer interface | Any such dependency violates selected scope |

Selected source rights and modification notices are item-specific in [SOURCE-PACK](SOURCE-PACK.md), not inferred from website openness. No hosted model, cloud database, new paid service or credential is required. Browser/device speech capabilities may differ; do not hide that difference behind generic “voice supported.”

Final readback must distinguish working, simulated, unsupported and untested rows. A required row that cannot demonstrate the specified behavior blocks a full functional PoC claim even if an accessible fallback works. See [validation protocol](VALIDATION.md).
