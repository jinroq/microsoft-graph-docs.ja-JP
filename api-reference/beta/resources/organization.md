---
title: 組織リソースの種類
description: 'Azure Active Directory テナントを表します。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3415edebdb792a931abf2b79a591ef3729d2cf6
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667506"
---
# <a name="organization-resource-type"></a>組織リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーやアプリケーションがサインインする Azure Active Directory テナントを表します。 このリソースでは読み取りおよび更新操作のみがサポートされ、作成と削除はサポートされません。 [directoryObject](directoryobject.md) から継承します。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[組織を取得する](../api/organization-get.md) | [organization](organization.md) |組織オブジェクトのプロパティと関係を読み取ります。|
|[Update organization](../api/organization-update.md) | [organization](organization.md)  |organization オブジェクトを更新します。 更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ | 型   | 説明 |
|:-------- |:---- |:----------- |
| assignedPlans | [assignedPlan](assignedplan.md) コレクション | テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。 |
| businessPhones | String コレクション | 組織の電話番号。 **メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。 |
| city | String | 組織の住所の市区町村名。 |
| country | String | 組織の住所の国/地域名。 |
| countryLetterCode | String | 組織の国/地域の省略形。 |
| createdDateTime | DateTimeOffset | 組織作成時のタイムスタンプです。 値は変更できず、組織が作成されると自動的に設定されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
| deletedDateTime | DateTimeOffset | ISO 8601 形式を使用して Azure AD テナントが削除されたときの日時を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります: `'2014-01-01T00:00:00Z'`。 読み取り専用。 |
| displayName | String | テナントの表示名。 |
| id | 文字列 | テナント ID。組織 (またはテナント) を表す一意の識別子です。 [directoryObject](directoryobject.md) から継承されました。 キー。 null 許容型ではありません。 読み取り専用です。 |
| isMultipleDataLocationsForServicesEnabled | Boolean | 組織の Multi-Geo が有効の場合 **true**、組織の Multi-Geo が有効ではない場合 **false**、**null** (既定)。 読み取り専用です。 詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。 |
| marketingNotificationEmails | String collection | null 許容ではありません。 |
| objectType | String | オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。 |
| onPremisesLastSyncDateTime | DateTimeOffset | 前回テナントがオンプレミスのディレクトリと同期した日付と時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
| onPremisesSyncEnabled | ブール値 | このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。 |
| postalCode | String | 組織の住所の郵便番号。 |
| preferredLanguage | String | 組織の優先言語。 ISO 639-1 コードに従う必要があります (例: "en")。 |
| privacyProfile | [privacyProfile](privacyprofile.md) | 組織のプライバシー プロファイル。 |
| provisionedPlans | [provisionedPlan](provisionedplan.md)コレクション | null 許容ではありません。 |
| securityComplianceNotificationMails | String collection ||
| securityComplianceNotificationPhones | String collection ||
| state | 文字列型 (String) | 組織の住所の都道府県名。 |
| street | String | 組織の住所のストリート名。 |
| technicalNotificationMails |String collection | null 許容ではありません。 |
| verifiedDomains | [verifiedDomain](verifieddomain.md)コレクション|このテナントに関連付けられているドメインのコレクション。null 許容ではありません。 |

## <a name="relationships"></a>関係

| リレーションシップ  | 型  |説明|
|:---------------|:--------|:----------|
|Certificateベース Authconfiguration|[Certificateベース Authconfiguration](certificatebasedauthconfiguration.md)コレクション| 証明書ベースの認証構成を管理するナビゲーションプロパティ。 このコレクションには、Certificateの1つのインスタンスのみを作成できます。  |
|extensions|[extension](extension.md) コレクション|組織リソースに対して定義されているオープン拡張機能のコレクション。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
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
  "objectType": "string",
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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
