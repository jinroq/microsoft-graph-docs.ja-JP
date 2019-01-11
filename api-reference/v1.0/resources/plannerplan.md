---
title: plannerPlan リソースの種類
description: '**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、グループが所有することができ、plannerTasks のコレクションが含まれています。 PlannerBuckets のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる詳細オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、プランナーを参照してください。'
localization_priority: Priority
ms.openlocfilehash: cfcc94fab067cc76bb530edbdb8477183ebf3531
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873011"
---
# <a name="plannerplan-resource-type"></a>plannerPlan リソースの種類

**plannerPlan** リソースは、Office 365 での計画を表します。計画は [group](group.md) によって所有され、[plannerTasks](plannertask.md) のコレクションが含まれています。[plannerBuckets](plannerbucket.md) のコレクションを含む場合もあります。各計画オブジェクトには [details](plannerplandetails.md) オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner-overview.md)」を参照してください。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[List buckets](../api/plannerplan-list-buckets.md) |[plannerBucket](plannerbucket.md) コレクション| **plannerBucket** オブジェクト コレクションを取得します。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |**plannerPlan** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String| 読み取り専用です。 計画の ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。|
|owner|String|計画を所有する[グループ](group.md)の ID です。 このフィールドを設定する前に、有効なグループが存在する必要があります。 設定すると後、は、このプロパティを更新できません。|
|タイトル|String|必須。計画のタイトル。|
|createdBy|[identitySet](identityset.md)|読み取り専用です。計画を作成したユーザー。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) コレクション| 読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。|
|詳細|[plannerPlanDetails](plannerplandetails.md)| 読み取り専用です。Null 許容型。計画に関する追加の詳細。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
