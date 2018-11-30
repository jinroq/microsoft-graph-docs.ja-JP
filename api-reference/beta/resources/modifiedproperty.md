---
title: modifiedProperty リソースの種類
description: Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069103"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty リソースの種類
Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|変更されたターゲットの属性のプロパティ名を示します。|
|newValue|文字列型 (String)|これらの更新された値を示します。|
|oldValue|文字列型 (String)|(更新) する前にプロパティの以前の値を示します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->