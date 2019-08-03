---
title: のリソースの種類
description: 1レベルののレベル
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dd8e67cbf4ba8994e03d683665928f9e62608d8e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173336"
---
# <a name="rubriclevel-resource-type"></a>のリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

1レベルの単位。 EducationRubric については、「 [](educationrubric.md) 」を参照し** てください**。 **

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|このフォルダーの説明。|
|displayName|String|この名前を指定します。|
|変化|[educationAssignmentGradeType](educationassignmentgradetype.md)|これが非ポイントの場合は Null になります。[educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md)の場合は、この点を参照してください。|
|levelId|String|このリソースの ID。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->