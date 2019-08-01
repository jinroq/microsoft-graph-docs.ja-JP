---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dcd601f27f0e6869a229fcbe7df195cd65481fd4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032993"
---
# <a name="chartlegend-resource-type"></a>ChartLegend リソースの種類

グラフに凡例を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartLegend](../api/chartlegend-get.md) | [WorkbookChartLegend](chartlegend.md) |chartLegend オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlegend-update.md) | [WorkbookChartLegend](chartlegend.md) |ChartLegend オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|overlay|ブール値|グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。|
|position|string|グラフの凡例の位置を表します。 使用可能な値: `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。|
|visible|ブール値|ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartLegendFormat](chartlegendformat.md)|塗りつぶしとフォントの書式設定を含む、グラフの凡例の書式設定を表します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
