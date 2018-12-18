---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
author: Jewan-microsoft
ms.openlocfilehash: bbb7b9457ce5a3d7ba9faf45d893ae86cdfd8b32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326909"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation リソースの種類

OneNote の特定の長時間操作の状態。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作の開始時刻です。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作によって返されるエラーです。|
|ID|string|操作 ID です。読み取り専用です。|
|lastActionDateTime| DateTimeOffset |操作の最後の操作の時間です。|
|resourceId|string|リソース ID。|
|resourceLocation|string|オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。 |
|status|string|操作の現在の状態: `notstarted`、`running`、`completed`、`failed` |
|percentComplete|string|操作がまだ `running` の状態の場合の操作達成率。

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[操作の取得](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |操作の現在の状態を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
