# Publishing CraftRoster releases

This repository is the public distribution channel. The source repository is `hurlburtc-png/CraftRoster`, which may become private after the release mirror is tested.

## Publishing requirements

- Publish only a tagged, CI-tested version from the source repository.
- Mirror the **exact** tested `CraftRoster.zip` asset (do not rebuild it from a different commit).
- Publish SHA-256 checksum and a matching source archive for the same tag.
- Include the MIT license and preserve third-party notices.
- Verify `CraftRoster/CraftRoster.toc` is the only addon root inside the install ZIP.
- Confirm the published version and checksum match the source release.
- Never overwrite an existing release tag or silently replace a ZIP.
- Do not expose GitHub tokens, saved variables, local player data or private issues.

## Automation credentials

A source-repository GitHub Actions workflow needs an explicitly scoped credential with **Contents: Read and write** on this release repository. The source repository's default `GITHUB_TOKEN` does not automatically gain write access to a different repository. Use a fine-grained token or GitHub App installation credential stored as an Actions secret in the source repository, and grant only this release repository access. Never put a token in committed files.

## Transition

1. Verify mirror publishing with a test or tagged beta release.
2. Verify anonymous download, source archive and checksum.
3. Change the source repository to private.
4. Verify the development integration and hourly automation still work.
5. Verify the next automated release can still publish to this public repository.

**Current status:** Configuration documentation only; no release has been mirrored here yet.
