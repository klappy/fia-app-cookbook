# Journey drafts

These are proposed product journeys grounded in [reviewed historical support](../journals/support/SUPPORT-001.md), with **derived ordering and recovery hypotheses**. They are not observed end-to-end user workflows, an authoritative FIA method sequence or implemented behavior. The supporting records distinguish historical needs from inferred design. [Role hypotheses](PERSONAS.md) also remain unvalidated.

Each exercise below requires an actual result before it can establish usability. Acceptance thresholds, owners and current product rulings are not filled. [Sources](../SOURCES.md#supporting-pass-001) provides authorized witness access.

## J-01 — Engage, discuss, resume

Context hypothesis: P-01 guides a shared session or P-04 follows a familiar resource rhythm. Individual use may differ. [R-01](REQUIREMENTS.md#r-01--pause-and-return-to-a-shared-resource) and R-04 develop the behavior. Historical support: [resource flow](../journals/support/SUPPORT-001.md#sup-001-24), [non-answering guidance](../journals/support/SUPPORT-001.md#sup-001-26), [expression](../journals/support/SUPPORT-001.md#sup-001-28), [persona assumption](../journals/support/SUPPORT-001.md#sup-001-31).

| Proposed step | Supported need / rationale | Derived interaction or recovery to test |
|---|---|---|
| Reach the intended resource and guided context | Unlike resource types make navigation central; users should not need to hunt through menus. | Check that selection leads to the intended context; allow deliberate reselection. |
| Listen and encounter a related question or media cue | Historical support describes Bible listening, scripted questions, maps and images across a multi-step experience. | Use a verified resource sample; do not turn that description into an independently verified method sequence. |
| Inspect the referenced resource at the relevant moment | Automatic presentation was desired to avoid extra searching. | Compare cue behavior against verified tags and timing. Show how to recover when a cue is missing; behavior not yet chosen. |
| Pause for discussion or dramatized questions | Make space for communal engagement; guidance should not reveal answers. | Observe group control and pacing. Test whether a return point is understandable across media. |
| Resume and express meaning | Resume relevant content; articulation does not require recording in this app. | Test replay, return and expression outside a recording workflow. Watch whether the group loses context. |

Alternative: a person may navigate deliberately rather than follow automatic guidance. Shared audible use was historically considered sufficient without synchronized user state. Conversational control remains a separate possibility; the AI priority disagreement is still open. Actual exercise results: **Not filled**.

## J-02 — Prepare content for offline use

Context hypothesis: P-03 anticipates using selected resources without connectivity. [R-02](REQUIREMENTS.md#r-02--prepare-and-manage-offline-resources) and R-07 develop the behavior. Historical support: [deliberate storage](../journals/support/SUPPORT-001.md#sup-001-62), [content packs](../journals/support/SUPPORT-001.md#sup-001-63), [platform exercises](../journals/support/SUPPORT-001.md#sup-001-58), [fidelity dependency](../journals/support/SUPPORT-001.md#sup-001-60).

| Proposed step | Supported need / rationale | Derived interaction or recovery to test |
|---|---|---|
| Choose useful language/resource content while connected | A useful app should not require the full audio collection; application and content size differ. | Evaluate actual resource boundaries before defining a pack. No language list is approved. |
| Obtain the selected content | Downloads, side-loading and optional audio packs were alternatives. | Observe transfer behavior; test interruption and an incomplete state rather than claiming a chosen mechanism. |
| Check that the resource is usable | Tags, timing and linked media matter to the experience. | Reconcile a verified resource manifest with what arrived; an availability indicator is a hypothesis. |
| Use the resource disconnected | Offline-first and audio-visual-first were desired together. | Exercise intended devices and platforms, including a missing remote dependency. Record actual limits. |
| Remove content no longer needed | Device storage cannot hold everything. | Investigate accidental removal, re-download and the meaning of removing a pack. No confirmation design is selected. |

Alternatives include text-to-speech while no human recording is installed and different pack arrangements. Actual Aquifer use, media optimization and permissions remain unassessed dependencies. Actual exercise results: **Not filled**.

## J-03 — Configure the app by speaking

Context hypothesis: P-04 wants to choose the resource experience through speech. R-05 develops the behavior. Historical support: [two distinct interaction aims](../journals/support/SUPPORT-001.md#sup-001-23), [voice over a defined flow](../journals/support/SUPPORT-001.md#sup-001-34), [app-driving configuration](../journals/support/SUPPORT-001.md#sup-001-35).

| Proposed step | Supported need / rationale | Derived interaction or recovery to test |
|---|---|---|
| Express the section to study | Spoken input was desired to change what the app does. | Check the interpreted section and provide a way to correct it; correction behavior is a hypothesis. |
| Choose the intended pericope | The historical example narrowed a section into the desired study unit. | Present available choices without claiming the catalog or language behavior is verified. |
| Choose suitable available Scripture resources | The example connected spoken language and Bible choices. | Test ambiguous language or unavailable resources; no localization rule is selected. |
| Enter the guided experience | The goal was navigation/configuration rather than only an answer. | Verify the resulting app state and allow return to deliberate selection. |

Alternative: a question-answer route through an external assistant was proposed. It does not replace the app-driving goal. A scripted resource cue is another interaction, not evidence that conversational control already works. No original-demo or first-pitch claim is made. Actual exercise results: **Not filled**.

## J-04 — Prepare individually and express meaning

Context hypothesis: P-02 wants to understand Scripture independently, potentially before communal use or another translation workflow. R-03, R-06 and R-08 develop the behavior. Historical support: [independent access](../journals/support/SUPPORT-001.md#sup-001-14), [internalization boundary](../journals/support/SUPPORT-001.md#sup-001-11), [audio choice](../journals/support/SUPPORT-001.md#sup-001-36), [community extension disagreement](../journals/support/SUPPORT-001.md#sup-001-15).

| Proposed step | Supported need / rationale | Derived interaction or recovery to test |
|---|---|---|
| Reach resources without the team’s translation-tool device | Other participants may need to view, listen or prepare independently. | Investigate actual access conditions without inventing an authentication model. |
| Engage orally, with optional text | Oral-first does not mean oral-only. | Ask whether available modes support the intended task; do not infer reading ability. |
| If recording is absent, consider a disclosed generated voice | Generated speech was proposed as a choice where written content exists. | Test comprehension of its origin and alternatives; no language quality is assumed. |
| Express understanding individually or with others | Expression is supported while recording/checking remains outside proposed initial scope. | Observe how the task finishes without making a production or publication workflow part of the app. |

Using progressively published Scripture was an extension proposed and challenged. This journey does not resolve that audience boundary or make formal community testing an initial feature. Self-recording and submission belong to a separate scope question. Actual exercise results: **Not filled**.

## J-05 — Turn feedback into another product iteration

Context hypothesis: P-05 helps a product team learn from use; this is a development journey, not an in-app feature or second work queue. R-09 and R-10 develop the behavior. Historical support: [focused feedback](../journals/support/SUPPORT-001.md#sup-001-48), [same-participant retest](../journals/support/SUPPORT-001.md#sup-001-49), [end-to-end submission](../journals/support/SUPPORT-001.md#sup-001-50), [product versus project work](../journals/support/SUPPORT-001.md#sup-001-64).

| Proposed step | Supported need / rationale | Derived procedure or recovery to test |
|---|---|---|
| Define the learning question and reachable participants | Feedback needs and collection time can determine the pace of iteration. | Establish actual responsibility and authorization through the [existing rail](../management/DELIVERY-PLAN.md); no owner is assigned here. |
| Exercise focused tasks and capture outcomes | Questions, forms and optional observation were proposed; a small sample can expose repeating issues. | Use an authorized, appropriate collection method. Sample size is not validated by the historical suggestion. |
| Verify that the response arrived | A rendered form alone did not establish working feedback in an adjacent lesson. | Check one real submission end to end and handle failure explicitly. |
| Synthesize needs, alternatives and contrary findings | Product work should turn observations into actionable requirements rather than forward every opinion. | Link a proposed change to evidence and the actual decision path; project tracking records its delivery separately. |
| Revise and retest the original problem | Retesting the same participants helps distinguish improvement from changed samples. | Preserve useful behavior, check regressions and still examine diverse environments. Actual improvement must be observed. |
| Widen use when justified | Broader sharing should follow growing confidence; provisional status should remain visible. | Record the basis for expanding review instead of treating technical completion as usability proof. |

A bounded development effort and continuing maintenance are distinct. There is no committed iteration count, release date, tested automated pipeline or current role appointment. Actual exercise results: **Not filled**.

## Add a journey


| Field | Entry |
|---|---|
| ID / status / role hypothesis | Not filled |
| Trigger / context / intended outcome | Not filled |
| Evidence revision and claim IDs | Not filled |
| Steps, with observed versus inferred ordering | Not filled |
| Pain points and evidence | Not filled |
| Recovery paths / alternatives | Not filled |
| Related requirements and dependencies | Not filled |
| Validation exercise / actual result / open questions | Not filled |

Record supporting evidence and unresolved threads in [Support](../journals/SUPPORT.md); use the [delivery plan](../management/DELIVERY-PLAN.md) for links to authorized work.

## Bounded PoC scenario

[PLAN](../poc/PLAN.md) defines a source-bound six-step, single-passage scenario with [observable validation](../poc/VALIDATION.md). Existing journey ordering remains hypothetical. [FIA website terminology and resource paths](../references/FIA-WEBSITE.md) inform navigation, while [source-pack evidence](../poc/SOURCE-PACK.md) determines actual included assets. Spoken app-driving remains distinct from synthetic narration and accessible controls.
