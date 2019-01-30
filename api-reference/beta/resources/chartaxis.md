---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640932"
---
# <a name="chartaxis-resource-type"></a>ChartAxis リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフの 1 つの軸を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis-get.md) | [ChartAxis](chartaxis.md) |chartAxis オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/chartaxis-update.md) | [ChartAxis](chartaxis.md)   |ChartAxis オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|majorUnit|object|2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。|
|maximum|object|数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minimum|object|数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minorUnit|object|2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[ChartAxisFormat](chartaxisformat.md)|グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。|
|majorGridlines|[ChartGridlines](chartgridlines.md)|指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|minorGridlines|[ChartGridlines](chartgridlines.md)|指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|title|[ChartAxisTitle](chartaxistitle.md)|軸タイトルを表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
