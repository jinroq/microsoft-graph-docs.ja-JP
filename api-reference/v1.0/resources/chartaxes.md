---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569432"
---
# <a name="chartaxes-resource-type"></a>ChartAxes リソースの種類

グラフの軸を表します。


## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|categoryAxis|[WorkbookChartAxis](chartaxis.md)|グラフの項目軸を表します。値の取得のみ可能です。|
|系列軸|[WorkbookChartAxis](chartaxis.md)|3 次元グラフの系列軸を表します。値の取得のみ可能です。|
|数値軸|[WorkbookChartAxis](chartaxis.md)|軸の数値軸を表します。 値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
