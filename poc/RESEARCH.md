# Focused research and reuse

Status: bounded planning assessment, 2026-09-11. These references inform implementation and hypotheses; they do not supersede the [selected scope](PLAN.md). No persona, outcome percentage, field result or end-user acceptance is validated here.

## Audience and domain

The [FIA website assessment](../references/FIA-WEBSITE.md) distinguishes three overarching concepts from the six-step passage process and records language/resource/rights limits. It supports narrative, experience and community as design considerations.

[oral-theology-kb](https://github.com/klappy/oral-theology-kb/tree/2743dd9ffd58c965efa50a6467a7db03876b7949), particularly `sources/stringer-widening-the-table.full.md`, provides interpretive material about oral learning, narrative, embodiment and communal understanding. Its manual extraction and `human_review:false` status remain visible. A focused reading including its FIA discussion informed group pause/activity affordances and the decision not to treat audio delivery alone as oral usability. Its historical process description is not the current passage guide's six-step authority. No broad demographic generalization or validated persona follows from this source. [Role hypotheses](../product/PERSONAS.md) still need actual research.

## Inspected implementation references

| Reference and revision | Actual paths inspected | Reuse decision |
|---|---|---|
| [Generative Glass](https://github.com/klappy/bt-design-system-generative-glass/tree/8d6b48dd93b6efa43305724a0cf320a85feabe5b) | SKILL.md, README.md, ui_kits/fia/{README.md,app.jsx,index.html}, tokens/fonts.css, components/navigation/GlassSheet.jsx, ui_kits/aquifer-window/{README.md,app.jsx} | Borrow shared primitives and truthful resource-detail/license structure. FIA prompts, sync toggles and Record are illustrative. Aquifer Window kit metadata/specimens are not production behavior. App repository for the production Window was not resolved; no production-code claim. |
| [conversational-bible-translation-poc](https://github.com/klappy/conversational-bible-translation-poc/tree/adefef4b58ea934ca4c6c333c824fb539e8f5d64) | README.md, mobile swipe/canvas components and canvas-state/conversation functions | Context continuity informs layout. Reject translation-production/chat/backend topology for this slice; planned/mock audio or FIA resources do not prove functionality. |
| [unfoldingtheword](https://github.com/klappy/unfoldingtheword/tree/cb6370c8a20124bdc730321638a60c39217a9485) | README.md, package.json, voice conversation/replay hooks | Supabase/AI service dependencies are unnecessary for deterministic source guidance. No import. |
| [offline_bible_app](https://github.com/klappy/offline_bible_app) | README.md and package setup | Setup documentation and legacy dependencies are not offline validation. No package installation or implementation reuse. |
| [Aquifer MCP](https://aquifer.klappy.dev/mcp) | Tool docs, source metadata, selected guide/Scripture/resource bodies and bounded catalog pages | Use real source retrieval and provenance. [SOURCE-PACK](SOURCE-PACK.md) binds selected revisions; broad metadata counts do not prove body/media coverage. |

Repository discovery searched the owner's available repositories and an additional Aquifer Window name search. No existing FIA app home was found that matched this bounded build. That is an authenticated-access finding, not proof that no other private repository exists. The proposed private app home requires creation/readback under its own gate.

## Methods and technical references

Cartographer successfully resolved the cookbook repository at its inspected revision and searched pause/resume/offline references; transport success and source revision were observed. Oddkit supplied the driver-seat lens and six-B criteria; the actual design delta and challenge receipts live with the planning dish. Reading a method alone is not its gate.

Targeted supplemental Bee queries addressed offline preparation, voice/navigation ambiguity and group pause. Two bounded pages per query were inspected. Search results remained leads; no snippet was promoted into a scope change. Complete-history search is not claimed. Exact queries/cursors and source coverage are in the authorized private ledger.

The browser platform references are [SpeechSynthesis](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis), [localService](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesisVoice/localService) and [CacheStorage](https://developer.mozilla.org/en-US/docs/Web/API/CacheStorage), retrieved 2026-09-11. These describe device voices, speech control and secure-context cache APIs; they do not prove this host's audible output or offline cache behavior. The build must supply that evidence.

See [requirements](../product/REQUIREMENTS.md), [journeys](../product/JOURNEYS.md), [source register](../SOURCES.md), [capabilities](CAPABILITIES.md) and [validation](VALIDATION.md).
