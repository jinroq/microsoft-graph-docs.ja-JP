---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている plannerPlan への参照を入力します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509162"
---
# <a name="plannerrecentplanreference-resource-type"></a>plannerRecentPlanReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている[plannerPlan](plannerplan.md)への参照を入力します。 ユーザーの**plannerRecentPlanReferences**は、アプリケーションによって明示的に維持されます。 ユーザー最後を表示した場合の計画、および更新プログラム**plannerRecentPlanReference**のエントリに応じて、計画の最新の機能を実装する任意のアプリケーションを記録します。
アプリケーションでは、 **plannerRecentPlanReference**のエントリが削除する、ユーザーがアクセスできる不要になった、または別のタイトルで更新された**plannerPlans**を参照できるように注意してください。
アプリは不一致がある場合にユーザーに通知し、エントリを常に最新の状態に保つことをお勧めします。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|日付と時刻計画が、ユーザーが最後に表示します。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|planTitle|String|時にプランのタイトル ユーザーに表示します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
