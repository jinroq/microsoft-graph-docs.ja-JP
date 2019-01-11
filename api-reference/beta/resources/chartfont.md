---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
ms.openlocfilehash: 0df14f98993c33b6b3eb3c0b2ea9fbdf211a8124
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824165"
---
# <a name="chartfont-resource-type"></a>ChartFont リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartFont](../api/chartfont-get.md) | [ChartFont](chartfont.md) |chartFont オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartfont-update.md) | [ChartFont](chartfont.md)   |ChartFont オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|bold|ブール値|フォントの太字の状態を表します。|
|color|文字列|テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。|
|italic|ブール値|フォントの斜体の状態を表します。|
|name|文字列|フォント名 (例: "Calibri")|
|size|double|フォント サイズ (例: 11)|
|underline|文字列|フォントに適用する下線の種類。可能な値は、`None`、`Single` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
