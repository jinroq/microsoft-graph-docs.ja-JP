---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8404a45ea7c56bbbb318994daa55229706d700a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960239"
---
# <a name="rangeborder-resource-type"></a>RangeBorder リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

オブジェクトの輪郭を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[RangeBorder を取得する](../api/rangeborder-get.md) | [RangeBorder](rangeborder.md) |rangeBorder オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangeborder-update.md) | [RangeBorder](rangeborder.md) |RangeBorder オブジェクトを更新します。 |
|[List](../api/rangeborder-list.md) | [RangeBorder](rangeborder.md) コレクション |rangeBorder オブジェクトのコレクションを取得します。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[RangeBorder](rangeborder.md)|オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。|
|ID|文字列|罫線の識別子を表します。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。|
|sideIndex|文字列|罫線の特定の辺を表す定数値。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。|
|style|文字列|罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。|
|weight|文字列|範囲を取り囲む罫線の太さを指定します。可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
