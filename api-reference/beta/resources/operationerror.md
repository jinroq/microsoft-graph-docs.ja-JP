---
title: operationerror リソースの種類
description: teamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568914"
---
# <a name="operationerror-resource-type"></a>operationerror リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。

## <a name="operationerror-properties"></a>operationerror プロパティ
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
