---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820805"
---
# <a name="planneruser-resource-type"></a>plannerUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerUser**リソースでは、[ユーザー](user.md)の計画のリソースへのアクセスを提供します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| ユーザーに割り当てられている[plannerTasks](plannertask.md)を取得します。|
|[リスト favoritePlans](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーがお気に入りとしてマークされている[plannerPlans](plannerplan.md)を取得します。|
|[リスト recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーが最近表示した[plannerPlans](plannerplan.md)を取得します。|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| **PlannerUser**オブジェクトを更新します。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。 PlannerUser の識別子|
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
