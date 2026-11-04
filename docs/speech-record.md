# Speech record contract (draft v0.1)

Each record represents **a specific speech or address**, not merely a speaker. One speaker can have many records.

Suggested JSON fields:

```json
{
  "id": "stable-speech-slug",
  "speaker": {
    "name": "Speaker name",
    "id": "stable-speaker-slug"
  },
  "title": "Documented title",
  "date": null,
  "place": null,
  "occasion": null,
  "original_language": null,
  "transcript": {
    "mode": "source-linked",
    "text": null,
    "source_url": null,
    "edition": null,
    "language": null,
    "verified_on": null,
    "verification_notes": null
  },
  "rights": {
    "basis": "unreviewed",
    "jurisdictions_reviewed": [],
    "evidence_urls": [],
    "reviewed_on": null,
    "notes": null
  },
  "media": [],
  "historical_context": null,
  "editorial_notes": [],
  "last_reviewed": null
}
```

Modes: `full-transcript`, `embedded-original`, `source-linked`.

Rights basis: `unreviewed`, `public-domain-verified`, `licensed`, `permission-granted`, `link-only`. A mode is not itself a legal determination.

Rules:
- Do not promote a source-linked entry to full transcript without reviewing the particular work and edition.
- Attribute translation and transcription separately from the original speaker.
- Preserve conflicting versions and uncertain dates in editorial notes; do not silently normalize them.
- Never use generated reconstructions as verbatim speech text.
- Validate outbound source links and embedded-source restrictions.
- Keep stable IDs independent of display title changes.

This is a proposed schema, not yet wired into the existing website.
