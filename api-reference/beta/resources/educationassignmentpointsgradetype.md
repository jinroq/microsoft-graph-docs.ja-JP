---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments.grading**プロパティと共に使用します。 これは、educationAssignmentGradeType のサブクラスです。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: b603ccec0ddd5be5003353a5062e51554cb61c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952665"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**Assignments.grading**プロパティと共に使用します。 これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。

これは、割り当てが焼き付けるし、この作業項目に各受講者が達成できるポイントの最大数を格納することを示します。 割り当てに設定すると、送信するたびに、各受講者用のポイントを格納するために関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが表示されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|maxPoints|単精度浮動小数点型 (Single)| 最大は、この割り当ての可能性を指しています。  |

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
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
