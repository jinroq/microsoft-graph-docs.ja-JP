---
title: governanceRoleDefinition リソースの種類
description: 役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528642"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション |リソースの役割の定義の一覧を表示します。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Id で指定されたロールの定義のエンティティのプロパティと関係を参照してください。|
No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされています`roleDefinitions`ここではエンティティのセットです。
## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----|:----------|:----------|:----------|
|id         |文字列     |役割の定義の id です。 |
|resourceId |String     |必須。 役割の定義に関連付けられているリソースの id です。 |
|externalId   |String     |役割の定義の外部の id です。|
|displayName|String     |役割の定義の表示名。|
|subjectCount|Int32     |省略可能。 ロールに割り当てられている被験者の数です。 リソースへのアクセスの要求元の状態を表します。 プロパティを取得するには、明示的に使用をしてください。`$select=subjectCount`クエリにします。|
|eligibleAssignmentCount|Int32|省略可能。 役割の定義に関連付けられている対象のロールの割り当ての数です。 プロパティを取得するには、明示的に使用をしてください。`$select=eligibleAssignmentCount`クエリにします。|
|activeAssignmentCount|Int32    |省略可能。 役割の定義に関連付けられているアクティブなロールの割り当ての数です。  プロパティを取得するには、明示的に使用をしてください。`$select=activeAssignmentCount`クエリにします。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 役割の定義に関連付けられているリソースです。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|役割の定義に関連付けられている役割の設定をします。|

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
