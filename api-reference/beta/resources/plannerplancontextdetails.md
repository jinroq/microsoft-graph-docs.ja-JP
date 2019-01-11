---
title: plannerPlanContextDetails リソースの種類
description: '**PlannerPlanContextDetails**リソースには、plannerPlanContext に関する追加情報が含まれています。'
localization_priority: Normal
ms.openlocfilehash: ec35a83e5ba2d2648c512f31f838f19bd3ec2e02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812055"
---
# <a name="plannerplancontextdetails-resource-type"></a>plannerPlanContextDetails リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerPlanContextDetails**リソースには、 [plannerPlanContext](plannerplancontext.md)に関する追加情報が含まれています。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
