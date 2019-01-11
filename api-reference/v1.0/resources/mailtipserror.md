---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
localization_priority: Normal
ms.openlocfilehash: a4916bc34d7c76dc6c6592ee03e64b20a6485190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892094"
---
# <a name="mailtipserror-resource-type"></a>mailTipsError リソースの種類

操作中に発生するエラーです。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:-----|:-----|:-----|
| message | String | エラー メッセージ。 |
| code | String | エラー コード。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
