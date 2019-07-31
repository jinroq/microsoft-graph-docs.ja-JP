---
title: プランユーザーリソースの種類
description: '**Plan ユーザー**リソースは、ユーザーの Planner リソースへのアクセスを提供します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2229020f00331e761eceeadf0739c84995e5bbdb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008993"
---
# <a name="planneruser-resource-type"></a>プランユーザーリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Plan ユーザー**リソースは、[ユーザー](user.md)の Planner リソースへのアクセスを提供します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| ユーザーに割り当てられている[プラン](plannertask.md)を取得します。|
|[お気に入りのプランを一覧表示する](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーによってお気に入りとしてマークされた[プラン](plannerplan.md)を取得します。|
|[リスト recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md) コレクション| ユーザーが最近閲覧した[プラン](plannerplan.md)を取得します。|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| プランの**ユーザー**オブジェクトを更新します。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用。 プランユーザーの識別子|
|お気に入りプランの参照|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| ユーザーがお気に入りとしてマークしたプランへの参照を含むコレクション。|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| 最近のプランをサポートするアプリで、ユーザーが最近表示したプランへの参照を含むコレクション。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。 Null 許容型。 ユーザーに割り当てられた担当者の[タスク](plannertask.md)を返します。|
|お気に入りのプラン|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 ユーザーがお気に入りとしてマークした[プラン](plannerplan.md)を返します。|
|recentPlans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 最近のプランをサポートするアプリで、ユーザーによって最近参照された[プラン](plannerplan.md)を返します。 |

## <a name="json-representation"></a>JSON 表記
リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
