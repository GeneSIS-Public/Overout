# Overout v1.0.0 — Release Information

[English](./RELEASE_INFORMATION_EN.md)

- **Document Version:** 1.0
- **Status:** Release Package Fixed / Public Distribution Preparing
- **Published By:** GeneSIS
- **Applicable Project:** `Project: Code-NOAH`
- **Applicable Operation:** `Operation: Protocol-Overout`
- **Product:** `Overout`
- **Version:** `v1.0.0`
- **Target Platform:** `Windows x64`
- **Public Release Date:** 準備中 <!-- PLACEHOLDER: PUBLIC_RELEASE_DATE -->

> 本書の日本語版を原文として管理します。英語版との間に解釈上の差異がある場合は、日本語版を優先します。

> 本書は固定済みRelease Packageの公開準備情報です。BOOTH上で一般配布が開始されるまで、Public Release開始を示すものではありません。

## 1. Release概要

| 項目 | 内容 |
|---|---|
| Product | `Overout v1.0.0` |
| Project | `Project: Code-NOAH` |
| Operation | `Operation: Protocol-Overout` |
| Platform | `Windows x64` |
| Application | `Overout.exe` |
| Distribution Form | ZIP Archive |
| Distribution Channel | GeneSIS公式BOOTH |
| Standalone Price | `¥1,000` |
| Founder Support | 同一Release BuildをAdditional Deliverableとして提供 |
| Source Code | 非公開 |

Standalone Product URL：

準備中 <!-- PLACEHOLDER: BOOTH_OVEROUT -->

正式Release Package：

```text
Overout_v1.0.0_Windows_x64.zip
```

Release Packageは固定済みです。GitHub Documentationを更新しても、固定済みZIPを再生成・変更しません。

Archive / EXEのHash、Release Identityおよび検証方法は[Release Verification](./RELEASE_VERIFICATION.md)を技術的Authorityとして参照してください。

## 2. Product Position

Overout v1.0.0は、Windows ClipboardからTextをSALVAGEし、同じShared Document Buffer上で人間がPREPARATIONを行うことによって、取得と整理を一つのLocal Workflowへ接続するText acquisition / editing APPです。

Architecture上の中心：

> **One Shared Document Buffer / Two Operational Contexts.**

OveroutはLocal-firstのStandalone Windows Applicationです。

通常利用のためにPython / pip / PyInstallerを別途Installする必要はありません。

Clipboard内容をGeneSISまたは外部Serviceへ送信するためのNetwork機能を必要としません。

## 3. SALVAGE

SALVAGEはWindows Clipboard上のText更新を取得するOperational Contextです。

主な機能：

- Clipboard Text Salvaging
- ACTIVE Acquisition
- PASSIVE Acquisition
- Layer Marker
- Alternating Tag
- Optional Timestamp
- Undo Last Capture
- L.A.I.N Navi
- s-CO2
- File Output
- Clear

`ACTIVE / PASSIVE`はいずれもSalvagingを行うAcquisition Methodです。ON / OFFの関係ではありません。

Salvagingを停止する場合は、PREPARATIONへ切り替えるかOveroutを終了します。

## 4. PREPARATION

PREPARATIONは同じShared Document Bufferを直接編集・整理するOperational Contextです。

PREPARATIONへ切り替えるとClipboard Listenerは停止し、通常のCopy / Cut / Pasteを使用できます。

主な機能：

- Direct Editing
- P.R.E.S.S.
- C.O.D.E.C. 1–0
- I.C. Move
- Blank Detection
- Layer Detection
- Word Search
- Structural Intervention
- Blank Compress
- Right-click Edit

## 5. Local Configuration / Output

Configuration：

```text
%LOCALAPPDATA%\Overout\config.json
```

File Outputで現在のShared Document BufferをLocal Fileへ出力できます。

## 6. Distribution

正式BinaryはGeneSIS公式BOOTHから配布します。

GitHub Repositoryでは`Overout.exe`または正式Release ZIPを配布しません。

Standalone購入者とG.E.N.E Founder Support購入者向けAdditional Deliverableで、別Build / Founder-only Binaryは作成しません。同一の固定済みOverout v1.0.0 Release Buildを提供します。

## 7. Release / Update Policy

正規に入手したOverout v1.0.0は、そのVersionとして継続して保持・利用できます。

v1.xにMaintenance / Feature Updateが提供される場合があります。

将来のMajor Versionは別Productまたは別途有償となる場合があります。価格、販売条件、Support条件は該当する公式案内を確認してください。

## 8. Windows Security / Integrity

`Overout.exe`はWindows Authenticodeで署名されていません。

Release IntegrityにはSHA-256、Release Manifest、Ed25519 Detached Signature、GeneSIS Release Public Keyを使用します。

これらはWindows AuthenticodeまたはSmartScreen Reputationを置き換えるものではありません。

## 9. EULA

正式Release Package内の日本語`EULA.txt`をAuthoritative EULAとして扱います。

GitHub上の[EULA](./EULA.md)はそのbyte-for-byte同期Public Copyです。

英語版は[Reference Translation](./EULA_EN.md)です。

## 10. Third-Party Software

Overout v1.0.0はStandalone Applicationとして必要なThird-Party Runtime Componentsを含みます。

詳細：[Third-Party Software Notices](./THIRD_PARTY_NOTICES.md)

## 11. Known Limitations

正式利用前に[Known Limitations](./KNOWN_LIMITATIONS.md)をご確認ください。

## 12. Support / Security / Privacy

- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [Security Policy](../SECURITY.md)
- [Privacy Notice](./PRIVACY_NOTICE.md)

未修正Security問題はPublic GitHub Issueへ投稿しないでください。

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
