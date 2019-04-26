---
title: convertIdResult リソースの種類
description: translateExchangeIds 関数によって実行される ID 形式変換の結果。
localization_priority: Normal
ms.openlocfilehash: 5981f75ee071777f9119d0db2c0078153a160180
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341041"
---
# <a name="convertidresult-resource-type"></a>convertIdResult リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[translateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| sourceId | String | 変換された識別子。 この値は、元の、変換されていない識別子です。 |
| targetId | String | 変換された識別子。 変換が失敗した場合、この値は表示されません。 |
| errorDetails | [genericerror](genericerror.md) | 変換エラーの理由を示す error オブジェクト。 この値は、変換に成功した場合は表示されません。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
