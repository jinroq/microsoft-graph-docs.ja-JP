---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: GeoCoordinates リソースは、ファイルに含まれているメタデータに基づいて、場所の地理的な座標と仰角を提供します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64b81bc2946658ffc8617662879bc6cb20e25047
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029310"
---
# <a name="geocoordinates-resource-type"></a>GeoCoordinates リソースの種類

**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>プロパティ

| プロパティ  | 型   | 説明
|:----------|:-------|:--------------------------------------------------------
| altitude  | 2 行分 | 省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。
| latitude  | 2 行分 | 省略可能。アイテムの緯度 (10 進数)。読み取り専用です。
| longitude | Double | 省略可能。アイテムの経度 (10 進数)。読み取り専用です。

## <a name="remarks"></a>注釈

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
