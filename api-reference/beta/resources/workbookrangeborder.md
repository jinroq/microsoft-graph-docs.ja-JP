---
title: workbookRangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6457380b3027df8d99b97219ac2ae43e99e0620a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964038"
---
# <a name="workbookrangeborder-resource-type"></a>workbookRangeBorder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オブジェクトの輪郭を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorkbookRangeBorder を取得する](../api/rangeborder-get.md) | [workbookRangeBorder](workbookrangeborder.md) |rangeBorder オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangeborder-update.md) | [workbookRangeBorder](workbookrangeborder.md) |RangeBorder オブジェクトを更新します。 |
|[List](../api/rangeborder-list.md) | [workbookRangeBorder](workbookrangeborder.md)コレクション |rangeBorder オブジェクトのコレクションを取得します。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[workbookRangeBorder](workbookrangeborder.md)|インデックスに基づいて border オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。|
|id|string|罫線の識別子を表します。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。|
|sideIndex|string|罫線の特定の辺を表す定数値。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。|
|style|string|罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。|
|weight|string|範囲を取り囲む罫線の太さを指定します。可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
