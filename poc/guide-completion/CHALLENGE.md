# Revised candidate challenge disposition

The original tool challenge in CHALLENGE.json applies to the earlier, broader candidate and is retained as historical evidence. It does not approve this narrowed revision. Independent exact-candidate review is pending before any further public write or implementation.

Revised driver challenge: can this helper accidentally require marks, navigate, stop playback or change Finish? The plan now explicitly forbids each and tests empty/partial/full marks against unchanged Finish eligibility. Can visiting all steps imply checks? No; historical state is preserved but never backfilled. Can a missed mark prevent finishing? No. Can undo lose the current audio offset? No; the ledger is independent of the checkpoint.

Confidence and costs: source observations are verified at the listed revisions. Explicit acknowledgement is a proposed optional interaction, not field-validated usability. Marking can be forgotten; omission has no workflow penalty. Source changes may invalidate a mark. Reconsider the helper if native review shows controls obscure the reading surface or imply a requirement.

Scope is one passage and both existing language adapters. No assessment claim, new navigation, mandatory completion flow or source-content rewrite. Root must review the exact amended text before publication; implementation additionally needs its own landed ticket/fire.
