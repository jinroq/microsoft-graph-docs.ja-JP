---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b95bc8c23ea71abb0d2c3f54e218d425e3d188ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880347"
---
# <a name="chartgridlines-resource-type"></a>ChartGridlines リソースの種類

グラフの軸の目盛線または補助目盛線を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartGridlines](../api/chartgridlines-get.md) | [WorkbookChartGridlines](chartgridlines.md) |chartGridlines オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartgridlines-update.md) | [WorkbookChartGridlines](chartgridlines.md)    |ChartGridlines オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|visible|ブール値|軸の目盛線を表示するか非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartGridlinesFormat](chartgridlinesformat.md)|グラフの目盛線の書式設定を表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
