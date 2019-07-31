---
title: workbookChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c5e469f5d95065fa3b5a161d510ca023e17f807a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007292"
---
# <a name="workbookchartdatalabels-resource-type"></a>workbookChartDataLabels リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorkbookChartDataLabels を取得する](../api/chartdatalabels-get.md) | [workbookChartDataLabels](workbookchartdatalabels.md) |chartDataLabels オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartdatalabels-update.md) | [workbookChartDataLabels](workbookchartdatalabels.md) |ChartDataLabels オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|position|string|データ ラベルの位置を表す DataLabelPosition 値。 使用可能な値は`None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、、 `Callout` `BestFit`です。|
|separator|string|グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。|
|showBubbleSize|ブール値|データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。|
|showCategoryName|ブール値|データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。|
|showLegendKey|ブール値|データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。|
|showPercentage|ブール値|データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。|
|showSeriesName|ブール値|データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。|
|showValue|ブール値|データ ラベルの値を表示するか非表示にするかを表すブール型の値。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[workbookChartDataLabelFormat](workbookchartdatalabelformat.md)|グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
