---
title: modifiedProperty リソースの種類
description: ターゲットシステムで実行された変更について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcf55dfc83414b5a516bac6cbeefa3358323b5fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966704"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ターゲットシステムで実行された変更について説明します。 

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|変更されたプロパティの名前。|
|newValue|文字列型 (String)|新しいプロパティ値。|
|oldValue|String|Old プロパティの値。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
