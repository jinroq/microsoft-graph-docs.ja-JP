---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
ms.openlocfilehash: 9de60c218f6fc54ed2be12b2987126195e5eb140
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068643"
---
# <a name="outlookgeocoordinates-resource-type"></a>outlookGeoCoordinates リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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