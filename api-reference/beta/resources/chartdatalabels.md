---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642325"
---
# <a name="chartdatalabels-resource-type"></a>ChartDataLabels リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartDataLabels](../api/chartdatalabels-get.md) | [ChartDataLabels](chartdatalabels.md) |chartDataLabels オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/chartdatalabels-update.md) | [ChartDataLabels](chartdatalabels.md) |ChartDataLabels オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|position|文字列|データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。|
|separator|文字列|グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。|
|showBubbleSize|ブール値|データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。|
|showCategoryName|ブール値|データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。|
|showLegendKey|ブール値|データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。|
|showPercentage|ブール値|データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。|
|showSeriesName|ブール値|データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。|
|showValue|ブール値|データ ラベルの値を表示するか非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[ChartDataLabelFormat](chartdatalabelformat.md)|グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
