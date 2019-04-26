---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 27b4b144f834f3b5eb4270a2875da5add10efb9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333758"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション |リソースのロール定義のコレクションを一覧表示します。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。|
`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`
## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----|:----------|:----------|:----------|
|id         |String     |ロール定義の id。 |
|resourceId |String     |必須。 ロール定義に関連付けられているリソースの id。 |
|externalId   |String     |ロール定義の外部 id。|
|displayName|文字列     |ロール定義の表示名。|
|templateId | String | |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 ロール定義に関連付けられているリソース。|
|rolesetting|[governanceRoleSetting](../resources/governancerolesetting.md)|ロール定義に関連付けられているロール設定。|

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
