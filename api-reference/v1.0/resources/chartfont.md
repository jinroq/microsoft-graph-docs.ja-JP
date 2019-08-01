---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9241691296b93eb21e19e10b81f36e692fea0692
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032999"
---
# <a name="chartfont-resource-type"></a>ChartFont リソースの種類

このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartFont](../api/chartfont-get.md) | [WorkbookChartFont](chartfont.md) |chartFont オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartfont-update.md) | [WorkbookChartFont](chartfont.md)   |ChartFont オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bold|ブール値|フォントの太字の状態を表します。|
|color|string|テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。|
|italic|ブール値|フォントの斜体の状態を表します。|
|name|string|フォント名 (例: "Calibri")|
|size|double|フォント サイズ (例: 11)|
|underline|文字列|フォントに適用する下線の種類。 使用可能な値は`None`、 `Single`、です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
