---
title: workbookChartTitle リソースの種類
description: グラフのグラフ タイトルのオブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8c102ea62b29cba017793dcaf135853121fc4bd4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007152"
---
# <a name="workbookcharttitle-resource-type"></a>workbookChartTitle リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのグラフ タイトルのオブジェクトを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorkbookChartTitle を取得する](../api/charttitle-get.md) | [workbookChartTitle](workbookcharttitle.md) |chartTitle オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/charttitle-update.md) | [workbookChartTitle](workbookcharttitle.md)    |ChartTitle オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|overlay|ブール値|グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。|
|text|string|グラフのタイトルのテキストを表します。|
|visible|ブール値|ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[workbookChartTitleFormat](workbookcharttitleformat.md)|塗りつぶしとフォントの書式設定を含む、グラフタイトルの書式設定を表します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
