# Selected source pack

Status: planning probes completed 2026-09-11; selected text bodies and metadata returned, media URLs answered HEAD. No media has yet been rendered, played or verified as saved offline. Source content quality is not independently theologically certified.

The finite scenario is Mark 1:1–13 in English. Aquifer's `get` tool returned FIATranslationGuide/eng/eng-mrk-p1-v2.1, article version 1.0.4, review level None, with all six steps. Preserve its labels, content and current review status. The current [FIA website](../references/FIA-WEBSITE.md) supplies useful parallel resource navigation; website metadata does not prove content equivalence or supersede these source bodies.

| Aquifer source repository under BibleAquifer | Inspected commit | Selected content / rights metadata |
|---|---|---|
| FIATranslationGuide | 5d6d59a22caa8f8539c5ff6a3e1ec74c4cfa5c6d | eng-mrk-p1-v2.1; WordCollective, CC BY-SA 4.0 |
| FIAMaps | 7e56e7bc68d354a72b7a3e882beb78d5f084d7f5 | c201/c202/c197/c168; license_info names Biblica, adaptation_notice names WordCollective; CC BY-SA 4.0 |
| FIAImages | 8fbb154360574ba2981fbaa4064a1e8979de7e82 | a112/a111/a203/a204; WordCollective, CC BY-SA 4.0 |
| FIAKeyTerms | 5ce5c6bd152236e16cf23290a40ab625175df8e3 | 21 associated English articles listed below; WordCollective, CC BY-SA 4.0 |
| VideoBibleDictionary | 85b4bec7634f3f5989d0767b372084eb19098227 | a13/a10/a184 descriptions and external links only; WordCollective, CC BY-SA 4.0 |
| BereanStandardBible | c7fbd7e8301d6b5aa03870780c04a7464b4dbb27 | Mark 1:1–13, all 13 verses; CC0/public domain metadata |
| unfoldingWordLiteral | 9c6a5e75d0849198240e38d22157b497bc84dc9f | Mark 1:1–13, all 13 verses; unfoldingWord, CC BY-SA 4.0 |
| unfoldingWordSimplified | 90d02427ebc22dc9e4e961c38221f1711426f5db | Mark 1:1–13, all 13 verses; unfoldingWord, CC BY-SA 4.0 |

The 21 exact FIAKeyTerms IDs are eng-t4-v1, eng-t5-v1, eng-t9-v1, eng-t23-v1, eng-t38-v1, eng-t53-v1, eng-t60-v1, eng-t63-v1, eng-t68-v1, eng-t76-v1, eng-t87-v1, eng-t88-v1, eng-t92-v1, eng-t103-v1, eng-t104-v1, eng-t109-v1, eng-t118-v1, eng-t125-v1, eng-t129-v1, eng-t145-v1, eng-t226-v2. Thus the guide's one-hop association set is 32 items: 21 terms, four maps, four images and three videos. Do not recursively import related-resource links. Preserve Desert's redirect meaning and the two Lord senses; do not collapse them into an invented definition.

## Source alias evidence

The guide's map IDs `eng-c201-v1`, `eng-c202-v1`, `eng-c197-v1`, `eng-c168-v1` returned missing when directly requested. Two bounded catalog pages exposed c201/c202/c197/c168, with matching titles and Mark 1:1–13 associations; explicit get calls returned those bodies. The website's matching four map filenames independently support identity, not byte equivalence. Bind these four aliases explicitly with source/target IDs and observed version; no generic stripping heuristic or silent fallback. A different or missing source revision fails the manifest check.

## Media boundary

Image source URLs returned by the articles:

- Photos: `https://s3.amazonaws.com/cbbt-er.public/media/photos/{a112|a111|a203|a204}/1000.jpg`.
- Maps: `https://s3.amazonaws.com/cbbt-er.public/media/maps/eng/{c201|c202|c197|c168}/v1/original.png`.
- Video links: `https://s3.amazonaws.com/cbbt-er.public/media/videos/{a13|a10|a184}/720p.mp4`.

All eight image HEAD requests returned 200 with image MIME types and nonzero lengths; together roughly 23 MB. Video HEADs also returned 200. These are accessibility leads only. B1 must fetch each required image, compute SHA-256, verify its actual type/dimensions and inspect all eight images; B4 must display each in the browser and recheck offline. Do not download videos; expose labeled external links with online-only state and no playback-success claim. No known audio timecodes or original spoken guide files are imported.

FIAMaps metadata names Biblica in license_info and WordCollective in adaptation_notice. Preserve both supplied notices verbatim in app attribution and NOTICE.md; the holder discrepancy remains unresolved. The shared CC BY-SA 4.0 string is not a full legal-clearance claim. This discrepancy alone supplies no demonstrated conflicting permission for the bounded private PoC, but B1 must inspect each actual asset for additional or conflicting notices before redistribution; a material conflict holds the affected asset.

For every included article/media item, persist original source URL, repository/commit/path where available, content ID, language, article version, review level, retrieved timestamp, raw-source digest, delivered digest, MIME/bytes and selected metadata license/holder. Preserve attributions in the app and NOTICE.md; format/segmentation changes are adaptations and retain applicable share-alike terms. Code licensing is a separate decision; source content is never relicensed by a blanket app license. B1 verifies metadata at its pinned revision; unavailable or conflicting rights hold that asset rather than fabricate clearance.

## Unit and cue manifest

Generate a deterministic manifest from the exact pinned guide body. Each h2 begins S01–S06; paragraph and list-item leaves produce U001 onward without duplicating nested text. Preserve complete source order, inline emphasis and links. Store SHA-256 of each normalized text unit and complete original article; the checked-in cue manifest references both ID and hash. This makes a source change visibly invalidate a cue instead of pointing to a different question.

The [cue manifest](CUE-MANIFEST.json) binds all 130 unit hashes, 39 pause coordinates and the hidden example boundary after a complete guide-unit read. They are source-read planning coordinates, not implemented timing. B1 must read back generated coordinates against the full guide, bind hashes and have its independent reviewer confirm every question/activity boundary. If coordinates differ under the specified parser, correct the coordinates and re-review without changing content or hiding the mismatch.

| Step | Required cue/action checks |
|---|---|
| S01 Hear and Heart | Scripture choice/listening prompt U002; discussion questions U003–U008 each stop separately. Offer three actual English versions without forcing three playback completions or claiming listening occurred. |
| S02 Setting the Stage | U005 Jordan image a112/map c197; U008 sandals a203/a204; U011 discussion and U012 pause. Verify map visibly contains the intended geography before associating it. |
| S03 Defining the Scenes | U007 regional map c168; U019 Jordan/wilderness images a112/a111; U021 Judea/Jerusalem maps c201/c202. U025 storyboard activity also stops. |
| S04 Embodying the Text | U014/U016 activity pauses. Hide source example region U017 through section end behind explicit reveal; do not auto-narrate sample responses. Preserve full source view. |
| S05 Filling the Gaps | U004 gospel t60; U006 Messiah t92/Christ t23; U008 Son of God t129; U013 prophet t104; U015 desert image a111/terms t38,t145; U017 Lord t87,t88; U019 baptism t9/repentance t109; U031 sin t125; U035 Holy Spirit t68; U038 heaven t63; U041 Satan t118; U043 angels t4. U029 embodied forgiveness activity also stops. Each discussion question stops. All 21 associated terms remain independently browsable. |
| S06 Speaking the Word | Turn-taking instruction U004 is followed by pause U005; further discussion/activity pauses are U007/U009 (do not add a duplicate U004 pause); U010 final practice also stops; finishing requires explicit user choice. No recording or assessed answer. |

The complete source, source manifest and cue audit are B1 outputs. These candidates do not exempt the remaining source units from review. No generated narration may supply new teaching or answers.

Related assessments: [guide use notes](../evaluation/aquifer/batches/2026-09-11-fia-aquifer-fiatranslationguide-eng-verified-001/USE-NOTES.md), [video body notes](../evaluation/aquifer/batches/2026-09-11-fia-aquifer-videobibledictionary-eng-verified-001/USE-NOTES.md), [website reference](../references/FIA-WEBSITE.md), [capabilities](CAPABILITIES.md).

## Canonical path readback

[RESOURCE-PATHS.json](RESOURCE-PATHS.json) records all 32 actual canonical paths, repository commits, file/content hashes and captured API-wrapper hashes. All 29 non-video content bodies occur exactly in their API wrapper. The three video bodies match after the documented relative-thumbnail URL expansion; the app does not import those thumbnails. This comparison binds meaningful body identity while preserving format differences, rather than claiming API-wrapper bytes equal source JSON. Scripture and guide source/body readbacks remain separately required in B1.
