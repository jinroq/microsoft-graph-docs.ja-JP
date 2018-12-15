---
title: physicalOfficeAddress リソースの種類
description: 連絡先やイベントなどのリソースの会社の住所を表します。
ms.openlocfilehash: 472e4dfd03670f5fd4ff6b5c5c53342fff5c391a
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284099"
---
# <a name="physicalofficeaddress-resource-type"></a>physicalOfficeAddress リソースの種類

リソース、組織の連絡先などの会社の住所を表します。

## <a name="properties"></a>Properties

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|city|String|市区町村。|
|countryOrRegion|String|国または地域。自由形式の文字列値です。例: 「米国」。|
|officeLocation  | String | 組織の連絡先の数の建物や事務所などの場所を Office です。  |
|postalCode|String|郵便番号。|
|state|String|都道府県。|
|street|String|番地。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
