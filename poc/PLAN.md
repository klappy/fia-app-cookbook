# Functional PoC plan

Historical planning status: proposed, prepared for independent review. No app behavior is implemented by this plan. Binding and publication receipts belong to the authorized coordination home linked in [Sources](../SOURCES.md). This plan selects a preliminary mobile-web experience, not the complete first release or the whole FIA corpus.

Confidence: high in the inspected source identity and reviewed scope boundaries; moderate in implementation feasibility on the named desktop browser; unknown for actual audible/offline behavior until build verification. This is one bounded experiment, not a universal product rule or superiority claim. A failed mandatory capability retracts the full-functional verdict.

## Scope and authority

The current task designates one complete source set as authority. Independent review checked the complete exposed source set, observed revision stability and retrieval exhaustion. This does not establish that every real-world utterance was recorded. Exact coverage counts and a retained catalog-count discrepancy are recorded privately. Exact identities, revisions and witnesses stay in the access-controlled evidence ledger. No later source was found and accepted as an explicit supersession.

| Neutral scope record | Disposition and rationale |
|---|---|
| ISR-01 | Include oral-first familiarization, internalization and articulation to help people understand Scripture. Optional text supports the experience. |
| ISR-02 | Include one device used individually or by a co-located group. Exclude recording, checking, uploading translation output and synchronized multi-user sessions. |
| ISR-03 | Exclude publication/distribution of a group's translation output; this is a different workflow. |
| ISR-04 | Include contextual resources and intentional stop/discuss/resume behavior. A deterministic source flow is permitted. |
| ISR-05 | Spoken app-driving remains desired but unresolved as a required initial capability. It is outside this bounded build; accessible controls are not relabeled spoken input. |
| ISR-06 | Synthetic narration is required for this selected slice, with explicit synthetic disclosure. Recognition and human audio recordings are separate capabilities. |
| ISR-07 | The broader first phase seeks complete process and assets. This preliminary PoC covers all six steps of one passage with its selected necessary resources; it cannot be called the complete FIA experience. |
| ISR-08 | Include saving needed content for later offline use. Do not download videos. Local hotspot/server deployment is a separate later product. |
| ISR-09 | Phone portrait is the design target; mobile web is an expressly preliminary feedback vehicle. Desktop-browser viewport testing cannot prove physical-phone usability. |
| ISR-10 | Exclude runtime generated UI, custom map authoring and coach/network systems. |
| ISR-11 | This build uses English only. Broader language candidates remain future scope, not inferred localized coverage. |
| ISR-12 | Verify selected resource identities, rights and actual bodies; incomplete catalog tags are not permission to invent timings or assets. |
| ISR-13 | Existing ownership boundaries remain intact. A private development repository does not settle production distribution ownership. |

[Official website terminology](../references/FIA-WEBSITE.md) informs the domain: three overarching concepts and six passage steps are different levels. Broader translation drafting there does not expand this app boundary. Interpretive oral-audience research informs design, not validated personas. Existing requirements and journeys remain hypotheses outside the accepted bounds of this specific build.

## Smallest complete scenario

A facilitator opens Mark 1:1–13, selects BSB, ULT or UST, hears synthetic Scripture and guide narration, and leads all six source steps. The app stops for questions and physical/group activities, reveals the associated image, map or term when relevant, and waits for an explicit Continue. The facilitator may inspect another associated resource and return to the same step/unit. Example drama answers remain hidden until explicitly requested. Participants speak or enact in person; the app captures no speech or translation.

Before disconnecting, the facilitator selects Save this passage. A finite pack contains the full guide, three 13-verse Scripture versions, 21 associated term articles, four maps and four images, plus three online-only video descriptions/links. Actual transferred items and bytes determine progress. Only a verified complete pack earns Saved. Offline reload restores the source position and selected version; all saved text and eight images remain available. Videos clearly require a connection. Browser-local synthetic voice support must be demonstrated separately for offline narration.

Completion is the user's explicit Finish session action after all six steps have been visited. It does not certify learning, translation quality, group participation or field readiness. The app keeps only passage/step/unit/version and visited-step state locally. No accounts, personal profiles, analytics, cloud state or content submission.

## Source and interaction contract

The [source pack](SOURCE-PACK.md) binds the guide, source revisions, assets, rights and aliases. Preserve exact guide/scripture meaning. Sanitized HTML may retain headings, paragraphs, lists and emphasis; display-only segmentation is identified as an app adaptation. Do not silently correct or complete source claims. Show source title/version and review level, attribution, modification notice and license links.

The six guide h2 sections are authoritative. Assign stable `S01`–`S06` steps and `U001...` paragraph/list-item units within each section; flatten leaf paragraphs and list items once, never double-read a list container. The cue manifest stores the exact source-text hash of each unit. A build fails if an upstream change invalidates it. It is not original audio time alignment.

Narration may split a long unit at sentence boundaries without altering its text, but advances the guide unit only after every chunk actually completes. Chunk position is transient; saved position remains the source unit. A timeout/error cancels and offers replay, never silently skips content. Narration advances units on actual speech completion. At a question, activity or configured resource cue, enter `discussion`, reveal the specified resource and stop automatically. Continue requires a click or keyboard action. Resource exploration preserves the suspended guide unit; Close restores focus to the opener. Jumping step/version cancels old speech before updating state. Pause/resume within a unit uses actual browser events; reload or unsupported pause restarts the current unit with clear wording. Never claim sample-accurate audio resume.

The selected guide contains example drama responses. Hide the complete example region beginning S04-U017 behind “Show source example”; do not automatically narrate it. All original text remains accessible in the source view. The user can move directly to the next step without opening examples. Question-like and activity units must be independently checked against the full source so no response is inadvertently narrated before the group responds.

## Technical decision

Primary runtime target: headed Google Chrome 152.0.7977.83 on macOS 26.2 build 25C5048a, observed by coordinator and independently confirmed for Chrome. Test responsive widths 320 and 390 pixels on that desktop browser; physical phones remain untested. Playwright Chromium is a separate automated-test target and cannot substitute for headed-browser or audible-output evidence. Reobserve installed versions at B3 and record any difference.

Available tool inventory and CUA expose visual/accessibility interaction but no proven audio capture/perception capability. B3 first probes the actual browser voice/output observation path. A legitimately available system-output-only loopback method may be used if verified; no microphone/ambient/private capture or safety bypass. Unverifiable audibility permits continued implementation and a usable artifact, but leaves the required audible row untested and the final result partial. No capture tool is promised.

Proposed home: new private `klappy/fia-functional-poc`, default branch `main`. Authenticated name lookup found no accessible repository; B1 must create and read back the actual name, visibility and branch before app changes. The coordinator has accepted proposing this reversible home; independent plan acceptance remains required. If creation fails or a collision appears, hold B1 and resolve the actual home, never change visibility or overwrite another repo.

Use React 19.3.0, React DOM 19.3.0, Vite 8.3.0, @vitejs/plugin-react 6.1.1, DOMPurify 3.4.15 and @playwright/test 1.63.0, exact versions plus lockfile. Node 22.16.0 observed satisfies Vite's >=22.12 engine. Optional compiler peers are not required. No React compiler configuration. A static Vite build uses same-origin versioned source files and assets; the content adapter rewrites each selected media reference to its manifest path and prevents incidental remote image/thumbnail loads. Other source links remain labeled explicit external navigation, not prefetches; no runtime backend or credential. `npm ci`, `npm run test`, `npm run build`, `npm run test:e2e`, `npm run preview -- --host 127.0.0.1 --port 4173` are the delivery commands. Include source verification and accessible failure paths in tests, not implementation-mirroring test volume.

Speech uses browser SpeechSynthesis after a user gesture, with an English local voice preferred and visibly identified. Voice enumeration, successful speech events and actually heard output are separate evidence levels. No voice or error produces an explicit unavailable state with readable content and navigation, not a simulated success. No microphone API, AI inference service, voice cloning, secret or new financial commitment is required.

Service worker and Cache Storage implement one versioned passage pack. Fetch into a staging cache, verify HTTP success and expected SHA-256 for every required resource, then atomically publish a manifest pointer. Failed/cancelled/quota-limited updates never replace a valid old pack. A corrupt or missing required entry invalidates Saved on readback. Application shell is separately cached after a successful online load. Clear passage removes the pack after confirmation, preserving shell and harmless progress. No offline completeness claim is based on localStorage alone. Browser storage eviction remains possible and is detected. Use exact current manifest bytes when calculating displayed download size; roughly 23 MB of original image assets is a planning estimate, not a promised quota.

## Design-system use and alternatives

Pin Generative Glass `8d6b48dd93b6efa43305724a0cf320a85feabe5b` and record copied paths in UPSTREAM.md. Recheck main at fire; inspect relevant changes without chasing a redesign or silently repinning. Reuse shared tokens, icons and Glass primitives through a thin app layer. Do not import the kit's fake sync state, Record button, invented prompts or fixed phone frame. Use responsive width and readable controls. Use system fonts; unverified font binaries and runtime font-CDN dependence are omitted and recorded as a deliberate divergence.

The inspected sheet lacks complete modal focus behavior. Use an app-level native dialog with focus return/escape and accessible labels around shared visual primitives; do not fork a replacement design system. Shared-core improvements go to existing upstream issues 1–3 or a concrete separate request.

| Six B | Verdict | Specific evidence, criterion and consequence |
|---|---|---|
| Borrow | applied | In this design, select Glass at the pinned SHA and actual Aquifer sources in SOURCE-PACK; implementation still pending. Reuse the design vocabulary and content provenance. |
| Bend | applied | Adapt the illustrative FIA kit to six source steps, truthful storage/narration states and responsive dimensions through an app layer. |
| Break | observed | Kit mock sync/Record/three prompts and missing focus containment cannot satisfy this source-guided slice; these are inspected gaps, not a general quality ranking. |
| Beget | delegated | Auggie owns subsequent B1–B4 ordering/dispatch and independent validation. Proposal is not worker acknowledgment or fire. |
| Bide | inspected-and-rejected | conversational-bible-translation-poc at adefef4b58ea934ca4c6c333c824fb539e8f5d64 provides contextual-canvas ideas, but its Netlify/chat/translation topology conflicts with the bounded purpose and adds gross overcomplication. unfoldingtheword at cb6370c8a20124bdc730321638a60c39217a9485 introduces Supabase/AI dependencies. Legacy offline_bible_app setup does not prove offline behavior. Aquifer Window visual patterns inform shared Glass reuse; its production app repository was not resolved and is not cited as implemented code. |
| Build | not-yet | Only the missing source-unit/cue orchestration, truthful speech adapter and verified pack lifecycle are proposed app code; no new framework or backend. |

Reversibility: forward low — static local app and finite versioned pack; backward low — revert app commits and remove its cache without migrating accounts or remote records.

## Delivery and completion boundary

B1 establishes the private app and verified source pack; B2 implements the six-step accessible guided experience; B3 implements real narration and offline lifecycle; B4 independently exercises the resulting commit and returns the runnable artifact with observed limits. Every dish has its own ordered/claim/fire/check/review/PR/readback gates. Actual attached required checks and Bugbot results must pass; no review claim is inferred from PR creation.

[Capabilities](CAPABILITIES.md) separates planned, working, simulated, unsupported and untested. [Validation](VALIDATION.md) defines the evidence needed to change status. If required narration, source fidelity, guided stops or saved offline resources cannot pass, report partial completion with the exact failed obligation. A fallback is useful but does not erase that debt. Publishing a plan is not delivering the artifact.


## Current implementation binding — delivery projection

The accepted bounded implementation now exists in its private app home. Current user-authorized prepared ElevenLabs recordings supersede the browser-only speech mechanism above; browser voices remain optional fallback. Source/scripture meaning,39discussion stops, hidden examples and the single-passage scope remain unchanged. The complete pinned Glass CSS and actual components are composed with the existing useful navigation. No runtime provider key, live synthesis, new backend or video download is needed.

[Capabilities](CAPABILITIES.md) and [validation](VALIDATION.md) record observed implementation results and limits. The earlier paragraphs are retained as planning history, not current availability claims. Human-heard narration quality remains mandatory and unverified; delivery is partial. Private kitchen receipts govern actual acceptance and gates, while this public text is a sanitized result projection.
