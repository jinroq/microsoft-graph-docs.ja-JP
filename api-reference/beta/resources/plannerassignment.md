---
title: plan/assignment リソースの種類
description: '[ **plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。 この型は、オープンタイププランの割り当てで使用されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541361"
---
# <a name="plannerassignment-resource-type"></a>plan/assignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ **plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。 この型は、オープンタイププランの[割り当て](plannerassignments.md)で使用されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|タスクの割り当てを実行したユーザーの id。つまり、割り当てまたは。|
|assignedDateTime|DateTimeOffset|タスクが割り当てられた日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|タスクの担当者を注文するために使用されるヒント。 この形式は、[ここで](planner-order-hint-format.md)説明するように定義されています。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
