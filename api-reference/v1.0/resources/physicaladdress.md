---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f301947d6d277cd4fd51b7db035ef4f7134a5e65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035511"
---
# <a name="physicaladdress-resource-type"></a>physicalAddress リソースの種類

連絡先やイベントなどのリソースの番地を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
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
