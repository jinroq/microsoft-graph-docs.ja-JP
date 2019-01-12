---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953564"
---
# <a name="planneruser-resource-type"></a>plannerUser リソースの種類

**plannerUser** リソースは、[user](user.md) のプランナー リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plans を一覧表示する](../api/planneruser-list-plans.md) |[plannerPlan](plannerplan.md) コレクション| **plannerPlan** オブジェクト コレクションを取得します。|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。planenrUser の識別子|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。ユーザーと共有している [plannerPlans](plannerplan.md) を返します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
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
