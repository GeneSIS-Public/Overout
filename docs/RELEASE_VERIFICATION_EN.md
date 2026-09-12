# Overout v1.0.0 — Release Verification

[日本語](./RELEASE_VERIFICATION.md)

- **Document Version:** 1.1
- **Status:** Canonical Package Verified / Public Distribution Active / Public Distribution Verification PASS
- **Published By:** GeneSIS
- **Product:** `Overout v1.0.0`
- **Platform:** `Windows x64`
- **Last Updated:** 2026-09-12

> The Japanese version is the original and authoritative version.

This document is the public verification record for the identity and integrity of the official Overout v1.0.0 Release Package. Public distribution is active through the GeneSIS Official BOOTH. This record covers both the Canonical Release Archive and verification of an archive re-downloaded through the actual public distribution route.

## 1. Official Release Archive

| Item | Official Value |
|---|---|
| File Name | `Overout_v1.0.0_Windows_x64.zip` |
| File Size | `10,365,863 bytes` |
| SHA-256 | `ba97cc581b5f765893940b6c8845b1f039c7f21847ef11ce649eb720ae126bd3` |

## 2. Adopted Binary

| Item | Official Value |
|---|---|
| File Name | `Overout.exe` |
| File Size | `10,570,682 bytes` |
| SHA-256 | `d541fb0ba43b829e74e7034562e0c0b1c9e51089ba9adc2161bb79647ac49afd` |

## 3. Release Identity / Manifest

| Item | Official Value |
|---|---|
| Release Identity SHA-256 | `ee7ca504f660366450899a7ed9966353e06762b6fb307b821bbe8adf92782448` |
| Release Manifest | `05_RELEASE_MANIFEST.json` |
| Manifest SHA-256 | `3c4e92a169efda20e2fd46ec23d539220c44c7d6875eb1cca1c53d5774b29758` |
| Detached Signature | `06_RELEASE_MANIFEST.sig` |
| Signature Size | `64 bytes` |
| Signature SHA-256 | `2be37942e53ca65dee9f83d6f033e04d9b72ebf2a69e1d0d21b56aca71230d1e` |
| Algorithm | `Ed25519` |
| Signing Key ID | `GENESIS-RELEASE-SIGNING-KEY-001` |
| Canonical JSON Profile | `GENESIS-CANONICAL-JSON-1` |

## 4. SHA256SUMS / Public Key

| Item | Official Value |
|---|---|
| SHA256SUMS | `07_SHA256SUMS.txt` |
| Entries | `20` |
| SHA256SUMS SHA-256 | `8dfba240e26b0b2298ba29c6a1e8cb104e6e9106fb0d95d9531f1fd838aa3bbf` |
| Public Key | `08_GENESIS_RELEASE_PUBLIC_KEY.pem` |
| Public Key File SHA-256 | `4138a950a661ed9a506733f646070f51f529a667c4163a6726ee45f9b8c7a610` |
| Raw Public Key Fingerprint SHA-256 | `6b180843342001a64a32db6ca414c53c01b96877481209c4ebaae433aecf6450` |

## 5. ZIP / EXE Verification

```powershell
Get-FileHash .\Overout_v1.0.0_Windows_x64.zip -Algorithm SHA256
Get-FileHash .\Overout.exe -Algorithm SHA256
```

Do not extract or run a Package when the calculated value does not match the official hash.

## 6. Ed25519 Verification

Using OpenSSL 3.x:

```powershell
openssl pkeyutl -verify -rawin -pubin `
  -inkey ".\08_GENESIS_RELEASE_PUBLIC_KEY.pem" `
  -in ".\05_RELEASE_MANIFEST.json" `
  -sigfile ".\06_RELEASE_MANIFEST.sig"
```

The signature covers the exact bytes of the Release Manifest.

## 7. Authenticode / SmartScreen

`Overout.exe` is not signed with Windows Authenticode.

The Ed25519 Release Manifest Signature is for Release provenance / integrity and does not replace Authenticode or SmartScreen reputation.

## 8. Canonical / Public Distribution Status

On 2026-09-12, the Overout v1.0.0 archive was re-downloaded through the actual GeneSIS Official BOOTH public distribution route and its SHA-256 was compared with the Canonical Release Archive.

Re-downloaded archive SHA-256:

```text
ba97cc581b5f765893940b6c8845b1f039c7f21847ef11ce649eb720ae126bd3
```

The value matches the Canonical Release Archive, confirming byte-level identity of the re-downloaded archive.

```text
Canonical Archive Verification: PASS
Public Distribution: ACTIVE
Public Route SHA-256 Verification: PASS
Public Distribution Verification: PASS
Failures: NONE
```

## 9. Security Concern

For unresolved concerns involving an official Package, do not post exploitable details publicly. Use the [Security Policy](../SECURITY_EN.md).

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
