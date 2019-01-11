---
title: modifiedProperty リソースの種類
description: Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844456"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty リソースの種類
Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します



## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
