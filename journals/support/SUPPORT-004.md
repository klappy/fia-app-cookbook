# Supporting pass 004 — media access, storage and bounded development

Status: sanitized historical proposals, rationales and unresolved questions from one reviewed source. These records do not establish current requirements, owners, commitments or shipped behavior.

Authorized reviewers can resolve each public record through the private projection and witness ledger under the [source-access rules](../../SOURCES.md). Private identifying context and quotations are excluded. The [claim register](../../claims/CLAIMS.tsv) remains proposed; [current PoC status](../../poc/NARRATION-MEDIA-STATUS.md) describes actual implementation, and [oral-audience research](../../research/ORAL-AUDIENCE.md) retains its separate evidence and limits.

Adjacent coaching and map-tool possibilities below are historical context, not assignments or authorization to add those products to the app.

## SUP-004-01
Status: historical support / proposal or open question. Attachment: FIA-010.

Image and audio size were identified as access constraints. A proxy was described as compressing images before device delivery, with device-size optimization and minimal artifacts claimed. Pixelation was explicitly questioned; these are historical demonstration reports, not present benchmark validation.

## SUP-004-02
Status: historical support / proposal or open question. Attachment: FIA-010.

Transfer comparisons distinguished original, first transformed request and cached reuse. Compression adds processing overhead and may not beat the original on a very fast connection. Simulated network averages were used, not direct measurements of every field setting; the rationale was faster access and lower storage use on constrained devices.

## SUP-004-03
Status: historical support / proposal or open question. Attachment: FIA-010.

A comparison mode and quality/resolution choices were described for inspecting tradeoffs. Very low quality may suffice for thumbnails but visibly loses detail; text within images is a difficult case. A question about automatic device selection was raised, not resolved as a verified app behavior.

## SUP-004-04
Status: historical support / proposal or open question. Attachment: FIA-010.

Medium quality was described as the proxy default, with reduced zoom detail judged against what a phone task needs. Existing low-resolution source images constrain the result. Reported visual similarity must not imply new detail can be recovered or that all images pass usability review.

## SUP-004-05
Status: historical support / proposal or open question. Attachment: FIA-006.

Caching avoids repeated downloads but consumes device space; compression reduces rather than removes that tradeoff. Maps were singled out because high-quality originals can be large. Transfer improvement does not solve the overall storage strategy.

## SUP-004-06
Status: historical support / proposal or open question. Attachment: FIA-009.

Broken source links were reported separately from slow loading. Map label readability and zoom were demonstrated as usability concerns. The report does not prove current links are broken or every compressed map is legible.

## SUP-004-07
Status: historical support / proposal or open question. Attachment: FIA-006.

Storage needs a logical content boundary: choosing a passage and optionally selecting images/audio with a package-size indication was discussed as an existing adjacent workflow. It is an example to evaluate, not a requirement to copy every detail.

## SUP-004-08
Status: historical support / proposal or open question. Attachment: FIA-006.

A competing preference was to spare users detailed download decisions: identify what the selected task needs, then ask whether to retain it or access it temporarily. Explain the benefit of keeping content rather than technical storage terminology.

## SUP-004-09
Status: historical support / proposal or open question. Attachment: FIA-006.

Warn when space fills and ask whether older material is still needed. First-in/first-out and use-based removal were alternatives; recency and frequency terminology was mixed. The policy was considered changeable, not a settled automatic-deletion rule.

## SUP-004-10
Status: historical support / proposal or open question. Attachment: FIA-006.

Already-full phones motivated alternatives such as removable media, import/export packs and local shared storage. Importing a zip pack was described but challenged as too complicated; device compatibility was partly uncertain. The anecdote is not a demographic claim about all users.

## SUP-004-11
Status: historical support / proposal or open question. Attachment: FIA-006.

Waiting for connectivity to download selected content was favored as a straightforward initial workflow. A local Wi-Fi storage server could support content too large for phones, but entails a separate application/product and real physical-device testing. Its possibility does not authorize that product or a current phase deadline.

## SUP-004-12
Status: historical support / proposal or open question. Attachment: FIA-010.

An audio comparison used a short Scripture chapter, and playback through a connected display failed for a format. Output-path compatibility therefore needs testing; small file size alone does not establish usable playback. Quoted Scripture/demo audio is not reproduced.

## SUP-004-13
Status: historical support / proposal or open question. Attachment: FIA-010.

The demonstration compared quality levels: medium differences were harder to hear without better listening equipment, while the lowest setting sounded noticeably degraded. Originals and archival formats were distinguished from delivery copies. These subjective historical comparisons do not certify current audio quality or all playback devices.

## SUP-004-14
Status: historical support / proposal or open question. Attachment: FIA-009.

Keeping originals authoritative and deriving smaller versions dynamically was proposed to avoid manually updating many copies when a source changes. Redistribution copies remain possible, and video may justify managing derivatives differently. The convenience claim is not proof of a correct current invalidation system.

## SUP-004-15
Status: historical support / proposal or open question. Attachment: FIA-010.

A proxy interface using an original URL and a few presets was described as hiding many compression choices. Voice/quality/format and image quality/resolution simplify integration; end users need not understand codec parameters. This is historical architecture, not a mandate for a particular current codec or host.

## SUP-004-16
Status: historical support / proposal or open question. Attachment: FIA-006.

Users want resources they can see and hear promptly more than abstract byte counts. Preparation was reported as slow with no visible indication of progress, suggesting a need to make completion understandable. No particular progress UI is validated here.

## SUP-004-17
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

A kitchen/order metaphor was proposed to make AI development approachable despite jargon. A repeatable recipe or explicit inputs, goal and checklist should be prepared before work starts, including a definition of done, rather than discovering missing questions during execution.

## SUP-004-18
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

The metaphor separates ordering, work in progress and a review stage before serving. Hiding execution complexity should not hide the need for final review. Reported personal effectiveness is not a measured project outcome or governing authority for this cookbook.

## SUP-004-19
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

The repair-versus-rebuild analogy distinguishes recoverable defects from a result so wrong that compensating edits make it worse. Sometimes restarting is preferable; this is a contextual judgment, not blanket permission to discard work.

## SUP-004-20
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Participants questioned how much detail is enough. Features may be grouped into a larger outcome, while the metaphor can stay internal if it does not help collaborators. Its usefulness should be tested with people rather than imposed universally.

## SUP-004-21
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Partial familiarity with FIA leaves unknowns. Iterative conversations and checking interpretations with domain knowledge were proposed to establish what is actually needed, rather than assume fluent terminology proves understanding.

## SUP-004-22
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

An adjacent coaching/training effort illustrated a handoff gap: technical possibility, domain understanding, partner expectations and concrete test tasks were not aligned. Clarify the requested work and subject-matter support before expecting useful testing. Private personnel assessments are withheld; no new adjacent-project assignment is made.

## SUP-004-23
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Limited available assistance prompted the question of whether bounded testing would be useful and what gaps it should target. Clarifying the boundary between this app and an adjacent service was proposed. Personal details and capacity commitments are withheld.

## SUP-004-24
Status: historical support / proposal or open question. Attachment: FIA-008.

Question-answering over a defined information collection was distinguished from process coaching, which might guide action, connect people and offer examples. Whether people would use AI for process guidance remained a research question; enthusiasm for a messaging channel is not proof of suitability.

## SUP-004-25
Status: historical support / proposal or open question. Attachment: FIA-008.

A training network may need to locate people who hold knowledge, not only documents. AI-assisted matching or a contact system was suggested, with gated rather than automatically public access. This is an adjacent future possibility, not an app contact feature authorization.

## SUP-004-26
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Sharing an expert contact raises consent concerns. A mediated introduction could ask both sides before exposing contact information and allow refusal. Illustrative names and sensitive scenario detail are withheld; no contact or introduction is performed.

## SUP-004-27
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Success configuring one domain does not establish understanding of another. Explicit partner ownership of intended workflow, roles and expected outcomes was proposed as a way to locate the remaining gap. Individual evaluations and organizational details remain withheld.

## SUP-004-28
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

Changing availability and work arrangements were part of the context, but no commitments are retained. A concrete app implementation was proposed as a reference that might inform another channel’s process guidance; it is not automatically authoritative or transferable unchanged.

## SUP-004-29
Status: historical support / proposal or open question. Attachment: FIA-003.

An oral, scripted overview using the interface and sample data was proposed for someone opening the app without context. It would walk through the process while explicitly not replacing official training; UX exploration should test that distinction.

## SUP-004-30
Status: historical support / proposal or open question. Attachment: FIA-003.

A welcome explanation and narrated demonstration were offered as precedents for helping users understand an app. A character/persona and conversational examples were mentioned, with discomfort about an overly personal presentation. These examples do not establish a need to add an avatar, chat mode or a new audience-specific component.

## SUP-004-31
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

A separate customizable-map ambition was contrasted with receiving individual static PDFs. The desired reusable tool was not the same product as commissioning maps. Feasibility was speculative and private parties/financial context are withheld; no map implementation is ordered here.

## SUP-004-32
Status: historical support / proposal or open question. Attachment: FIA-009.

The map proposal would choose known geographic features, place labels and translate them using an existing researched dataset, rather than generate an unconstrained picture. Data availability and ease of development were reported assumptions requiring verification.

## SUP-004-33
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

An AI-callable map-building tool was imagined as a reusable foundation: conversational selection, accuracy checks and human review before release, with broader dynamic use only after trust develops. Animation was speculative. This remains separate future scope.

## SUP-004-34
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

A presentation use case imagined showing a geographic journey with contextual visuals, while also wanting a narrowly scoped tool resistant to feature expansion. Monetization detail is withheld; this is not evidence of demand, a current roadmap or permission to build it.

## SUP-004-35
Status: historical support / proposal or open question. Attachment: supporting development question; no new requirement ratified.

The source questions whether licensing/tool access or a mismatch between software development and one-off artifact production caused the map-tool gap. Those causes were unresolved. Human adjustment of selected known content was desired, not assumed accomplished.

## SUP-004-36
Status: historical support / proposal or open question. Attachment: FIA-009.

Content-template building blocks and complicating cases need analysis so the design language covers the resource experience. A prototype from available content may miss attribution or other data gaps; list and address all such gaps rather than rely on a single recurring example.
