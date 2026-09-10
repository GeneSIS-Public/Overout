# Overout v1.0.0 End User License Agreement
## English Reference Translation

[日本語 Authoritative Text](./EULA.md)

- **Document Status:** RELEASE FINAL / OVEROUT v1.0.0
- **Target APP:** Overout
- **Target APP Version:** v1.0.0
- **EULA ID:** `OVEROUT-EULA-V1.0.0`
- **EULA Document Version:** 1.0
- **Last Updated:** `2026-09-08`

> **This English document is a non-authoritative Reference Translation.**
> The authoritative terms are the Japanese `EULA.txt` included in the official Overout v1.0.0 Release Package. The repository file `docs/EULA.md` is a byte-for-byte synchronized public copy of that Japanese Package EULA. If any inconsistency or difference in interpretation arises, the Japanese text governs to the extent permitted by applicable law.

## 0. Premise

This EULA (End User License Agreement, hereinafter the “Agreement”) defines the terms of use for Overout v1.0.0 (hereinafter the “Software” or “Overout”).

A person who uses the Software is referred to as an “Operator” in the Product. In this Agreement, the expression “user (Operator)” may be used where clarification of the legal meaning is necessary.

The Operator must review this Agreement before using the Software.

When the official distribution page displays, before purchase or Download, a link to this EULA and a notice that completion of purchase or Download will be treated as agreement to these terms, completion of the purchase or Download by the Operator in that state will be treated as indicating agreement to this Agreement.

Overout v1.0.0 does not include a function that creates an in-APP record of EULA consent. The official distribution page and the EULA included in the Package constitute the authoritative published terms of use.

If you do not agree to this Agreement, do not use the Software.

## 1. Definitions

1. **Developer / Rights Holder**
   The person who develops the Software or lawfully holds rights relating to the Software. The official display name, contact information, and other information are shown on the official distribution page, in Release Information, or in other official guidance.

2. **Software**
   The Overout v1.0.0 distribution, including `Overout.exe`, Overout-specific UI, functions, concrete implementation, names, related documents, and distribution materials.

3. **Operator**
   An individual or other user entity that uses the Software. The expression “user (Operator)” may be used for legal explanation.

4. **Operator Output**
   Text, plans, Code, analyses, materials, works, and other content that the Operator creates, edits, processes, or embodies by using Overout as a tool for Text acquisition / editing / organization. This does not include the Software itself, copies of the Software, modifications, derivative versions, concrete implementation, official documents, or Third-Party Elements themselves.

5. **Third-Party Elements**
   Third-party Software / Runtime Components bundled with the Software, including Python, Tcl/Tk, PyInstaller, OpenSSL, and others.

## 2. Product Position

Overout is a Text acquisition / editing APP that operates on Windows.

Its primary functions and Concepts include SALVAGE, PREPARATION, Shared Document Buffer, Clipboard Text Capture, P.R.E.S.S., C.O.D.E.C., I.C. Move, L.A.I.N Navi, s-CO2, and S.N.A.K.E.D.

S.N.A.K.E.D. (Space Normalization And Key Extraction Display) is the Concept name relating to detection, visualization, and normalization of blank lines in PREPARATION. In Overout v1.0.0, this concept is reflected mainly in Blank Detection and Blank Compress.

Overout v1.0.0 does not require an external Python environment for normal use.

The normal functions of Overout v1.0.0 do not require connection to an external Network Service.

## 3. License and Operator Output

Subject to compliance with this Agreement, the Developer grants the Operator a non-exclusive, non-transferable, and non-sublicensable right to use a legitimately obtained copy of the Software in a Windows environment that the Operator manages or is otherwise lawfully authorized to use.

Within the scope of this license, the Operator may:

- use a legitimately obtained copy of Overout;
- retain Backup copies to the extent reasonably necessary for use and preservation of the Software;
- use Overout for personal work, creation, research, study, planning, development, writing, information organization, and support of work for which the Operator is responsible;
- edit, process, publish, distribute, sell, provide to customers or third parties, or commercially use Operator Output at the Operator’s own judgment and responsibility.

When Operator Output contains third-party copyrighted works, confidential information, personal information, or other protected material, the Operator is responsible for confirming the required rights, permissions, and handling conditions.

Conditions for common organizational deployment, shared use by multiple users, use involving redistribution, OEM, White Label, SaaS, hosting, or incorporation into a service provided to third parties are governed by the conditions on the official distribution page or by separate permission from the Developer.

## 4. Prohibited Conduct

Except where permitted by applicable law or by separate express permission, the Operator must not:

1. reproduce, redistribute, sell, or provide the Software to a third party without authorization beyond the scope of use or Backup permitted by this Agreement;
2. publish, sell, distribute, or provide to a third party a modified, derivative, or altered version of the Software without the Developer’s prior permission;
3. represent all or part of the Software as a product of the Operator or a third party;
4. remove, alter, or conceal Copyright, License, origin, Developer, or other rights notices;
5. conduct reverse engineering, decompilation, disassembly, or other analysis for the purpose of obtaining non-public concrete implementation, except where permitted by law;
6. infringe the License, terms, or rights applicable to Third-Party Elements;
7. use the Software for unlawful or rights-infringing conduct, or for the purpose of facilitating such conduct;
8. incorporate the Software, its executable file, non-public concrete implementation, legally protected UI expression, or official documents into a product, Service, System, Platform, SaaS, OEM, White Label, or other third-party offering without the Developer’s prior permission.

This Article does not prohibit the Operator from using Overout as a tool to create, publish, sell, or commercially use Operator Output.

## 5. Clipboard / Local Data

While Overout is in SALVAGE Mode, when Text is copied in Windows and the Text on the Clipboard changes, Overout acquires that Text into the Shared Document Buffer.

In this Agreement and the bundled README, this Overout-specific acquisition process is referred to as `Salvaging / SALVAGE acquisition`.

ACTIVE / PASSIVE are differences in acquisition method, not an ON / OFF switch for Salvaging. Under either method, Text copied while SALVAGE Mode is active is subject to acquisition.

The Operator must take into account that the Clipboard may contain confidential information, personal information, third-party secrets, or other sensitive content. When performing Copy operations that are not intended for Salvaging, the Operator must take appropriate action according to the situation, such as switching to PREPARATION or exiting Overout.

Configuration is stored as a normal Local File at:

```text
%LOCALAPPDATA%\Overout\config.json
```

Overout does not guarantee that this Config is encrypted at rest using an Overout-specific method.

The Operator is responsible for appropriately managing the Windows Account, Device, Backup destination, and related environment.

## 6. Third-Party Elements

`Overout.exe` bundles Third-Party Elements including Python, Tcl/Tk, PyInstaller, and others.

Third-Party Elements are governed by their respective License terms.

See:

```text
GeneSIS_Overout_開示資料\03_第三者ソフトウェア・ライセンス情報_THIRD_PARTY_NOTICES.txt
GeneSIS_Overout_開示資料\04_COMPONENT_LICENSE_INDEX.csv
GeneSIS_Overout_開示資料\THIRD_PARTY_LICENSES\
```

This Agreement does not modify the License terms applicable to Third-Party Elements.

## 7. Update / Support / Future Versions

This Agreement defines the terms of use for Overout v1.0.0.

A legitimately obtained copy of Overout v1.0.0 may be retained as a Version covered by the license.

Maintenance or Feature Updates may be provided, but no specific Update, Support period, feature addition, or free provision of a future Version is guaranteed.

In this document, “Major Version” generally means a major Version update in which the leading Version number changes, such as `v1.x → v2.x`.

A future Major Version may substantially change functions, structure, or conditions of provision, and may be provided as a separate Product or as a separately paid offering.

Additional conditions concerning price, sales terms, Support conditions, Supplemental Deliverables, and similar matters are governed in priority by the official distribution page or other official guidance.

## 8. Ownership of Rights

Rights in Overout itself, the executable file, source code, proprietary concrete implementation, legally protected UI expression, names, related documents, distribution materials, and other legally protected Software materials belong to the Developer or other lawful rights holders.

This Agreement does not transfer to the Operator ownership, copyright, trademark rights, or other intellectual property rights relating to the Software.

Rights in content contained in Operator Output are governed by its creator, rights holders, applicable law, and individual contractual terms. The Developer does not acquire ownership or intellectual property rights in Operator Output merely because the Output was created or edited through Overout.

## 9. Disclaimer

The Software is provided “as is.”

To the extent permitted by law, the Developer does not guarantee completeness, accuracy, usefulness, fitness for a particular purpose, continuous operation, preservation of data, or complete compatibility with all Windows environments, IMEs, Fonts, or other environments.

The Operator is responsible, at the Operator’s own judgment and responsibility, for management of use of the Software, Clipboard content, File Output, editing results, configuration, and Backup.

To the extent permitted by law, the Developer is not liable for damage arising from use or inability to use the Software, data loss, configuration damage, or other causes related to the Software.

This Article does not exempt or limit the Developer’s liability to the extent that such exemption or limitation is invalid under the Consumer Contract Act or other mandatory law, or in cases of intentional misconduct, gross negligence, or other circumstances in which liability cannot legally be exempted or limited.

## 10. Termination of the License

If the Operator violates this Agreement, the Developer may terminate the license granted under this Agreement.

If the license is terminated, the Operator must stop using the Software and, where lawfully or appropriately requested by the Developer under this Agreement, delete or destroy copies, modifications, or unauthorized distributions of the Software.

Rights relating to Operator Output remain subject to applicable law, third-party rights, and individual agreements.

## 11. Governing Law and Dispute Resolution

This Agreement is governed by and interpreted in accordance with the laws of Japan.

If a dispute arises in connection with this Agreement or the Software, the Developer and the Operator will, where reasonably possible, discuss the matter in good faith and endeavor to resolve it.

If the dispute cannot be resolved through discussion, it will be resolved by a court having jurisdiction under the laws of Japan.

## 12. Changes to This Agreement / Additional Conditions / Contact

The Developer may change this Agreement when necessary.

For a new official APP Version or a change in conditions of use, review the Agreement applicable to that Version, the official distribution page, or other official guidance.

Additional conditions concerning Support, Updates, sales conditions, organizational use, commercial integration, OEM, joint development, individual licensing, or other matters are governed by the official distribution page, bundled documents, Support Policy, individual agreements, or other official guidance.

Contact methods for the Developer are displayed on the official distribution page, in Release Information, in the README, or in other official guidance.

## 13. Copyright

Copyright © 2026 GeneSIS: Concept Engineer's HQ. All rights reserved.

End of EULA — English Reference Translation
