---
title: physicalOfficeAddress リソースの種類
description: 連絡先、イベントなどのリソースの勤務先住所を表します。
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573733"
---
# <a name="physicalofficeaddress-resource-type"></a>physicalOfficeAddress リソースの種類

組織の連絡先などのリソースの勤務先住所を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|city|String|市区町村。|
|countryOrRegion|String|国または地域。自由形式の文字列値です。例: 「米国」。|
|officeLocation  | String | 組織の連絡先の建物やオフィス番号などのオフィスの場所。  |
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
