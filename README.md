# Humanity Speaks

**History deserves to be heard in its own words.**

Humanity Speaks is a public, source-aware collection of consequential speeches and human voices across history.

**Website:** https://humanityspeaks.teambotics.app/

## Status

This repository was initialized on 2026-11-04. The existing website is already deployed separately on Vercel and currently has a 33-speaker collection. **This initial commit does not claim to contain or deploy that existing website's source code.** Migration and verification are outstanding.

## Editorial commitments

- **Actual words, not just biographies.** Each speech should offer a readable primary text when its rights and source permit.
- **Provenance first.** Preserve speaker, occasion, date, original language, edition, source links, and transcription uncertainty.
- **No invented quotations.** Unverified text remains clearly marked; paraphrases never masquerade as transcripts.
- **Accessible and agent-readable.** Use semantic HTML and structured data; an iframe alone is not a reliable transcript for accessibility or indexing.
- **Durable links.** Keep speaker and speech URLs stable when moving deployments.
- **Context without endorsement.** Document historically important speech without treating inclusion as approval.

## Speech publication modes

1. **Full transcript** — where public domain status, permission, or a suitable license has been checked for the particular text and edition.
2. **Embedded original** — when the publisher allows framing and it provides a usable reading experience.
3. **Source-linked** — when reproduction or embedding is unavailable; show verified metadata and a direct link rather than fabricating text.

The project should record the source and rationale for each mode; legal status is evaluated per speech, translation, and jurisdiction rather than inferred from the speaker's identity.

## Repository plan

- `data/speeches/` — one structured record per speech, using `docs/speech-record.md`
- `src/` — application source once recovered and migrated from the live Vercel deployment
- `docs/` — editorial, provenance, accessibility, and deployment decisions

## Deployment safety

The existing Vercel project and `humanityspeaks.teambotics.app` remain the production baseline. Do not repoint the domain or replace production with this documentation-only repository. First recover the actual application source, reproduce the existing pages and routes, test a preview, then deliberately cut over.

## Contributions

Contributions of primary sources, corrections, translations with clear rights, and historical context are welcome. Include the original source URL and enough edition/date information for independent verification. Do not submit third-party copyrighted transcripts without a documented basis for republication.

## Licensing

**No blanket license is asserted for third-party speech texts, recordings, images, or translations.** A project-code license may be selected separately once the application source is migrated.
