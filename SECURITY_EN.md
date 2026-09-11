# Overout — Security Policy

[日本語](./SECURITY.md)

- **Document Version:** 1.0
- **Status:** Active
- **Published By:** GeneSIS
- **Applicable Project:** `Project: Code-NOAH`
- **Applicable Operation:** `Operation: Protocol-Overout`
- **Applicable Product:** `Overout v1.x`
- **Applicable Repository:** `GeneSIS-Public/Overout`
- **Established:** `2026-09-10`
- **Effective From:** `2026-09-10`

> The Japanese version is the original and authoritative version.

This Policy defines the scope, private reporting route, report contents, and disclosure boundaries for unresolved Security issues related to Overout.

## 1. Scope

Covered: official Overout v1.x Release Packages, official `Overout.exe`, official Repository Documentation, Release / Verification Information, and other expressly covered Deliverables.

Generally excluded: development/internal/unreleased builds, third-party modified or repacked packages, unofficial patches/builds, unrelated external-product-only issues, social engineering/spam/DoS, and unlawful or unauthorized scenarios.

### Supported Versions

| Version | Security Support |
|---|---|
| Overout v1.0.0 | Officially released — Covered |
| Development / Internal / Unreleased | Not covered |

## 2. Private Reporting

Do not post unresolved Security details publicly.

When GitHub Private Vulnerability Reporting is enabled, use it. Otherwise contact:

`genesis.official.poc@mail.com`

Subject:

```text
[Security Report]
```

When uncertain, use the private route.

## 3. Information to Include

Include where possible: Overout Version, package source, Windows environment, summary, date/time, minimal reproduction steps, expected impact, required privileges, safely redacted logs/screenshots, relevant hashes, workaround, disclosure status, and preferred contact method.

Use synthetic/minimal Clipboard samples rather than real confidential content.

## 4. Information Not to Send

Do not send passwords, tokens, API keys, private keys, authentication/2FA/backup codes, complete payment information, unnecessary purchaser information, personal or third-party private data, confidential Clipboard Text, complete secret-containing buffers, unnecessary local files, or unsolicited executable exploits/malware.

See the [Privacy Notice](./docs/PRIVACY_NOTICE_EN.md).

## 5. Testing and Disclosure Boundaries

Do not access unauthorized accounts/devices/files/data, collect third-party Clipboard or document data, modify/delete/destroy data, perform DoS, use social engineering, attack/track third parties, distribute malware, or violate law, the EULA, or third-party rights.

This Policy does not authorize unlawful conduct or create a safe harbor.

## 6. Response Policy

GeneSIS may investigate, request information, assess impact, provide workarounds, prepare maintenance updates, revise Documentation, or publish a Security Notice.

No reply, fix, deadline, advisory, or specific result is guaranteed. Disclosure decisions are made by the GeneSIS-Operator.

This Policy does not create an NDA, reward program, or bug bounty.

## 7. Non-Security Matters

General usage, feature requests, minor UI issues, publicly safe ordinary defects, Windows/Tk/IME compatibility, Known Limitations, absence of Authenticode, SmartScreen warnings, purchases, Founder Support, EULA/rights, and Privacy requests are generally not Security reports.

See [Contact and Support](./docs/CONTACT_AND_SUPPORT_EN.md).

## 8. Release Integrity Anomalies

For ZIP/EXE hash mismatches, manifest/signature inconsistencies, missing verification artifacts, or suspected tampering, do not run the Package and first use [Release Verification](./docs/RELEASE_VERIFICATION_EN.md).

If concern remains after re-download, use the private route.

## 9. Related Documents

- [Release Verification](./docs/RELEASE_VERIFICATION_EN.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS_EN.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT_EN.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE_EN.md)
- [EULA — English Reference Translation](./docs/EULA_EN.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
