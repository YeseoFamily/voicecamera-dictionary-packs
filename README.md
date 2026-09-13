# VoiceCamera dictionary packs

Versioned, offline bilingual dictionary packs distributed for the VoiceCamera mobile app.

## Distribution contract

- The app reads a signed/versioned index before presenting a download.
- Each pack is published as an immutable GitHub Release asset with its SHA-256 checksum.
- A pack is downloaded only after explicit user confirmation, verified before activation, and kept locally for offline use.
- The app retains the previously verified pack if an update fails.

## Initial status

This repository currently contains distribution metadata only. No dictionary dataset is published yet.

## Content and licensing

Every published pack must include a machine-readable manifest, provenance, license text, attribution, and any required share-alike notices. Content must be reviewed for license compatibility before release. In particular, Wikimedia/Wiktionary-derived data is only published with the applicable CC BY-SA 4.0 attribution and notice requirements.

## Release process

1. Generate a pack from an approved source using a reproducible script.
2. Validate schema, entry quality, language pair, size, and SHA-256.
3. Perform license and attribution review.
4. Publish an immutable GitHub Release asset and update the index only after review.
5. Keep release notes with source version, generator revision, checksums, and known limitations.

## Planned language pairs

- English ↔ Korean
- Japanese ↔ English
- Spanish ↔ English

The product UI is localized independently from dictionary content; a device locale never silently changes the user’s chosen learning pair.
