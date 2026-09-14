# Overout

[English](./README_EN.md)

> **コピーしたテキストを、集めて、整える。**

Overoutは、Windows上でCopyしたTextを取得・蓄積し、そのまま同じDocument上で整理・編集するための、Windows x64向けLocal-first Text acquisition / editing APPです。

Browser、Editor、Chatなどで行う通常のCopy操作を利用してTextを集め、必要に応じて整理・編集し、Local Fileへ出力できます。

## Current Release

| 項目 | 内容 |
|---|---|
| Product | `Overout` |
| Version | `v1.0.0` |
| Platform | `Windows x64` |
| Application | `Overout.exe` |
| Status | Release Package Fixed / Public Distribution Active |
| Public Release Date | 2026-09-11 |
| Standalone Price | `¥1,000` |
| Source Code | Not Publicly Released |

正式Release Packageはすでに固定済みです。GitHub上のDocumentation更新は、固定済みRelease Packageそのものを変更しません。

## Download / Purchase

Overout v1.0.0の正式Binaryは、GeneSIS公式BOOTHから配布しています。

**Standalone Product:** https://genesis-protocol.booth.pm/items/8828676

GitHub Repositoryでは、`Overout.exe`または正式Release ZIPを配布しません。

既存のProject: Code-NOAH Phase 1 Founder Support購入者には、Standalone版と**同一のOverout v1.0.0 Release Build**をSupplemental / Additional Deliverableとして提供しています。Founder専用Binaryは作成しません。

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

SALVAGEとPREPARATIONは別々のDocumentを扱うのではなく、同じShared Document Bufferに対するOperational Contextを切り替えます。

## SALVAGE

SALVAGEは、Windows Clipboard上のText更新を取得するModeです。

`ACTIVE / PASSIVE`はSalvagingのON / OFFではなく、**Textの取得方式**です。どちらを選択していても、SALVAGE Mode中にCopyされたTextはShared Document Bufferへ取り込まれます。

- **ACTIVE** — Layer Marker、alternating Tag、optional Timestamp等を利用しながら構造化して取得
- **PASSIVE** — 自動Tag / Layer Markerを抑え、CopyしたTextを元の形に近い状態で取得
- **Undo Last Capture** — 直前の1回分のSALVAGE取得を戻す
- **L.A.I.N Navi** — Clipboard Event / acquisition statusの確認
- **s-CO2** — Manual Layer Marker
- **File Output** — 現在のDocumentをLocal Fileへ出力
- **Clear** — Shared Document BufferをClear

Salvaging自体を停止したい場合は、**PREPARATIONへ切り替えるかOveroutを終了**してください。

## PREPARATION

PREPARATIONは、同じShared Document Bufferを直接整理・編集するOperational Contextです。PREPARATION中はClipboard Salvagingを行わず、通常のCopy / Cut / Pasteを使用できます。

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

`S.N.A.K.E.D.`（Space Normalization And Key Extraction Display）は、PREPARATIONにおける空行の検出・可視化・正規化に関するConcept名称で、v1.0.0では主にBlank Detection / Blank Compressへ反映されています。

## Quick Start

1. 正式配布ZIPを任意のFolderへ展開します。
2. `Overout.exe`を起動します。通常利用で管理者権限は必要ありません。
3. 起動時はSALVAGEです。
4. ACTIVEまたはPASSIVEを選び、Browser / Editor / Chat等で必要なTextをCopyします。
5. 直接編集や通常のCopy / Cut / Pasteを行う場合はPREPARATIONへ切り替えます。
6. 必要に応じてDetection、Search、C.O.D.E.C.、Blank Compress等で整理します。
7. File OutputからLocal Fileへ保存します。

設定は通常のLocal JSONとして次へ保存されます。

```text
%LOCALAPPDATA%\Overout\config.json
```

Overout v1.0.0は、Clipboard内容をGeneSISまたは外部Serviceへ送信するためのNetwork機能を必要としません。

## Release Verification

- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)

Windows AuthenticodeによるCode署名はありません。そのためSmartScreen等の警告が表示される場合があります。

**警告が表示されたことだけでMalwareと確定するわけではなく、警告がないことだけで安全性が証明されるものでもありません。** 出所とHashを確認してください。

## Documentation

- [Documentation Index](./docs/README.md)
- [Release Information](./docs/RELEASE_INFORMATION.md)
- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)
- [EULA](./docs/EULA.md)
- [Third-Party Software Notices](./docs/THIRD_PARTY_NOTICES.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE.md)
- [Security Policy](./SECURITY.md)
- [Changelog](./CHANGELOG.md)

正式Release Package内の日本語`EULA.txt`を利用条件のAuthoritative Textとして扱います。GitHub上の`docs/EULA.md`は、そのPackage EULAとbyte-for-byte同期した購入・Download前確認用Public Copyです。英語版はReference Translationです。

## Additional Guidance

次の案内コンテンツは順次追加予定です。これらの公開はOverout v1.0.0のBinary配布開始条件ではありません。

- Release記事：[Overout v1.0.0を公開しました。コピーしたテキストを、集めて、整える。](https://note.com/genesis_protocol/n/n4a2ac2d036fb)
- 操作案内記事：[Overout 操作 Guide](https://note.com/genesis_protocol/n/n402676e24c27)
- 操作案内動画：[Overout v1.0.0_Demo](https://www.youtube.com/watch?v=uv82vMVvrP4)

## GeneSIS / Project: Code-NOAH

Overoutは、`Project: Code-NOAH`配下の`Operation: Protocol-Overout`から生じたProductです。

G.E.N.Eは`Project: Code-NOAH`の直系成果物です。OveroutはG.E.N.Eの下位Productではなく、`Project: Code-NOAH`配下の`Operation: Protocol-Overout`から成立した別の成果物です。

- [GeneSIS_総合案内](https://note.com/genesis_protocol/n/n75a09dc02341)
- [G.E.N.E Repository](https://github.com/GeneSIS-Public/G.E.N.E)
- [Quick Questions](https://note.com/genesis_protocol/n/n6a2a06ad2698)
- [X](https://x.com/GeneSIS_PRCL)
- [YouTube](https://www.youtube.com/channel/UCFZC86OLvWEd7z4M9PLF98g)

## Contact

公開可能な通常不具合・Documentation Feedback・Development FeedbackはGitHub Issuesを使用できます。

購入、Founder Support、EULA、権利、Privacy、非公開不具合等は[Contact and Support](./docs/CONTACT_AND_SUPPORT.md)をご確認ください。

未修正のSecurity問題はPublic Issueへ投稿せず、[Security Policy](./SECURITY.md)の非公開経路を使用してください。

---

**……………………文脈をSalvageする。 GeneSIS by Concept Engineer's HQ.**

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
