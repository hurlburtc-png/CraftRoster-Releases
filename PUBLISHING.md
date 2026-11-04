# Publishing CraftRoster releases

This repository is the public distribution channel. Source development occurs separately in `hurlburtc-png/CraftRoster`.

## Two distinct deliverables

**Game addon:** publish the exact CI-tested **`CraftRoster.zip`** from a tagged source release. It must contain only one addon root, `CraftRoster/`, with `CraftRoster.toc` directly inside. Include SHA-256 checksum, release notes, source archive and license notices.

**Optional Windows updater:** publish separately as **`CraftRoster-Windows-Updater.zip`** or a clearly named signed installer, **never inside `CraftRoster.zip`**. It requires independent Windows testing, security review, provenance/checksum, instructions and version number. An addon release must not imply that an updater has been tested or released.

Do not reuse a release asset name ambiguously. Clearly distinguish addon ZIP, updater ZIP/installer and GitHub's auto-generated source archives on the release page.

## Publishing rules

- Mirror the **exact** tagged, CI-tested addon ZIP; never rebuild from another commit.
- Check SHA-256, archive root, matching TOC version and source tag.
- Publish immutable tags; never silently replace old assets.
- Keep source archive and bundled third-party notices/licenses.
- Never expose tokens, local SavedVariables or private issue contents.
- Verify public anonymous downloads after publishing.
- Keep release descriptions honest about native-client and native-Windows test status.

## Credentials and automation

Publishing from the private source repository to this public mirror requires a narrowly scoped GitHub App credential or fine-grained token with Contents write access to **this release repository**. The default source `GITHUB_TOKEN` cannot write to another repository. Never commit credentials.

A source release created by GitHub Actions using `GITHUB_TOKEN` may not trigger a separate `release: published` workflow. Verify the workflow trigger and resulting mirror run; do not assume a published source release reached the public mirror.

## Current status

The latest verified public addon release is **v0.8.0-beta.100**, published November 4, 2026. **No Windows updater is verified as published**. Documentation does not constitute a release.
