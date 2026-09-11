# Adult and Kid Goat — resource-body findings

The source-reported title is **Adult and Kid Goat**, with exact public key `VideoBibleDictionary/eng/a183` and reported version `1.0.4`. Retrieve the entry through the [Aquifer MCP endpoint](https://aquifer.klappy.dev/mcp) using `get` with resource code `VideoBibleDictionary`, language `eng` and content ID `a183`. The rendered body SHA256 is `57f3bbd25292b1f099fe45b55845d7f54f379d4f713c569f6e3334774857c2a0`; this binds the inspected wrapper, not the film. The source's review field was `None`, which is metadata rather than an evaluator verdict.

This limited pass examines one returned resource body, not the linked film. The body contains a preview image, two links to the same video target and a source-reported duration of 67 seconds. Its header associates several Scripture passages with the entry; the body does not explain those relationships or provide a teaching sequence.

The wrapper provides a way to reach media, but its text does not establish what the video teaches, how it should be used within FIA, or whether playback works. A title or preview cannot substitute for watching and evaluating the film. The separate image and video remain unexamined dependencies.

No transcript, captions, synchronization instructions or rights terms appeared in this returned body. That observation is limited to the body; it does not establish their absence from the media or its authoritative source. The reported duration is not measured runtime, and the wrapper's size is not a media-download measurement.

For the [proposed app framing](../../../../PRODUCT.md), this is a concrete media-access case relevant to FIA-003. Separate media dependencies need assessment before drawing conclusions about offline use or transfer size under FIA-006 and FIA-010. These are analytical implications, not approved requirements or evidence of implemented behavior.

See [use notes](USE-NOTES.md) and [dimension coverage](COVERAGE.tsv). Authorized reviewers can resolve exact identity, body hash and original asset edges in the [private unit record](https://github.com/klappy/kitchen/blob/main/rail/meals/2026-09-11-fia-aquifer-evaluation/evaluation/2026-09-11-fia-aquifer-videobibledictionary-eng-verified-001/UNIT-COVERAGE.tsv). Media meaning, spoken language, instructional suitability, rights and actual device/offline behavior remain unassessed.
