---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
ms.openlocfilehash: d226c5edb3fecc3a2e27fae32060f786f790d7e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071685"
---
# <a name="chartdatalabels-resource-type"></a>ChartDataLabels リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartDataLabels](../api/chartdatalabels-get.md) | [ChartDataLabels](chartdatalabels.md) |chartDataLabels オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartdatalabels-update.md) | [ChartDataLabels](chartdatalabels.md) |ChartDataLabels オブジェクトを更新します。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->