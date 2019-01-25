---
title: privilegedAccess リソースの種類
description: " たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512928"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権を持つユーザーの管理 (PIM) サービスによって提供される機能のグループを表します。 別のインスタンスの`privilegedAccess`PIM; によって管理されている別のプロバイダーを表します。たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。


`privilegedAccess`ここでは、読み取り専用です。 No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`privilegedAccess`のエンティティ セット。

## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----------|:----------|:----------|
|id         |String     |PIM によって管理されているプロバイダーの id。|
|displayName|String     |PIM によって管理されているプロバイダーの表示名。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ   | 型                                         |説明|
|:---------------|:---------------------------------------------|:----------|
|resources       |[governanceResource](../resources/governanceresource.md)コレクション            |プロバイダーのリソースのコレクションです。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|プロバイダーのロールの割り当てのコレクションです。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション|プロバイダーのロール定義のコレクションです。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|プロバイダーの役割の割り当て要求のコレクションです。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)コレクション|プロバイダーのロールの設定のコレクションです。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
