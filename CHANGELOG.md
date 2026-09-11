# Overout — Changelog

[English](./CHANGELOG_EN.md)

- **Document Version:** 1.0
- **Published By:** GeneSIS
- **Applicable Project:** `Project: Code-NOAH`
- **Applicable Operation:** `Operation: Protocol-Overout`
- **Applicable Product Line:** `Overout v1.x`

この文書は、Overoutの正式Public Releaseについて、利用者に影響する追加、変更、修正、削除、CompatibilityおよびSecurity関連の変更をRelease単位で記録します。

内部開発履歴、Technical Spike、非公開Build、Release Gate、Audit工程、Public Release前の内部修正および利用者へ影響しない軽微な文書修正は、原則として記録しません。

## [Unreleased]

現在、固定済みOverout v1.0.0 Release Packageに対する未公開Product変更はありません。

## [v1.0.0] — 2026-09-11

### Release

| 項目 | 内容 |
|---|---|
| Product | `Overout` |
| Version | `v1.0.0` |
| Project | `Project: Code-NOAH` |
| Operation | `Operation: Protocol-Overout` |
| Platform | `Windows x64` |
| Application | `Overout.exe` |
| Release Package | `Overout_v1.0.0_Windows_x64.zip` |
| Distribution | GeneSIS公式BOOTH — https://genesis-protocol.booth.pm/items/8828676 |
| Public Release Date | 2026-09-11 |
| Source Code | Not Publicly Released |

Overout v1.0.0は、`Operation: Protocol-Overout`から成立した最初の正式Release Packageであり、2026-09-11にPublic Distributionを開始しました。

### Added

#### SALVAGE
- Windows Clipboard Text Salvaging
- ACTIVE / PASSIVE Acquisition
- Layer Marker / Alternating Tag / Optional Timestamp
- Undo Last Capture
- L.A.I.N Navi
- s-CO2 Marker
- File Output / Clear

ACTIVE / PASSIVEはいずれもSALVAGE Mode内のAcquisition Methodであり、どちらでもCopyされたTextをShared Document Bufferへ取り込みます。

#### PREPARATION
- Shared Document Buffer Direct Editing
- Standard Copy / Cut / Paste
- P.R.E.S.S.
- C.O.D.E.C.
- I.C. Move
- Blank Detection / Layer Detection
- Word Search
- Structural Intervention
- Blank Compress
- Right-click Edit

SALVAGEとPREPARATIONは同じShared Document Bufferに対するOperational Contextを切り替えます。

#### Application / Operation
- Windows x64 Standalone Application
- JA / EN UI
- Local Config / Local File Output
- Local-first Operation
- Clipboard内容をGeneSISまたは外部Serviceへ送信するためのNetwork機能を必要としない構成

### Distribution
- Standalone Productとしての提供開始
- 正式Binary配布先をGeneSIS公式BOOTHとして設定
- GitHubをPublic Documentation / Release / Verification Informationの公開場所として設定
- Project: Code-NOAH Phase 1 Founder Support購入者へ同一Release BuildをAdditional Deliverableとして提供
- Founder-only Binaryなし
- Source Code非公開

### Release Verification

固定値・検証手順は[Release Verification](./docs/RELEASE_VERIFICATION.md)をAuthorityとして参照してください。

### Known Limitations

[Known Limitations](./docs/KNOWN_LIMITATIONS.md)をご確認ください。

### Security

未修正Security問題は[Security Policy](./SECURITY.md)の非公開経路を使用してください。

### Notes

v1.0.0以前の非公開開発期間について個別Public Fix Listは公開しません。

## Related Documents

- [Overout README](./README.md)
- [Release Information](./docs/RELEASE_INFORMATION.md)
- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE.md)
- [Security Policy](./SECURITY.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
