---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88330f98b2d652d347aae703ec91fd4de8678c9d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576396"
---
# <a name="chartlegend-resource-type"></a>ChartLegend リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフに凡例を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartLegend](../api/chartlegend-get.md) | [WorkbookChartLegend](chartlegend.md) |chartLegend オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlegend-update.md) | [WorkbookChartLegend](chartlegend.md) |ChartLegend オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|overlay|boolean|グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。|
|position|文字列|グラフの凡例の位置を表します。 可能な値: `Top`、 `Bottom`、 `Left`、 `Right`、 `Corner`、 `Custom`。|
|visible|boolean|ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartLegendFormat](chartlegendformat.md)|グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。|

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
