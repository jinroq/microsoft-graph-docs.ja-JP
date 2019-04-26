---
title: privilegedAccess リソースの種類
description: " たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563676"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権 id 管理 (PIM) サービスによって提供される機能のグループを表します。 PIM が管理`privilegedAccess`するさまざまなプロバイダーを表すさまざまなインスタンス。たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。


`privilegedAccess`現時点では読み取り専用です。 `PATCH` `DELETE` `POST` `PUT`エンティティセットでは、、、、または操作はサポートされていません。 `privilegedAccess`

## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----------|:----------|:----------|
|id         |String     |PIM によって管理されるプロバイダーの id です。|
|displayName|String     |PIM によって管理されるプロバイダーの表示名。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ   | 型                                         |説明|
|:---------------|:---------------------------------------------|:----------|
|リソース       |[governanceResource](../resources/governanceresource.md)コレクション            |プロバイダーのリソースのコレクション。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|プロバイダーのロール割り当てのコレクション。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション|プロバイダーのロール日のコレクション。|
|rolerequests 要求 |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|プロバイダーのロール割り当て要求のコレクション。|
|rolesettings |[governanceRoleSetting](../resources/governancerolesetting.md)コレクション|プロバイダーのロール設定のコレクション。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
