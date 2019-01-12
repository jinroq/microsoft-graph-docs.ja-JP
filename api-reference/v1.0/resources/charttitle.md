---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトル オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f6c843e24839b51da67bda5ed3484a32c868ae54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986916"
---
# <a name="charttitle-resource-type"></a>ChartTitle リソースの種類

グラフのグラフ タイトル オブジェクトを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartTitle](../api/charttitle-get.md) | [WorkbookChartTitle](charttitle.md) |chartTitle オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/charttitle-update.md) | [WorkbookChartTitle](charttitle.md)    |ChartTitle オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|overlay|ブール値|グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。|
|text|文字列|グラフのタイトルのテキストを表します。|
|visible|ブール値|ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartTitleFormat](charttitleformat.md)|グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
