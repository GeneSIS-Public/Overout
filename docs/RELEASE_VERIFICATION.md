# Overout v1.0.0 — Release Verification

[English](./RELEASE_VERIFICATION_EN.md)

- **Document Version:** 1.0
- **Status:** Canonical Package Verified / Public Distribution Verification Pending
- **Published By:** GeneSIS
- **Product:** `Overout v1.0.0`
- **Platform:** `Windows x64`

本書はOverout v1.0.0正式Release Packageの同一性・Integrityを確認するための公開Verification Recordです。

本書の存在だけでPublic Distribution開始を示すものではありません。

## 1. Official Release Archive

| Item | Official Value |
|---|---|
| File Name | `Overout_v1.0.0_Windows_x64.zip` |
| File Size | `10,365,863 bytes` |
| SHA-256 | `ba97cc581b5f765893940b6c8845b1f039c7f21847ef11ce649eb720ae126bd3` |

正式Archiveは固定済みです。再圧縮、File追加・削除・編集等を行うと通常SHA-256が変化します。

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
| SHA256SUMS File | `07_SHA256SUMS.txt` |
| Entry Count | `20` |
| SHA256SUMS SHA-256 | `8dfba240e26b0b2298ba29c6a1e8cb104e6e9106fb0d95d9531f1fd838aa3bbf` |
| Public Key File | `08_GENESIS_RELEASE_PUBLIC_KEY.pem` |
| Public Key File SHA-256 | `4138a950a661ed9a506733f646070f51f529a667c4163a6726ee45f9b8c7a610` |
| Raw Ed25519 Public Key Fingerprint SHA-256 | `6b180843342001a64a32db6ca414c53c01b96877481209c4ebaae433aecf6450` |

## 5. ZIP SHA-256 Verification

PowerShell:

```powershell
Get-FileHash .\Overout_v1.0.0_Windows_x64.zip -Algorithm SHA256
```

Expected:

```text
ba97cc581b5f765893940b6c8845b1f039c7f21847ef11ce649eb720ae126bd3
```

Mismatchの場合は実行・展開を中止し、正規配布元から再取得してください。

## 6. EXE SHA-256 Verification

```powershell
Get-FileHash .\Overout.exe -Algorithm SHA256
```

Expected:

```text
d541fb0ba43b829e74e7034562e0c0b1c9e51089ba9adc2161bb79647ac49afd
```

## 7. Ed25519 Manifest Signature Verification

Package内：

```text
GeneSIS_Overout_開示資料\
├─ 05_RELEASE_MANIFEST.json
├─ 06_RELEASE_MANIFEST.sig
├─ 07_SHA256SUMS.txt
└─ 08_GENESIS_RELEASE_PUBLIC_KEY.pem
```

OpenSSL 3.xでの検証例：

```powershell
openssl pkeyutl -verify -rawin -pubin `
  -inkey ".\08_GENESIS_RELEASE_PUBLIC_KEY.pem" `
  -in ".\05_RELEASE_MANIFEST.json" `
  -sigfile ".\06_RELEASE_MANIFEST.sig"
```

Ed25519署名はRelease Manifestのexact bytesに対するDetached Signatureです。Manifestを編集すると検証できません。

## 8. Authenticode / SmartScreen

`Overout.exe`はWindows Authenticodeで署名されていません。

Ed25519 Release Manifest SignatureはRelease Provenance / Integrity確認用であり、Windows AuthenticodeまたはSmartScreen Reputationを置き換えません。

SmartScreen警告の有無だけで安全性・危険性を判断しないでください。

## 9. Canonical Archive Verification

GeneSIS内部のCanonical Release Archiveは、Size / SHA-256比較、SHA256SUMS 20 / 20、Ed25519 Signature、Adopted Binary等のVerificationを完了しています。

```text
Canonical Archive Verification: PASS
Failures: NONE
```

## 10. Public Distribution Verification

BOOTH一般配布開始後、実際のPublic Distribution RouteからArchiveを取得し、File Name、File Size、SHA-256、展開可否、主要Fileの存在を再確認します。

現時点：

```text
Public Distribution Verification: PENDING
```

確認完了後、本Sectionの状態を更新します。

## 11. Release Integrity Concern

Hash mismatch、Manifest / Signature不整合、Verification Artifact欠落等を確認した場合は実行せず再Download・再検証してください。

公式配布物自体へのSecurity Concernが残る場合は、Public Issueへ詳細を投稿せず[Security Policy](../SECURITY.md)の非公開経路を使用してください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
