---
title: operationError リソースの種類
description: TeamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 43486d21f7c8f852a965c5378688f826c26ac58b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009301"
---
# <a name="operationerror-resource-type"></a>operationError リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。

## <a name="operationerror-properties"></a>operationError プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|string (読み取り専用)|操作エラーコード。|
|message|string (読み取り専用)|操作エラーメッセージ。|

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
