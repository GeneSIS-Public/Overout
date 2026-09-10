# Overout — Security Policy

[English](./SECURITY_EN.md)

- **Document Version:** 1.0
- **Status:** Active
- **Published By:** GeneSIS
- **Applicable Project:** `Project: Code-NOAH`
- **Applicable Operation:** `Operation: Protocol-Overout`
- **Applicable Product:** `Overout v1.x`
- **Applicable Repository:** `GeneSIS-Public/Overout`
- **Established:** `2026-09-10`
- **Effective From:** `2026-09-10`

本書は、Overoutに関する未修正Security問題の対象範囲、非公開報告経路、報告内容および開示上の基本方針を定めます。

## 1. Scope

対象：
- GeneSISが正式配布するOverout v1.x Release Package
- 正式`Overout.exe`
- 本Repository上の公式Public Documentation
- Release / Verification Information
- GeneSISが明示的に対象としたOverout関連Deliverable

原則対象外：
- Development Build、内部運用版、未公開試験版
- 第三者が改変・再Pack・再配布したPackage
- 非公式Patch / Build
- Overoutと無関係なWindows、Browser、第三者製品単独の問題
- Social Engineering、Spam、DoS目的の行為
- 違法・無権限・EULA違反を前提とするScenario

### Supported Versions

| Version | Security Support |
|---|---|
| Overout v1.0.0 | Release準備中 — 正式一般公開後に対象 |
| Development / Internal / Unreleased | 対象外 |

## 2. Private Reporting

未修正のSecurity問題をPublic GitHub Issue、note、X、YouTube、その他の公開場所へ投稿しないでください。

このRepositoryでGitHub Private Vulnerability Reportingが有効な場合は、その非公開報告経路を使用してください。

利用できない場合はGeneSIS公式窓口へ連絡してください。

`genesis.official.poc@mail.com`

メール件名：

```text
[Security Report]
```

Security問題か判断できない場合も、公開せず非公開経路を使用してください。

## 3. Information to Include

可能な範囲で、Overout Version、Package取得元、Windows Version / 実行環境、問題概要、確認日時、最小の再現条件・手順、想定Impact、必要権限、公開可能なLog / Screenshot、関連Hash、Workaround、既公開状況、希望連絡方法を含めてください。

Clipboard内容が関係する場合は、実際の機密TextではなくSynthetic / Minimal Sampleを使用してください。

## 4. Information Not to Send

Password、Token、API Key、秘密鍵、認証Code、2FA / Backup Code、完全な決済情報、不要なBOOTH購入者情報、個人情報、第三者の非公開情報、実際の機密Clipboard Text、秘密情報を含む完全なShared Document Buffer、不要なLocal File、依頼されていないExecutable Exploit / Malwareを送信しないでください。

Path、Log、Screenshot、Config、Document内の秘密情報は伏せてください。

GeneSISがPassword、認証Code、秘密鍵、完全な決済情報を求めることはありません。

個人情報の取扱いは[Privacy Notice](./docs/PRIVACY_NOTICE.md)をご確認ください。

## 5. Testing and Disclosure Boundaries

権限のないAccount / Device / File / DataへのAccess、第三者Clipboard / Document / Local Dataの収集、Dataの改変・削除・破壊、DoS、Social Engineering、第三者への攻撃・追跡・情報収集、Malware配布、法令・EULA・第三者権利に反する行為を行わないでください。

Fix、Workaroundまたは公式Security Noticeが用意されるまで、悪用可能な詳細の公開を控えるよう依頼する場合があります。

本Policyは違法Access等を許可するものでもSafe Harborを付与するものでもありません。

## 6. Response Policy

GeneSISは報告を確認し、必要に応じて再現・調査、追加情報確認、Impact評価、Workaround、Maintenance Update、Documentation修正、Security Noticeを検討します。

報告受領は返信、修正、期限、Advisoryその他の結果を保証しません。公開の要否・時期はGeneSIS-Operatorが判断します。

本PolicyはNDA、Reward Program、Bug Bountyを成立させるものではありません。

## 7. Non-Security Matters

一般的な使用方法、Feature Request、軽微なUI問題、安全に公開できる通常不具合、Windows / Tk / IME一般Compatibility、Known Limitations、Authenticode未署名自体、SmartScreen警告自体、購入 / Founder Support / EULA / 権利 / Privacyは通常Security Reportではありません。

通常問い合わせは[Contact and Support](./docs/CONTACT_AND_SUPPORT.md)をご確認ください。

## 8. Release Integrity Anomalies

ZIP / EXE Hash mismatch、Manifest / Signature不整合、Verification Artifact欠落、公式Package改変・置換が疑われる場合は実行せず[Release Verification](./docs/RELEASE_VERIFICATION.md)で再確認してください。

再取得後もConcernが残る場合は本Policyの非公開経路を使用してください。

## 9. Related Documents

- [Release Verification](./docs/RELEASE_VERIFICATION.md)
- [Known Limitations](./docs/KNOWN_LIMITATIONS.md)
- [Contact and Support](./docs/CONTACT_AND_SUPPORT.md)
- [Privacy Notice](./docs/PRIVACY_NOTICE.md)
- [EULA](./docs/EULA.md)

---

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.
