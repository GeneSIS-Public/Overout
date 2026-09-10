# Overout v1.0.0 — Known Limitations

[English](./KNOWN_LIMITATIONS_EN.md)

- **Document ID:** `OVEROUT-KNOWN-LIMITATIONS-V1.0.0`
- **Document Version:** 1.0
- **Status:** RELEASE CONTENT FINAL
- **Last Updated:** `2026-09-08`
- **Target:** `Overout v1.0.0 / Windows x64`

## 1. Scope

Release前のWindows実機試験までに確認された、または配布上明示すべき制限・注意事項です。

採用ONEFILE Binaryについて、Release Blockerとなる問題は確認されていません。

## 2. Windows x64

正式対象はWindows x64です。

macOS / Linux / Windows ARM64等を正式Support対象として保証するReleaseではありません。

## 3. Windows Authenticode

`Overout.exe`にはWindows Authenticode Code Signing Certificateによる署名がありません。

SmartScreen、Smart App Control、組織Policy、Browser Download保護等により警告・実行制限が表示される場合があります。

Package同梱のEd25519 Release Manifest SignatureはOrigin / Integrity確認用であり、Windows Publisher表示やSmartScreen Reputationを置き換えません。

## 4. Japanese IME / ASCII Symbols

Windows Japanese IME / Tkの組合せでは、一部Key Eventが通常の半角ASCII入力と異なる形で通知される場合があります。

v1.0.0には実機確認した互換経路への対応を含みますが、記号を確実に半角ASCIIとして入力する必要がある場合はEnglish input / IME OFFを推奨します。

## 5. Rare Superscript / Subscript Visual Clipping

一部Unicode上付き / 下付き文字等は、Windows / Tk / Fontの組合せによりわずかにClipして見える場合があります。

確認範囲では表示上の問題であり、Document Buffer内のText Data欠損としては扱っていません。

## 6. Clipboard Capture Scope

SALVAGEはWindows ClipboardのText更新を対象とします。

画像、独自Binary Format、APP固有Clipboard Object等を一般的に取り込むClipboard Managerではありません。

### Operational Clarification

Package同梱Known Limitationsには「Captureを必要としない時間はPASSIVEを使用」とする記載がありますが、**Overout v1.0.0のACTIVE / PASSIVEはいずれもSalvagingを行います。**

- ACTIVE — structured acquisition
- PASSIVE — near-raw acquisition
- Salvaging停止 — PREPARATIONへ切り替える、またはOveroutを終了

機密TextをCopyする可能性がありSalvagingを意図しない場合は、PREPARATIONへ切り替えてください。

## 7. Local Config

設定：

```text
%LOCALAPPDATA%\Overout\config.json
```

Overout独自方式による保存時暗号化を提供するものではありません。OS Account / Device / Backup先の保護はOperator側のWindows Security設定に依存します。

## 8. Future Version Compatibility

Maintenance / Feature Updateが提供される場合がありますが、将来Major Versionで同一仕様、同一UI、完全な設定互換性を永久に保証するものではありません。

## 9. Undo Last Capture

`Undo Last Capture`は一般Editor Undoではなく、**直前のSALVAGE Transaction 1回分**を戻す機能です。

PREPARATIONで本文を編集した後など、直前Captureを安全に特定できない場合は利用できないことがあります。

## 10. Release Position

```text
Adopted ONEFILE RC1: PASS
Known Release Blocker: NONE IDENTIFIED
Known Items: ACCEPTED LIMITATIONS / DISTRIBUTION NOTES
```

## 11. Related Documents

- [Release Verification](./RELEASE_VERIFICATION.md)
- [Contact and Support](./CONTACT_AND_SUPPORT.md)
- [Security Policy](../SECURITY.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
