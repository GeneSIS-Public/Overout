# Overout v1.0.0 — Known Limitations

[日本語](./KNOWN_LIMITATIONS.md)

- **Document ID:** `OVEROUT-KNOWN-LIMITATIONS-V1.0.0`
- **Document Version:** 1.0
- **Status:** RELEASE CONTENT FINAL
- **Last Updated:** `2026-09-08`
- **Target:** `Overout v1.0.0 / Windows x64`

> The Japanese version is the original and authoritative version.

## 1. Scope

These are limitations and distribution notes identified by pre-release Windows testing. No Release Blocker was identified in the adopted ONEFILE binary.

## 2. Windows x64 Only

The official target is Windows x64. macOS, Linux, and Windows ARM64 are not guaranteed as supported targets.

## 3. No Windows Authenticode Signature

`Overout.exe` is not signed with a Windows Authenticode certificate. SmartScreen, Smart App Control, organizational policy, or browser protection may display warnings or restrictions.

The bundled Ed25519 Release Manifest Signature is for origin / integrity verification and does not replace Windows Publisher identity or SmartScreen reputation.

## 4. Japanese IME / ASCII Symbols

Some Windows Japanese IME / Tk combinations may report key events differently from normal half-width ASCII input.

If reliable half-width ASCII symbol input is required, English input / IME OFF is recommended.

## 5. Rare Unicode Visual Clipping

Some superscript / subscript Unicode characters may appear slightly clipped depending on Windows, Tk, and fonts. This has been treated as a visual issue rather than loss of Text Data.

## 6. Clipboard Capture Scope

SALVAGE targets Windows Clipboard Text updates and is not a general manager for images, proprietary binary formats, or application-specific Clipboard objects.

### Operational Clarification

The Package Known Limitations contains historical wording suggesting use of PASSIVE when capture is not needed. In Overout v1.0.0, however, **both ACTIVE and PASSIVE perform Salvaging**.

- ACTIVE — structured acquisition
- PASSIVE — near-raw acquisition
- To stop Salvaging — switch to PREPARATION or exit Overout

If you may Copy confidential Text and do not intend to acquire it, switch to PREPARATION.

## 7. Local Config

```text
%LOCALAPPDATA%\Overout\config.json
```

Overout does not provide application-specific encryption-at-rest for this configuration file.

## 8. Future Compatibility

Future Major Versions are not guaranteed to preserve the same specification, UI, or complete configuration compatibility indefinitely.

## 9. Undo Last Capture

`Undo Last Capture` is a one-level SALVAGE transaction undo, not a general editor Undo.

It may become unavailable after PREPARATION edits when the previous Capture transaction cannot be safely identified.

## 10. Release Position

```text
Adopted ONEFILE RC1: PASS
Known Release Blocker: NONE IDENTIFIED
Known Items: ACCEPTED LIMITATIONS / DISTRIBUTION NOTES
```

## 11. Related Documents

- [Release Verification](./RELEASE_VERIFICATION_EN.md)
- [Contact and Support](./CONTACT_AND_SUPPORT_EN.md)
- [Security Policy](../SECURITY_EN.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
