---
title: workbookRangeFill リソースの種類
description: Range オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eea7337fa4aefb1bde607740b9a2fc78264dae91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348881"
---
# <a name="workbookrangefill-resource-type"></a>workbookRangeFill リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Range オブジェクトの背景を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookRangeFill を取得する](../api/rangefill-get.md) | [workbookRangeFill](workbookrangefill.md) |rangeFill オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangefill-update.md) | [workbookRangeFill](workbookrangefill.md)   |RangeFill オブジェクトを更新します。 |
|[Clear](../api/rangefill-clear.md)|なし|範囲の背景をリセットします。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|color|string|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
