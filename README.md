# Dar al-Zilal — binary distribution

This repository contains downloadable game/launcher binaries and signed update metadata only. Game and launcher source repositories remain private.

- `game-preview-*`: beta candidates; drafts are invisible to players until the owner approves publication.
- `game-qa-*` and `channel-qa`: explicitly experimental updater acceptance tests. Never selected by preview/stable launchers.
- `blobs-*`: immutable SHA-256 addressed content shared across versions; these storage releases are not game releases.
- `channel-preview`: signed pointer to the currently approved beta. It is not created/advanced by code pushes.

Download only the launcher package provided by the developer. The launcher verifies release signatures, chunk hashes and complete installed files. It requires no GitHub account or token.

There is no approved stable release yet. Do not confuse QA storage/test assets with a stable game build.
