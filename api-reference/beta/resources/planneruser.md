---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526880"
---
# <a name="planneruser-resource-type"></a>plannerUser リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerUser**リソースでは、[ユーザー](user.md)の計画のリソースへのアクセスを提供します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| ユーザーに割り当てられている[plannerTasks](plannertask.md)を取得します。|
|[リスト favoritePlans](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーがお気に入りとしてマークされている[plannerPlans](plannerplan.md)を取得します。|
|[リスト recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーが最近表示した[plannerPlans](plannerplan.md)を取得します。|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| **PlannerUser**オブジェクトを更新します。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 PlannerUser の識別子|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| ユーザーは、お気に入りとしてマークする計画への参照を格納するコレクション。|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| 最近の計画をサポートするアプリケーションでユーザーが最近表示された計画への参照を格納するコレクション。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。|
|favoritePlans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 ユーザーは、お気に入りとしてマークされている[plannerPlans](plannerplan.md)を返します。|
|recentPlans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 最近の計画をサポートするアプリケーションでユーザーが最近表示した[plannerPlans](plannerplan.md)を返します。 |

## <a name="json-representation"></a>JSON 表記
リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
