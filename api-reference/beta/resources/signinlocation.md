---
title: signInLocation リソースの種類
description: 市、州、および記号の発生場所からの国を提供します。
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070574"
---
# <a name="signinlocation-resource-type"></a>signInLocation リソースの種類
市、州、および記号の発生場所からの国を提供します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|city|String|サインインが発生した場所の市区町村を提供します。 これは、サインインの活動からの緯度/経度情報を使用して計算されます。|
|countryOrRegion|String|サインインが発生した場所 (2 文字のコード) の国コード情報を提供します。  これは、サインインの活動からの緯度/経度情報を使用して計算されます。|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|緯度、経度および高度の記号には、発生した場所を提供します。|
|state|String|サインインが発生した場所の状態を提供します。 これは、サインインの活動からの緯度/経度情報を使用して計算されます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->