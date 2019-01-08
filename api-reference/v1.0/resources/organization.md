---
title: 組織リソースの種類
description: " 作成および削除はサポートされていません。 directoryObject から継承します。"
ms.openlocfilehash: b98455c52d963d4e523253dc2a3b75137be9e854
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748333"
---
# <a name="organization-resource-type"></a>組織リソースの種類

ユーザーやアプリケーションにサインインする Azure Active Directory のテナントを表します。 このリソースの読み取りと更新の操作のみがサポートされて作成および削除はサポートされていません。 [directoryObject](directoryobject.md) から継承します。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[組織を取得する](../api/organization-get.md) | [organization](organization.md) |組織オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/organization-update.md) | [organization](organization.md)  |organization オブジェクトを更新します。 更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。 |
|**オープン拡張機能**| 
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| 
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ

| プロパティ                             | 型                                                              | 説明                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | [assignedPlan](assignedplan.md) コレクション                        | テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。                                                                                                                                                                                                            |
| businessPhones                      | String コレクション                                         | 組織の電話番号です。 注意: 文字列のコレクションですに、1 つだけの数がこのプロパティに設定できます。                                                                                            |
| city                                 | String                                                            | 組織の住所の市区町村名                                                                                                                                                                                                                                        |
| country                              | String                                                            | 組織の住所の国/地域名                                                                                                                                                                                                                              |
| countryLetterCode                    | String                                                            | 組織の国/地域の略称                                                                                                                                                                                                                                     |
|createdDateTime|DateTimeOffset| 組織が作成された日時のタイムスタンプです。 値は変更できず、組織が作成されたときに自動的に設定されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
| deletedDateTime                    | DateTimeOffset                                                    | Azure AD テナントは、ISO 8601 形式を使用して削除されたときの日付と時刻を表すし、は、UTC 時刻では常にします。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。                                                                                     |
| displayName                          | String                                                            | テナントの表示名。                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | テナントの一意識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。                                                                                                                                                            |
|isMultipleDataLocationsForServicesEnabled|Boolean|**true の**場合組織は、複数地域で有効になっています。複数地域が有効な場合は**false**の組織ではありません。**null**(既定値)。 値の取得のみ可能です。 詳細については、[オンラインの複数の地域 OneDrive](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)を参照してください。|
| marketingNotificationEmails          | String コレクション                                                 | null 許容ではありません。                                                                                                                                                                                                                                                                        |
| onPremisesLastSyncDateTime               | DateTimeOffset                                                    | 前回テナントがオンプレミスのディレクトリと同期した日付と時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
| onPremisesSyncEnabled                       | Boolean                                                           | このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。                        |
| postalCode                           | String                                                            | 組織の住所の郵便番号                                                                                                                                                                                                                                      |
| preferredLanguage                    | String                                                            | 組織の優先言語。 ISO 639-1 コードに従う必要があります (例: "en")。                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | 組織のプライバシー プロファイル。                                                                                                                                                                                                                                              |
| provisionedPlans                     | [ProvisionedPlan](provisionedplan.md) コレクション                  | null 許容ではありません。                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | String コレクション                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | String コレクション                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String                                                            | 組織の住所の都道府県名                                                                                                                                                                                                                                       |
| street                               | String                                                            | 組織の住所の番地                                                                                                                                                                                                                                          |
| technicalNotificationMails           | String コレクション                                                 | null 許容ではありません。                                                                                                                                                                                                                                                                        |
| verifiedDomains                      | [VerifiedDomain](verifieddomain.md) コレクション                    | このテナントに関連付けられているドメインのコレクション。null 許容ではありません。                                                                                                                                                                                                                 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|組織に対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
