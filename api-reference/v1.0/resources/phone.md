---
title: 電話リソースの種類
description: 電話番号を表します。
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023191"
---
# <a name="phone-resource-type"></a>電話リソースの種類

電話番号を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|数値|文字列|電話番号。|
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
