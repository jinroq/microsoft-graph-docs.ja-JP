---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4b20078b7d4d0cabf4c16e212fd3e9264cad1650
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830801"
---
# <a name="rangeborder-resource-type"></a>RangeBorder リソースの種類

オブジェクトの輪郭を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[RangeBorder を取得する](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |rangeBorder オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |RangeBorder オブジェクトを更新します。 |
|[List](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md)コレクション |rangeBorder オブジェクトのコレクションを取得します。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。|
|ID|文字列|枠線の識別子を表します。 可能な値: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft`、 `EdgeRight`、 `InsideVertical`、 `InsideHorizontal`、 `DiagonalDown`、 `DiagonalUp`。 読み取り専用です。|
|sideIndex|文字列|罫線の特定の側面を示す定数値です。 可能な値: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft`、 `EdgeRight`、 `InsideVertical`、 `InsideHorizontal`、 `DiagonalDown`、 `DiagonalUp`。 読み取り専用です。|
|style|文字列|境界線の線のスタイルを指定する線のスタイルの定数の 1 つです。 可能な値: `None`、 `Continuous`、 `Dash`、 `DashDot`、 `DashDotDot`、 `Dot`、 `Double`、 `SlantDashDot`。|
|weight|文字列|範囲周辺の罫線の太さを指定します。 可能な値: `Hairline`、 `Thin`、 `Medium`、 `Thick`。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
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
