---
title: networkLocationDetail リソースの種類
description: ネットワーク上の場所に関連付けられている詳細情報を示します。 .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070961"
---
# <a name="networklocationdetail-resource-type"></a>networkLocationDetail リソースの種類
ネットワーク上の場所に関連付けられている詳細情報を示します。 .



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|networkType|String|ネットワークの種類を提供します。 使用可能な値は、 `intranet`、 `extranet`、`namedNetwork`と`trusted`。|
|ネットワーク名リソース|String|ネットワークの名前です。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->