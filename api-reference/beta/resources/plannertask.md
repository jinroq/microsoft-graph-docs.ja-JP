---
title: plannerTask のリソースの種類
description: '**plannerTask** リソースは、Office 365 の Planner のタスクを表します。Planner のタスクは plan に格納され、また、タスクは計画の中の bucket に割り当てることができます。各タスクオブジェクトには、タスクについてのより詳細な情報を保持するための details オブジェクトがあります。グループ、プラン、タスクの関係についての詳細は「概要」を参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2313b31e0a962f27fa728af8c8953b646210397a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511213"
---
# <a name="plannertask-resource-type"></a>plannerTask のリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerTask** リソースは、Office 365 の Planner のタスクを表します。Planner のタスクは [plan](plannerplan.md) に格納され、また、タスクは計画の中の [bucket](plannerbucket.md) に割り当てることができます。各タスクオブジェクトには、タスクについてのより詳細な情報を保持するための [details](plannertaskdetails.md) オブジェクトがあります。グループ、プラン、タスクの関係についての詳細は「[概要](planner-overview.md)」を参照してください。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerTask](../api/plannertask-get.md) | [plannerTask](plannertask.md) |**plannerTask** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannertask-update.md) | [plannerTask](plannertask.md) |**plannerTask** オブジェクトを更新します。 |
|[Delete](../api/plannertask-delete.md) | なし |**plannerTask** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|チェックリストの項目数で、値が「false」である場合は、不完全な項目があることを示します。|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|タスクが適用されているカテゴリ。可能な値については、「[適用されるカテゴリ](plannerappliedcategories.md)」を参照してください。|
|assigneePriority|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|assignments|[plannerAssignments](plannerassignments.md)|タスクが割り当てられている一連の担当者。|
|bucketId|String|バケット ID は、タスクが属する。 バケットは、タスクが含まれるプランにする必要があります。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。 |
|checklistItemCount|Int32|タスクに存在するチェックリストの項目の数です。|
|completedBy|[identitySet](identityset.md)|タスクを完了したユーザーの ID。|
|CompletedDateTime|DateTimeOffset|読み取り専用。タスクの `'percentComplete'` が `'100'` にセットされる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|conversationThreadId|文字列|タスク内の会話のスレッド ID。これは、グループ内に作成された会話スレッド オブジェクトの ID です。|
|createdBy|[identitySet](identityset.md)|タスクを作成したユーザーの ID。|
|createdDateTime|DateTimeOffset|読み取り専用。タスクが作成された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|タスクが期限切れになる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|hasDescription|Boolean|読み取り専用。タスクの details オブジェクトが保持する説明が空でない場合、値は `true` になり、そうでない場合は `false` になります。|
|id|String|読み取り専用です。 タスクの ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。|
|orderHint|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|percentComplete|Int32|タスクの完了の割合。`100` に設定すると、タスクが完了したと見なされます。 |
|planId|String|タスクが属している計画 ID。|
|previewType|string|タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。|
|referenceCount|Int32|タスクに上に存在している外部への参照の数。|
|startDateTime|DateTimeOffset|タスクが開始される日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|タイトル|String|タスクのタイトル。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| 読み取り専用。Null 許容型。assignedTo 別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| 読み取り専用。Null 許容型。バケット別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|
|詳細説明|[plannerTaskDetails](plannertaskdetails.md)| 読み取り専用。Null 許容型。タスクに関する追加の詳細。|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| 読み取り専用。Null 許容型。進捗状態別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "string",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertask.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
