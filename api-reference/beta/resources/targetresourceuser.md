---
title: targetResourceUser リソースの種類
description: 追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。 TargetResource リソースから派生します。
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069763"
---
# <a name="targetresourceuser-resource-type"></a>targetResourceUser リソースの種類
追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。 [TargetResource](targetresource.md)リソースから派生します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|userPrincipalName|String|ユーザーの一意の Id を示します。 特定のユーザーのユーザー Id を参照します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->