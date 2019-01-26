---
title: ChartFill リソースの種類
description: グラフ要素の塗りつぶしの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 17c123a3fb8c1fe2f2dd6f09b1fda3695bad0404
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577138"
---
# <a name="chartfill-resource-type"></a>ChartFill リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフ要素の塗りつぶしの書式設定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Clear](../api/chartfill-clear.md)|なし|グラフ要素の塗りつぶしの色をクリアします。|
|[Setsolidcolor](../api/chartfill-setsolidcolor.md)|なし|グラフ要素の塗りつぶしの書式設定を均一な色に設定します。|

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartFill"
}-->

```json
{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
