---
title: operationError リソースの種類
description: TeamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a46943fad974c2e7a12041e9def6a8a6ad6c9a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035715"
---
# <a name="operationerror-resource-type"></a>operationError リソースの種類



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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
