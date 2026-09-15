# Observed source evidence

- App8ef31b2 `src/lib/flow.js`: initial visited first step; selectStep appends visited; moveUnit and afterNarration navigate; canFinish checks visited count/current step only. `validateSession` retains finished based on visited count.
- `src/lib/session.js` and `src/lib/workspace.js`: persist position/visited and exact audio checkpoint; no completed-section ledger.
- `src/lib/guide-presentation.js`: Spanish finish derives from six visitedSections; canonical heading merges/aliases define ordinary presentation.
- `src/components/SpanishSession.jsx`: moveGuide appends visitedSections; shared GuideScreen receives visited-derived completion; index rows currently separate language mapping.
- `src/components/GuideScreen.jsx`, `GuideIndex.jsx`: existing step dropdown/section index and explicit Finish; no inline completed state.
- `src/vendor/glass/components/forms/GlassSelect.jsx`: native select/options, textual labels supported; rich option markup not supported.
- Cookbook5ff8b9a `poc/PLAN.md` line35: explicit Finish after six steps visited; only local visited/position state. New plan proposes a governed supersession, not reinterpretation of historical records.
- Live Glass8d6b48d `ui_kits/fia/README.md`: Progress proposal, structure explicitly provisional until cookbook; `ui_kits/fia/app.jsx`: ProgressGrid sample and check tab icon; `components/progress/ProgressGrid.prompt.md`: books/chapter status cells. Neither source supplies actual app completion semantics.

Repository heads refreshed through Git reads. Canon driver's-seat lens retrieved through callable Oddkit get. No app code changed during planning. Independent root review is pending.
