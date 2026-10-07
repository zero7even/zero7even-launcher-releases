# Zero7even Launcher Releases

Public distribution repository for official Zero7even Launcher releases.

This repository is intended for downloadable launcher builds and public update metadata. Launcher source code belongs in the private `zero7even-launcher` repository.

## Repository layout

```text
zero7even-launcher-releases/
├── windows-releases/
├── linux-releases/
├── macos-releases/
├── android-releases/
├── release-notes/
├── checksums/
├── update-manifests/
└── public-version-metadata/
```

Release artifacts are grouped by launcher version inside each platform directory.

Example:

```text
windows-releases/
└── 0.1.0/
    ├── Zero7even-Setup.exe
    └── Zero7even-Portable.zip
```

## Update metadata

`update-manifests/manifest-schema.json` defines the public update-manifest format.

`public-version-metadata/latest.json` exposes the current release-channel state without inventing a release before one exists.

Checksums use SHA-256 and are grouped by version.

## Security

This repository must contain only public release artifacts and metadata.

Do not publish source-only secrets, signing private keys, credentials, OAuth secrets, internal configuration, or private certificates.

## Related repository

`zero7even-launcher` contains the launcher source and build logic.

---

Copyright © Zero7even.
