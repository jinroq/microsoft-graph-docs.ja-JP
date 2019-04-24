---
title: modifiedProperty リソースの種類
description: 変更された Azure AD のリソースについて、古い値と新しい値を持つすべての変更されたプロパティを示します。
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506237"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty リソースの種類
変更された Azure AD のリソースについて、古い値と新しい値を持つすべての変更されたプロパティを示します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|変更されたターゲット属性のプロパティ名を示します。|
|newValue|文字列型 (String)|これらの更新された値を示します。|
|oldValue|String|プロパティの以前の値 (更新前) を示します。|

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
