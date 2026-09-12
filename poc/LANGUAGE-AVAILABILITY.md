# Second-language availability: Spanish is a planning candidate

Read-only triage under language-availability fire d0591d32. Retrieval: 2026-09-12 UTC (local evening 2026-09-11); exact observation timestamps and response hashes accompany this note. No app changes, translation or synthesis. English remains the only runnable verified app pack.

Spanish has a real six-step Mark1:1–13 guide and two returned Scripture texts. It is the strongest candidate from this bounded inspection, not a proven globally best language or ready-to-enable complete pack. A language switcher requires a separate cooked plan because source associations and versions differ materially from English.

| Capability | Actual evidence | Limit |
|---|---|---|
| Guide | FIATranslationGuide/spa/spa-mrk-p1-v2.1, version1.0.4, passage41001001–41001013; full29,556-character HTML body retrieved. Six section headings. Repository5d6d59a22caa8f8539c5ff6a3e1ec74c4cfa5c6d, spa/json/41.content.json; bodySHAf5a129481d155d7fcb4011d459e154f6c09a1d0bb5f4d4383126bd602a402cee. MCP exact-ID read succeeded. | No independent Spanish semantic/cue review yet; English111activities/39stops must not be transplanted. |
| Scripture | Actual scripture(Mark1:1–13,spa) returns ReinaValera1909 and AquiferSpanishBibleReferenceText, each numbered1–13. | Two versions, not three; per-edition license/body pins still required. No Spanish recordings proved. |
| Terms | Spanish guide has15explicit term associations. All15 matching bodies found in pinned FIAKeyTerms5ce5c6bd152236e16cf23290a40ab625175df8e3/spa/json. Exact IDs and body hashes in term-coverage.json. MCP spa-t4-v1 returns Spanish body, with title still “angel”. | English pack has21terms; these sets differ. This is body availability, not semantic validation or complete localized labels. |
| Images | FIAImages/spa/a112 returns Spanish title Río Jordán and actual image URL, version1.0.4, MRK1:1–13 association. | Same shared image URL as English; only this sample probed. No claim all4localized metadata/assets are validated. |
| Maps | Catalog reports FIAMaps no localizations; browse(FIAMaps,spa) returns no articles. | Spanish maps unverified/unavailable through this probe. English-labeled fallback requires explicit policy; cannot present as localized. |
| Video | VideoBibleDictionary/spa/a13 returns Río Jordán metadata and79-second MP4 URL. | Same shared MP4 URL; not downloaded/played, language of spoken track unproved. |
| Narration | No Spanish audio bytes were requested or played. | Catalog “-audio” entries and text-language metadata are not audio existence/quality proof; app172clips remain current English narration. |

Important discovery: browse(FIATranslationGuide,spa) and browse(FIAKeyTerms,spa) display English article IDs/titles in their catalog pages. get(spa,eng-mrk-p1-v2.1) and get(spa,eng-t4-v1) fail. Actual localized IDs are spa-mrk-p1-v2.1 and spa-t4-v1, discovered from canonical repository bodies. Treat browse counts1465/512 as catalog metadata, not verified Spanish coverage. French same English-ID lookup failed; no conclusion that French guide is absent.

Spanish guide metadata1.1.2 declares CC BY-SA4.0, Word Collective2025 and non-English adaptation notice naming Mission Mutual. Preserve supplied notices; other selected editions/media still need asset-specific review. Guide associations contain15terms and no map/image/video resource links, so English resource links cannot be silently imported as Spanish source associations.

The actual shared LanguagePicker distinguishes Resources in / Project language / Translate into / App language and supports language capability indicators. Reuse its real component after defining which dimension changes. Spanish is LTR and can use existing Latin font fallback; actual accented text/wrapping/offline fallback still need tests. RTL is not established by this Spanish slice; other-language Arabic/Hindi typography and direction are separate validation, not automatic support.

Recommendation: cook a bounded Spanish source/UX plan before implementation. Keep unsupported media and untested audio explicit; avoid an empty switcher or mixed-language content presented as Spanish-complete.

## Source and review pointers

- [Pinned Spanish guide body](https://github.com/BibleAquifer/FIATranslationGuide/blob/5d6d59a22caa8f8539c5ff6a3e1ec74c4cfa5c6d/spa/json/41.content.json).
- [Pinned Spanish term bodies](https://github.com/BibleAquifer/FIAKeyTerms/tree/5ce5c6bd152236e16cf23290a40ab625175df8e3/spa/json); [15 associated IDs and body hashes](LANGUAGE-TERM-COVERAGE.json).
- [Existing selected English pack](SOURCE-PACK.md), [FIA website coverage](../references/FIA-WEBSITE.md), and [source register](../SOURCES.md).

Independent review checked the complete findings and retrieval/body-availability evidence. It passed the limited availability and privacy claims; it did not validate Spanish meaning, cue interpretation, asset licensing or spoken audio. English remains the only implemented pack. The proposed Spanish planning dish is ordered separately; no Spanish app build or generation is authorized by this availability note.
