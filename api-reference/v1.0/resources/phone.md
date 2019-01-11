---
title: 電話リソースの種類
description: 電話番号を表します。
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805062"
---
# <a name="phone-resource-type"></a>電話リソースの種類

電話番号を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|number|文字列|電話番号。|
|種類|phoneType|電話番号の種類。 可能な値: `home`、 `business`、 `mobile`、 `other`、 `assistant`、 `homeFax`、 `businessFax`、 `otherFax`、 `pager`、 `radio`。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
