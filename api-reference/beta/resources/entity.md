---
title: エンティティ リソースの種類
description: なし
ms.openlocfilehash: a59426c004663ae048118dcf1fba5cb64611eaf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071883"
---
# <a name="entity-resource-type"></a>エンティティ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="properties"></a>プロパティ
| プロパティ | 型  | 説明 |
|:---------|:------|:------------|
|id        |String | 読み取り専用。  |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "abstract": "true",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->
```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->