---
title: plannerPlanContextDetails リソースの種類
description: '**PlannerPlanContextDetails**リソースには、plannerPlanContext に関する追加情報が含まれています。'
ms.openlocfilehash: 44c1099c1155372a23029cd0cc6a4decd68c5bc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067387"
---
# <a name="plannerplancontextdetails-resource-type"></a>plannerPlanContextDetails リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerPlanContextDetails**リソースには、 [plannerPlanContext](plannerplancontext.md)に関する追加情報が含まれています。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|url|String|関連付けられた[plannerPlanContext](plannerplancontext.md)によって表されるユーザー エクスペリエンスの URL です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
