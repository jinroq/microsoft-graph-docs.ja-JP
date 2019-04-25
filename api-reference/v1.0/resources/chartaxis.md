---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88066c356306a619ee620a13eefb6592d7b5f100
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569243"
---
# <a name="chartaxis-resource-type"></a>ChartAxis リソースの種類

グラフの 1 つの軸を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis-get.md) | [WorkbookChartAxis](chartaxis.md) |chartAxis オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartaxis-update.md) | [WorkbookChartAxis](chartaxis.md)   |ChartAxis オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| id       |string   | 一意の識別子。 読み取り専用。|
|majorUnit|Json|2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。|
|maximum|Json|数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minimum|Json|数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minorUnit|Json|2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartAxisFormat](chartaxisformat.md)|グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。|
|majorGridlines|[WorkbookChartGridlines](chartgridlines.md)|指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|minorGridlines|[WorkbookChartGridlines](chartgridlines.md)|指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|title|[WorkbookChartAxisTitle](chartaxistitle.md)|軸タイトルを表します。 値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
