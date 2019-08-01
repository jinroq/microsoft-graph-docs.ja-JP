---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6cfa08c15318fdaa58ac71e01a940b621b207f12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035673"
---
# <a name="outlookgeocoordinates-resource-type"></a>outlookGeoCoordinates リソースの種類

物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accuracy|double|緯度と経度の精度です。 一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。|
|altitude|double|場所の標高です。|
|altitudeAccuracy|double|標高の精度。|
|latitude|double|場所の緯度です。|
|longitude|double|場所の経度です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
