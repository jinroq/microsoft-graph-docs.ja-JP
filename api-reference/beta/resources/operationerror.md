---
title: operationerror リソースの種類
description: teamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
ms.openlocfilehash: 957f1ed2960c33f2e7bc07f79e7f749a3b9f15a5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341764"
---
# <a name="operationerror-resource-type"></a>operationerror リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。

## <a name="operationerror-properties"></a>operationerror プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|string (読み取り専用)|操作エラーコード。|
|メッセージ​​|string (読み取り専用)|操作エラーメッセージ。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
