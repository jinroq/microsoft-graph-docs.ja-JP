---
title: governanceRoleSetting リソースの種類
description: " ルールなど。"
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506320"
---
# <a name="governancerolesetting-resource-type"></a>governanceRoleSetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

役割の割り当てが作成または変更されたときに評価する必要がある各ロール定義の構成のセットを表します。 たとえば、役割の設定には "最大割り当て期間" ルール、"アクティブ化に必要な MFA" ルールなどが含まれます。

## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [governanceRoleSetting](../resources/governancerolesetting.md)コレクション|リソースのロール設定のコレクションを一覧表示します。|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |役割設定のプロパティと関係を読み取ります。|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |役割設定オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
|プロパティ               |型                                      |説明|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |rolesetting の id。|
|resourceId           |String                                  |必須。 ロール設定が関連付けられているリソースの id。|
|roleDefinitionId     |String                                  |必須。 ロール設定が関連付けられているロール定義の id。|
|isDefault            |ブール値                                 |読み取り専用。 rolesetting が既定の rolesetting であるかどうかを示します|
|lastUpdatedDateTime  |DateTimeOffset                          |読み取り専用です。 役割の設定が最後に更新された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|lastupdatedby        |String                                  |読み取り専用です。 rolesetting を最後に更新した管理者の表示名。|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|管理者が対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。|
|adminmembersettings  |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|管理者が直接メンバーの役割の割り当てを追加しようとしたときに評価されるルールの設定。|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。 現時点では、この設定はサポートされていません。|
|usermembersettings   |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが役割の割り当てをアクティブ化しようとしたときに評価されるルールの設定。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 このロール設定に関連付けられたリソース。|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|読み取り専用です。 このロール設定で適用されるロール定義。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
