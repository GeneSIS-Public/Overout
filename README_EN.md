# Overout

[日本語](./README.md)

> **Collect copied text. Organize it in place.**

Overout is a local-first text acquisition / editing application for Windows x64. It collects text through ordinary Copy operations in browsers, editors, chats, and other applications, then lets the Operator organize and edit that text in the same document before writing it to a local file.

## Current Release

| Item | Details |
|---|---|
| Product | `Overout` |
| Version | `v1.0.0` |
| Platform | `Windows x64` |
| Application | `Overout.exe` |
| Status | Release Package Fixed / Public Distribution Active |
| Public Release Date | 2026-09-11 |
| Standalone Price | `JPY 1,000` |
| Source Code | Not Publicly Released |

The official Release Package is already fixed. Updates to GitHub Documentation do not modify that fixed Release Package.

## Download / Purchase

The official Overout v1.0.0 binary is available through the GeneSIS Official BOOTH.

**Standalone Product:** https://genesis-protocol.booth.pm/items/8828676

This GitHub Repository does not distribute `Overout.exe` or the official Release ZIP.

Existing Project: Code-NOAH Phase 1 Founder Support purchasers receive the **same Overout v1.0.0 Release Build** as a Supplemental / Additional Deliverable. No Founder-only Overout binary is created.

- [GeneSIS BOOTH](https://genesis-protocol.booth.pm/)
- [Project: Code-NOAH Phase 1 Founder Support](https://genesis-protocol.booth.pm/items/8664431)

## Basic Workflow

```text
External App / Browser / Chat / Editor
        │
        │ Copy
        ▼
Windows Clipboard
        │
        │ SALVAGE
        ▼
Shared Document Buffer
        │
        │ Mode Change
        ▼
PREPARATION
        │
        ├─ Direct Edit
        ├─ Detection
        ├─ Search
        ├─ Structural Intervention
        ├─ C.O.D.E.C.
        └─ Blank Compress
        │
        ▼
Local File Output
```

> **One Shared Document Buffer / Two Operational Contexts.**

SALVAGE and PREPARATION do not operate on separate documents. They switch Operational Contexts while using the same Shared Document Buffer.

## SALVAGE

`ACTIVE / PASSIVE` are acquisition methods, not an on/off switch for Salvaging. In either method, Text copied while SALVAGE is active is acquired into the Shared Document Buffer.

- **ACTIVE** — structured acquisition with Layer Markers, alternating Tags, and optional Timestamps
- **PASSIVE** — near-raw acquisition without automatic Tags / Layer Markers
- **Undo Last Capture** — removes the latest single SALVAGE acquisition transaction
- **L.A.I.N Navi** — shows Clipboard Event / acquisition status
- **s-CO2** — manual Layer Marker operation
- **File Output** — writes the current document to a local file
- **Clear** — clears the Shared Document Buffer

To stop Salvaging, **switch to PREPARATION or exit Overout**.

## PREPARATION

PREPARATION is the editing and organization Operational Context for the same Shared Document Buffer. Clipboard Salvaging is stopped in PREPARATION, so ordinary Copy / Cut / Paste can be used.

Primary functions include Direct Editing, P.R.E.S.S., C.O.D.E.C. 1–0, I.C. Move, Blank Detection, Layer Detection, Word Search, Structural Intervention, Blank Compress, and Right-click Edit.

`S.N.A.K.E.D.` (Space Normalization And Key Extraction Display) is the Concept name concerning blank-line detection, visualization, and normalization in PREPARATION. In v1.0.0 it is reflected mainly in Blank Detection / Blank Compress.

## Quick Start

1. Extract the official distribution ZIP.
2. Start `Overout.exe`. Administrator privileges are not required for normal use.
3. Overout starts in SALVAGE.
4. Select ACTIVE or PASSIVE and Copy the Text you want.
5. Switch to PREPARATION for direct editing or ordinary Copy / Cut / Paste.
6. Organize the text as needed.
7. Save through File Output.

```text
%LOCALAPPDATA%\Overout\config.json
```

Overout v1.0.0 does not require network functionality to send Clipboard contents to GeneSIS or an external service.

## Release Verification

- [Release Verification](./docs/RELEASE_VERIFICATION_EN.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS_EN.md)

The executable is not signed with Windows Authenticode, so SmartScreen or similar warnings may appear. A warning alone does not establish malware, and the absence of a warning alone does not establish safety.

## Documentation

- [Documentation Index](./docs/README_EN.md)
- [Release Information](./docs/RELEASE_INFORMATION_EN.md)
- [Release Verification](./docs/RELEASE_VERIFICATION_EN.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS_EN.md)
- [EULA — English Reference Translation](./docs/EULA_EN.md)
- [Third-Party Software Notices](./docs/THIRD_PARTY_NOTICES_EN.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT_EN.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE_EN.md)
- [Security Policy](./SECURITY_EN.md)
- [Changelog](./CHANGELOG_EN.md)

The authoritative terms for Overout v1.0.0 are the Japanese `EULA.txt` included in the official Release Package. `docs/EULA.md` is a byte-for-byte synchronized public copy. The English EULA is a non-authoritative Reference Translation.

## Additional Guidance

These materials may be added later and are not prerequisites for starting binary distribution:

- Release article (Japanese): https://note.com/genesis_protocol/n/n4a2ac2d036fb
- Operation guide article: Preparing <!-- PLACEHOLDER: NOTE_OVEROUT_GUIDE -->
- Operation guide video: Preparing <!-- PLACEHOLDER: YOUTUBE_OVEROUT_GUIDE -->

## GeneSIS / Project: Code-NOAH

G.E.N.E is a direct-line deliverable of `Project: Code-NOAH`. Overout is not a subordinate Product of G.E.N.E; it is a separate deliverable created through `Operation: Protocol-Overout` within `Project: Code-NOAH`.

- [GeneSIS General Information](https://note.com/genesis_protocol/n/n75a09dc02341)
- [G.E.N.E Repository](https://github.com/GeneSIS-Public/G.E.N.E)
- [Quick Questions](https://note.com/genesis_protocol/n/n6a2a06ad2698)
- [X](https://x.com/GeneSIS_PRCL)
- [YouTube](https://www.youtube.com/channel/UCFZC86OLvWEd7z4M9PLF98g)

## Contact

For purchases, Founder Support, EULA, rights, Privacy, or non-public defects, see [Contact and Support](./docs/CONTACT_AND_SUPPORT_EN.md).

Do not post unresolved Security issues publicly. Use the private route described in the [Security Policy](./SECURITY_EN.md).

---

**……………………Salvage the context. GeneSIS by Concept Engineer's HQ.**

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
