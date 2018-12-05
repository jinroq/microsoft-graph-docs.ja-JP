---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
ms.openlocfilehash: 819240be3eb9a088fde43390fbb1d1d4af1fd30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073075"
---
# <a name="physicaladdress-resource-type"></a>physicalAddress リソースの種類

連絡先やイベントなどのリソースの番地を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|type|String|アドレスの種類。 可能な値は、`unknown`、`home`、`business`、`other` です。|
|postOfficeBox|String|私書箱番号です。|
|city|String|市区町村。|
|countryOrRegion|String|国または地域。自由形式の文字列値です。例: 「米国」。|
|postalCode|String|郵便番号。|
|state|String|都道府県。|
|street|String|番地。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->