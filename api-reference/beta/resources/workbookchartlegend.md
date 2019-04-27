---
title: workbookChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e9c032966f62ac48e178aa6625b3f9891d2518a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348890"
---
# <a name="workbookchartlegend-resource-type"></a>workbookChartLegend リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフに凡例を表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookChartLegend を取得する](../api/chartlegend-get.md) | [workbookChartLegend](workbookchartlegend.md) |chartLegend オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlegend-update.md) | [workbookChartLegend](workbookchartlegend.md) |ChartLegend オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|overlay|ブール値|グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。|
|position|string|グラフの凡例の位置を表します。 使用可能な値は`Top`、 `Bottom`、 `Left` `Right` `Corner`、、、 `Custom`、です。|
|visible|ブール値|ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[workbookChartLegendFormat](workbookchartlegendformat.md)|塗りつぶしとフォントの書式設定を含む、グラフの凡例の書式設定を表します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
