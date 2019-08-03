---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments**プロパティと組み合わせて使用します。 これは、educationAssignmentGradeType のサブクラスです。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef866debcf2c70862aae30048f68bd026c4e5250
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172797"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Assignments**プロパティと組み合わせて使用します。 これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。

これは、割り当てが採点され、各学生がこの作業項目に対して達成できる最大ポイント数を格納することを示します。 割り当てに対してこのプロパティを設定すると、各学生のポイントの保存用に、各送信に関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが取得されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|maxPoints|1 行| この割り当てで可能な最大ポイント。  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
