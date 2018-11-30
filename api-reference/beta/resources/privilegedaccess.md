---
title: privilegedAccess リソースの種類
description: " たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。"
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074103"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
