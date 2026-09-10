# Overout v1.0.0 — Release Information

[日本語](./RELEASE_INFORMATION.md)

- **Document Version:** 1.0
- **Status:** Release Package Fixed / Public Distribution Preparing
- **Published By:** GeneSIS
- **Applicable Project:** `Project: Code-NOAH`
- **Applicable Operation:** `Operation: Protocol-Overout`
- **Product:** `Overout`
- **Version:** `v1.0.0`
- **Target Platform:** `Windows x64`
- **Public Release Date:** Pending <!-- PLACEHOLDER: PUBLIC_RELEASE_DATE -->

> The Japanese version is the original and authoritative version.

> This document describes a fixed Release Package being prepared for public distribution. It does not by itself indicate that BOOTH public distribution has started.

## 1. Release Overview

| Item | Details |
|---|---|
| Product | `Overout v1.0.0` |
| Project | `Project: Code-NOAH` |
| Operation | `Operation: Protocol-Overout` |
| Platform | `Windows x64` |
| Application | `Overout.exe` |
| Distribution Form | ZIP Archive |
| Distribution Channel | GeneSIS Official BOOTH |
| Standalone Price | `JPY 1,000` |
| Founder Support | Same Release Build as an Additional Deliverable |
| Source Code | Not publicly released |

Standalone Product URL:

Preparing <!-- PLACEHOLDER: BOOTH_OVEROUT -->

Official Release Package:

```text
Overout_v1.0.0_Windows_x64.zip
```

The Release Package is already fixed. GitHub Documentation updates do not regenerate or modify the fixed ZIP.

See [Release Verification](./RELEASE_VERIFICATION_EN.md) as the technical authority for archive / EXE hashes, Release Identity, and verification procedures.

## 2. Product Position

Overout v1.0.0 is a text acquisition / editing application that SALVAGEs Text from the Windows Clipboard and connects acquisition and organization in one Local Workflow by allowing human PREPARATION on the same Shared Document Buffer.

> **One Shared Document Buffer / Two Operational Contexts.**

Overout is a local-first standalone Windows application. No separate Python / pip / PyInstaller installation is required for normal use.

Overout does not require network functionality to send Clipboard contents to GeneSIS or an external service.

## 3. SALVAGE

SALVAGE acquires Windows Clipboard Text updates.

Primary functions include Clipboard Text Salvaging, ACTIVE / PASSIVE Acquisition, Layer Markers, alternating Tags, optional Timestamps, Undo Last Capture, L.A.I.N Navi, s-CO2, File Output, and Clear.

ACTIVE and PASSIVE are both acquisition methods that perform Salvaging. To stop Salvaging, switch to PREPARATION or exit Overout.

## 4. PREPARATION

PREPARATION directly edits and organizes the same Shared Document Buffer.

Switching to PREPARATION stops the Clipboard Listener and enables ordinary Copy / Cut / Paste.

Primary functions include Direct Editing, P.R.E.S.S., C.O.D.E.C. 1–0, I.C. Move, Blank Detection, Layer Detection, Word Search, Structural Intervention, Blank Compress, and Right-click Edit.

## 5. Local Configuration / Output

```text
%LOCALAPPDATA%\Overout\config.json
```

File Output writes the current Shared Document Buffer to a local file.

## 6. Distribution

Official binaries are distributed through the GeneSIS Official BOOTH. This GitHub Repository does not distribute `Overout.exe` or the official Release ZIP.

The standalone route and the G.E.N.E Founder Support Additional Deliverable use the same fixed Overout v1.0.0 Release Build. No Founder-only binary is created.

## 7. Release / Update Policy

A legitimately obtained Overout v1.0.0 may continue to be retained and used as that Version.

Maintenance / Feature Updates may be provided within v1.x. A future Major Version may be a separate Product or separately paid offering.

## 8. Windows Security / Integrity

`Overout.exe` is not signed with Windows Authenticode.

Release Integrity uses SHA-256, a Release Manifest, an Ed25519 Detached Signature, and the GeneSIS Release Public Key. These do not replace Windows Authenticode or SmartScreen reputation.

## 9. EULA / Third-Party Software

The authoritative EULA is the Japanese `EULA.txt` in the official Release Package. [EULA.md](./EULA.md) is its byte-for-byte synchronized public copy. [EULA_EN.md](./EULA_EN.md) is a Reference Translation.

See [Third-Party Software Notices](./THIRD_PARTY_NOTICES_EN.md).

## 10. Support / Security / Privacy

- [Known Limitations](./KNOWN_LIMITATIONS_EN.md)
- [Contact and Support](./CONTACT_AND_SUPPORT_EN.md)
- [Security Policy](../SECURITY_EN.md)
- [Privacy Notice](./PRIVACY_NOTICE_EN.md)

Do not post unresolved Security issues in public GitHub Issues.

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
