---
title: targetResourceUser リソースの種類
description: 追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。 TargetResource リソースから派生します。
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831929"
---
# <a name="targetresourceuser-resource-type"></a>targetResourceUser リソースの種類
追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。 [TargetResource](targetresource.md)リソースから派生します。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
