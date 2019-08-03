---
title: リソースの種類 (最高)
description: の品質 (最高)
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fd8ad7aa7d0a19fe1774e18bba5d59af52140
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173308"
---
# <a name="rubricquality-resource-type"></a>リソースの種類 (最高)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

高品質 (最高) EducationRubric については、「 [](educationrubric.md) 」を参照し** てください**。 **

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|criteria|の[条件](rubriccriterion.md)のコレクション|この検索基準のコレクションです。|
|description|[itemBody](itembody.md)|このテンプレートの説明。|
|displayName|String|この名前を指定します。|
|qualityId|String|このリソースの ID。|
|weight|1 行|存在する場合は、この品質の数値ウェイトを指定します。  重みは100まで追加する必要があります。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->