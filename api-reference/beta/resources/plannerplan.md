---
title: plannerPlan リソースの種類
description: '**plannerPlan** リソースは、Office 365 での計画を表します。 計画は group によって所有され、plannerTasks のコレクションが含まれています。 plannerBuckets のコレクションを含む場合もあります。 各プランオブジェクトには details オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、計画、タスク間のリレーションシップの詳細については、「Planner」を参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5da918e3ba0e8087d4572799168fa1132e0ce5e7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344467"
---
# <a name="plannerplan-resource-type"></a>plannerPlan リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerPlan** リソースは、Office 365 での計画を表します。 計画は [group](group.md) によって所有され、[plannerTasks](plannertask.md) のコレクションが含まれています。 [plannerBuckets](plannerbucket.md) のコレクションを含む場合もあります。 各プランオブジェクトには[details](plannerplandetails.md)オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner-overview.md)」を参照してください。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[List buckets](../api/plannerplan-list-buckets.md) |[plannerBucket](plannerbucket.md) コレクション| **plannerBucket** オブジェクト コレクションを取得します。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |**plannerPlan** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String| 読み取り専用です。 計画の ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|owner|String|計画を所有している [Group](group.md) の ID。 このフィールドを設定するためには、有効なグループが存在していなければなりません。 設定すると、このプロパティを更新することはできません。|
|title|String|必須。 計画のタイトル。|
|createdBy|[identitySet](identityset.md)|読み取り専用です。 計画を作成したユーザー。|
|状況|[plannerPlanContextCollection](plannerplancontextcollection.md)| 読み取り専用です。 このプランが使用される追加のユーザーエクスペリエンス。このプランは、[コンテキスト](plannerplancontext.md)エントリをプランとして表現します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) コレクション| 読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。|
|詳細|[plannerPlanDetails](plannerplandetails.md)| 読み取り専用です。 Null 許容型。 計画に関する追加の詳細。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。 Null 許容型。 計画に含まれるタスクのコレクション。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
