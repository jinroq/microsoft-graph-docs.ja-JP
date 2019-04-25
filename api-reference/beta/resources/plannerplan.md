---
title: plan リソースの種類を計画する
description: プラン**** リソースは、Office 365 のプランを表します。 プランは、グループが所有することができ、プランのタスクのコレクションが含まれています。 また、プランのコレクションを持つこともできます。 各プランオブジェクトには details オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、プラン、およびタスク間の関係の詳細については、「Planner」を参照してください。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578870"
---
# <a name="plannerplan-resource-type"></a>plan リソースの種類を計画する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プラン**** リソースは、Office 365 のプランを表します。 プランは、[グループ](group.md)が所有することができ、プランの[タスク](plannertask.md)のコレクションが含まれています。 また、[プラン](plannerbucket.md)のコレクションを持つこともできます。 各プランオブジェクトには[details](plannerplandetails.md)オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、プラン、およびタスク間の関係の詳細については、「 [Planner](planner-overview.md)」を参照してください。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |**plan**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[バケットをリストする](../api/plannerplan-list-buckets.md) |[プラン | バケット](plannerbucket.md)コレクション| **プラン**を取得するオブジェクトコレクション。|
|[タスクを一覧表示する](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) コレクション| プランを取得する**タスク**オブジェクトコレクション。|
|[更新する](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |**plan**オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String| 読み取り専用。 プランの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|owner|String|プランを所有する[グループ](group.md)の ID。 このフィールドを設定するためには、有効なグループが存在していなければなりません。 設定された後は、このプロパティは更新できません。|
|title|String|必須。 計画のタイトル。|
|createdBy|[identitySet](identityset.md)|読み取り専用。 プランを作成したユーザー。|
|状況|[plannerPlanContextCollection](plannerplancontextcollection.md)| 読み取り専用。 このプランが使用される追加のユーザーエクスペリエンス。このプランは、[コンテキスト](plannerplancontext.md)エントリをプランとして表現します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[プラン | バケット](plannerbucket.md)コレクション| 読み取り専用。Null 許容型。計画に含まれるバケットのコレクション。|
|details|[plannerPlanDetails](plannerplandetails.md)| 読み取り専用。 Null 許容型。 計画に関する追加の詳細。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用。 Null 許容型。 計画に含まれるタスクのコレクション。|

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
