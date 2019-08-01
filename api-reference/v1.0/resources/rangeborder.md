---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b5a12c05bed39363d8a8a01eef749f2e88b929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034931"
---
# <a name="rangeborder-resource-type"></a>RangeBorder リソースの種類

オブジェクトの輪郭を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[RangeBorder を取得する](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |rangeBorder オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |RangeBorder オブジェクトを更新します。 |
|[List](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md)コレクション |rangeBorder オブジェクトのコレクションを取得します。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|インデックスに基づいて border オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。|
|id|string|罫線の識別子を表します。 使用可能な値は`EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、、 `DiagonalUp`、です。 読み取り専用です。|
|sideIndex|string|罫線の特定の辺を表す定数値。 使用可能な値は`EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、、 `DiagonalUp`、です。 読み取り専用です。|
|style|string|罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。 使用可能な値は`None`、 `Continuous`、 `Dash` `DashDot` `DashDotDot` `Dot` `Double`、、、、、 `SlantDashDot`、です。|
|weight|string|範囲を取り囲む罫線の太さを指定します。 使用可能な値: `Hairline`、`Thin`、`Medium`、`Thick`。|

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
