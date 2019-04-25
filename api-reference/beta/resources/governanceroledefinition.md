---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547448"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション |リソースのロール定義のコレクションを一覧表示します。|
|[取得](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。|
`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`
## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----|:----------|:----------|:----------|
|id         |String     |ロール定義の id。 |
|resourceId |String     |必須。 ロール定義に関連付けられているリソースの id。 |
|externalId   |String     |ロール定義の外部 id。|
|displayName|String     |ロール定義の表示名。|
|subjectcount|Int32     |省略可能。 役割に割り当てられているサブジェクトの数。 これは、リソースへの要求者のアクセスの状態を表します。 プロパティを取得するには、クエリ`$select=subjectCount`で明示的にを使用してください。|
|eligibleAssignmentCount|Int32|省略可能。 役割の定義に関連付けられている対象の役割の割り当ての数。 プロパティを取得するには、クエリ`$select=eligibleAssignmentCount`で明示的にを使用してください。|
|active割り当てカウント|Int32    |省略可能。 ロール定義に関連付けられているアクティブなロール割り当ての数。  プロパティを取得するには、クエリ`$select=activeAssignmentCount`で明示的にを使用してください。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用。 ロール定義に関連付けられているリソース。|
|rolesetting|[governanceRoleSetting](../resources/governancerolesetting.md)|ロール定義に関連付けられているロール設定。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
