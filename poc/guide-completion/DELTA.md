# Driver-seat delta and challenge inputs

Ran the canon driver's-seat prompt against this plan, existing English/Spanish state, shared guide components, current cookbook finish contract and live Glass FIA proposal before challenge. Canon retrieved through Oddkit (`driver-seat-lens`, content hash adp0vp).

As the facilitator, I can browse six steps in seconds without doing any work. As the implementer, I cannot turn visited or an audio-ended callback into evidence that a group finished a discussion. As the returning user, I need my reading position and my explicit completion marks to survive independently.

Changes made by the lens:
- Replaced initially tempting visit/audio-end checks with explicit section acknowledgement, then derived step completion. This removes false completed discussion claims and includes silent readers.
- Combined marking and continuing into one primary action so every section does not require two extra clicks; kept navigation-only Next for intentional skipping.
- Made completion a separate bounded ledger, preserving existing playback/position rather than mixing new semantics into visited arrays.
- Bound to per-section source digest and canonical aliases instead of whole app revision, so an unrelated media release does not erase valid marks.
- Named Finish-session migration as an explicit semantic change instead of leaving the old visited-based promise contradictory.
- Kept checks in shared dropdown/index surfaces, distinguishing current position from completion.

Rejected: audio end as completion (seek/ended cannot establish discussion); completed-step-only storage (cannot truthfully check sections); auto-mark on Next (navigation is not acknowledgement); new Progress tab now (DS is explicitly proposed and its chapter-grid data is absent); human/assessment score (unsupported); cross-language hash matching (distinct source activity identities).

System: source adapter → explicit mark/undo ledger → one derived completion projection → shared guide/index/step labels and Finish gate. Playback, media quality and offline download status remain separate evidence domains.

Challenge cases to test the revised plan: jumping to step6 after visiting all steps, seeking to audio end, a discussion cue merged into its primary, a translated source revision, quota failure after marking, removing saved audio, and revisiting a completed section. None may fabricate or erase unrelated completion evidence.
