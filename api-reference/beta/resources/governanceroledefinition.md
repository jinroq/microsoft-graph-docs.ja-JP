---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 Azure リソースの場合は、所有者、リーダー、共同作成者など、Azure RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: c760cc04b8dae39c06d0dbc2c4821401bd75a699
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422508"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


ロール定義を表します。 Azure リソースの場合は、所有者、リーダー、共同作成者など、Azure RBAC の役割を表すことができます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション |リソースのロール定義のコレクションを一覧表示します。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。|

`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`

## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----|:----------|:----------|:----------|
|id         |文字列     |ロール定義の id。 |
|resourceId |String     |必須。 ロール定義に関連付けられているリソースの id。 |
|externalId   |String     |ロール定義の外部 id。|
|displayName|String     |ロール定義の表示名。|
|templateId | String | |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 ロール定義に関連付けられているリソース。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|ロール定義に関連付けられているロール設定。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "templateId":"String"
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
  "suppressions": []
}
-->
