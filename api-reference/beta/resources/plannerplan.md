---
title: plannerPlan リソースの種類
description: '**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、グループが所有することができ、plannerTasks のコレクションが含まれています。 PlannerBuckets のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる詳細オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、プランナーを参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529552"
---
# <a name="plannerplan-resource-type"></a>plannerPlan リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、[グループ](group.md)が所有することができ、 [plannerTasks](plannertask.md)のコレクションが含まれています。 [PlannerBuckets](plannerbucket.md)のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる[詳細](plannerplandetails.md)オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、[プランナー](planner-overview.md)を参照してください。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|Get plannerPlan | [plannerPlan](plannerplan.md) |plannerPlan オブジェクトのプロパティとリレーションシップを読み取ります。|
|List buckets |[plannerBucket](plannerbucket.md) コレクション| plannerBucket オブジェクト コレクションを取得します。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |plannerPlan オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|文字列| 読み取り専用です。 計画の ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。|
|owner|String|計画を所有する[グループ](group.md)の ID です。 このフィールドを設定する前に、有効なグループが存在する必要があります。 設定すると後、は、このプロパティを更新できません。|
|タイトル|String|必須。計画のタイトル。|
|createdBy|[identitySet](identityset.md)|読み取り専用です。計画を作成したユーザー。|
|コンテキスト|[plannerPlanContextCollection](plannerplancontextcollection.md)| 読み取り専用です。 このプランが使用されている、追加のユーザー エクスペリエンスは、 [plannerPlanContext](plannerplancontext.md)のエントリとして表されます。|

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
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
