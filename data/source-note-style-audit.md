# FRUS Source Note Style Audit

Generated: 2026-06-30T13:52:14.843Z

Scope: document-level `Source:` notes harvested from published Carter, Reagan, and George H.W. Bush FRUS document pages on `history.state.gov` and published at `FRUS-Sources`.

## Result

PASS: all document-level Source notes in the copy-paste exports meet the FRUS source-note style and extraction-safety gates.

## Counts

- Document rows in full export: 13042
- Document-level Source notes checked: 12298
- Unique Source-note texts: 12073
- Copy-paste Source-note rows exported: 12298
- Failing audit gates: 0

## Copy-Paste Gate

- Every exported compiler row begins with exactly one leading `Source:` label.
- The copy-paste exports exclude editorial-note, empty-stub, and pending-placeholder rows.
- No copy-paste Source note contains HTML/TEI tags, footnote backlink residue, public URLs, local filesystem paths, replacement characters, embedded newlines, or leading/trailing whitespace.
- Hashes in the filtered CSV match the current Source-note text.

## Accepted Official FRUS Cases

- 2 notes contain a second internal `Source:` string because the published FRUS note itself cites a source titled or labeled that way; these are not leading-label duplicates.
- 5 notes begin with a redacted source path such as `Source: [ ... not declassified`; these are official published FRUS forms and are retained.

## Files

- `copy-paste-source-notes.txt`: source-note text only, one note per paragraph.
- `copy-paste-source-notes.csv`: source-note rows only, with document context columns.
- `document-source-notes.csv`: full register, including status rows for documents without source notes.
- `source-note-style-audit.json`: machine-readable audit details.
