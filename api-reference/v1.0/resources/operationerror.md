---
title: operationError リソースの種類
description: TeamsAsyncOperation で発生したエラーをについて説明します。
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824585"
---
# <a name="operationerror-resource-type"></a>operationError リソースの種類



[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。

## <a name="operationerror-properties"></a>operationError プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|code|文字列 (読み取り専用)|操作のエラー コードです。|
|message|文字列 (読み取り専用)|エラー メッセージを操作します。|

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
