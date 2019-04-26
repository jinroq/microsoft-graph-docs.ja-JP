---
title: plan/assignment リソースの種類
description: '[ **plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。 この型は、オープンタイププランの割り当てで使用されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fddb3214417fc1320b6218b4e9fd0266b176e26a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344615"
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
  "suppressions": []
}
-->
