---
title: アイコン リソースの種類
description: セルのアイコンを表します。
localization_priority: Normal
ms.openlocfilehash: 833fa4cb4061a96b01077c3adeb7dcaed49e0a02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567810"
---
# <a name="icon-resource-type"></a>アイコン リソースの種類

セルのアイコンを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[アイコンを取得する](../api/icon-get.md) | [Icon](icon.md) |アイコン オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/icon-update.md) | [Icon](icon.md)  |アイコン オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|index|int|指定したセット内のアイコンのインデックスを表します。|
|set|string|アイコンがその一部であるセットを表します。 使用可能な値は`Invalid`次`ThreeArrows`の`ThreeArrowsGray`とおり`ThreeFlags`です`ThreeTrafficLights1`。 `ThreeTrafficLights2`、 `ThreeSigns` `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveQuarters`、、、、、、、、、、、、 `ThreeStars` `FiveArrows` `FiveArrowsGray` `FiveRating`, `ThreeTriangles`, `FiveBoxes`.|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
