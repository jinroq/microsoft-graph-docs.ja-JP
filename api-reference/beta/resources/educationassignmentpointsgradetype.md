---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments.grading**プロパティと共に使用します。 これは、educationAssignmentGradeType のサブクラスです。'
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073487"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**Assignments.grading**プロパティと共に使用します。 これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。

これは、割り当てが焼き付けるし、この作業項目に各受講者が達成できるポイントの最大数を格納することを示します。 割り当てに設定すると、送信するたびに、各受講者用のポイントを格納するために関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが表示されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
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