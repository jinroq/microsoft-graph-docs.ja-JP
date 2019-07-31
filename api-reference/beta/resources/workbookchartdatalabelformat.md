---
title: workbookChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd60187d5bc62675b53b4a0a254afa3632e9c1d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964003"
---
# <a name="workbookchartdatalabelformat-resource-type"></a>workbookChartDataLabelFormat リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのデータ ラベルの書式設定プロパティをカプセル化します。


## <a name="methods"></a>メソッド
None

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|fill|[workbookChartFill](workbookchartfill.md)|現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。|
|font|[workbookChartFont](workbookchartfont.md)|グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。 読み取り専用です。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
