---
title: convertIdResult リソースの種類
description: translateExchangeIds 関数によって実行される ID 形式変換の結果。
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535392"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
