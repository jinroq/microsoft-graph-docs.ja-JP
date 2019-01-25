---
title: educationAssignmentPointsGrade リソースの種類
description: ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。 これから educationAssignmentGrade、サブクラスを作成します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523737"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。 これは、 [educationAssignmentGrade](educationassignmentgrade.md)データが追加されます、ユーザーにこのプロパティをからサブクラスを作成します。 最大のポイントは、 **assignments.grading**プロパティに格納されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|points|単精度浮動小数点型 (Single)|先生をポイント数では、この送信オブジェクト、といいます。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
