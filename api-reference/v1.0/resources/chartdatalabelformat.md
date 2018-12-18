---
title: ChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: 4c8961eb884a5ab603feda368934795cb73915d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356477"
---
# <a name="chartdatalabelformat-resource-type"></a>ChartDataLabelFormat リソースの種類

グラフのデータ ラベルの書式設定プロパティをカプセル化します。


## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。|
|font|[WorkbookChartFont](chartfont.md)|グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->