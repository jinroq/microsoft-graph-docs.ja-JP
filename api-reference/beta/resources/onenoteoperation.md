---
title: onenoteOperation リソースの種類
description: 長時間実行されている特定の OneNote 操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568872"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

長時間実行されている特定の OneNote 操作の状態。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作の開始時刻。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作によって返されたエラー。|
|id|string|操作 id。読み取り専用です。|
|lastactiondatetime| DateTimeOffset |操作の最後の操作の時刻。|
|resourceId|string|リソース id。|
|resourceLocation|string|オブジェクトのリソース URI。 たとえば、コピーされたページまたはセクションのリソース URI。 |
|status|string|操作の現在の状態: `notstarted`、 `running` `completed`、、`failed` |
|percentComplete|string|操作がまだ状態の`running`場合の操作達成率。

## <a name="relationships"></a>関係
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[操作を取得する](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |操作の状態を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
