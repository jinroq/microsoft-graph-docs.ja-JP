---
title: educationAssignmentPointsGrade リソースの種類
description: 1つの割り当てがポイントグレードの種類に設定されている場合、各提出物には、"**成績**" プロパティに関連付けられたオブジェクトがあります。 これにより、educationAssignmentGrade からサブクラスが作成されます。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 166f6b5ce377441641cf12232c2194dff1184765
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340586"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

1つの割り当てがポイントグレードの種類に設定されている場合、各提出物には、"**成績**" プロパティに関連付けられたオブジェクトがあります。 これにより、 [educationAssignmentGrade](educationassignmentgrade.md)からサブクラスが作成され、このプロパティに who データが追加されます。 max 要素は、 **assignments**プロパティに格納されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|points|1 行|教師がこの送信オブジェクトを提供しているポイントの数。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
