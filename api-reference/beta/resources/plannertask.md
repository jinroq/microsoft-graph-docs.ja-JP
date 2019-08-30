---
title: plannerTask のリソースの種類
description: '**plannerTask** リソースは、Office 365 の Planner のタスクを表します。Planner のタスクは plan に格納され、また、タスクは計画の中の bucket に割り当てることができます。各タスクオブジェクトには、タスクについてのより詳細な情報を保持するための details オブジェクトがあります。グループ、プラン、タスクの関係についての詳細は「概要」を参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9ced498b9bc56d8f21f96ede67d1a9a6501ddb21
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677177"
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
|activeChecklistItemCount|Int32|チェックリストの項目数。値が `false` である場合は、不完全な項目があることを示します。|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|タスクが適用されているカテゴリ。可能な値については、「[適用されるカテゴリ](plannerappliedcategories.md)」を参照してください。|
|assigneePriority|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|assignments|[plannerAssignments](plannerassignments.md)|タスクが割り当てられている一連の担当者。|
|bucketId|String|タスクが属しているバケット ID。 バケットは、タスクが存在している計画に含まれている必要があります。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。 |
|checklistItemCount|Int32|タスクに存在するチェックリストの項目の数です。|
|completedBy|[identitySet](identityset.md)|タスクを完了したユーザーの ID。|
|CompletedDateTime|DateTimeOffset|読み取り専用。タスクの `'percentComplete'` が `'100'` にセットされる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|conversationThreadId|String|タスク内の会話のスレッド ID。これは、グループ内に作成された会話スレッド オブジェクトの ID です。|
|createdBy|[identitySet](identityset.md)|タスクを作成したユーザーの ID。|
|createdDateTime|DateTimeOffset|読み取り専用。タスクが作成された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|タスクが期限切れになる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|hasDescription|Boolean|読み取り専用。タスクの details オブジェクトが保持する説明が空でない場合、値は `true` になり、そうでない場合は `false` になります。|
|id|String|読み取り専用。 タスクの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|orderHint|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|percentComplete|Int32|タスクの完了の割合。`100` に設定すると、タスクが完了したと見なされます。 |
|priority|Int32|タスクの優先度。 有効な値の範囲は`0` ~ `10` (包含) で、値が低い優先度 (`0`最も高い`10`優先度で、最も低い優先度) になります。  現在、Planner では`0`値`1`が`2` "緊急" `3` `4`として解釈され、" `5`重要`6` `7` " `8` `9` `10` 、、、、および "低" として解釈されます。  現時点では、Planner は`1` "緊急"、 `3` `5` "中" `9` 、"低" の値を設定します。|
|planId|String|タスクが属している計画 ID。|
|previewType|String|タスクに表示されるプレビューの種類を設定します。 可能な値は、`automatic`、`noPreview`、`checklist`、`description`、`reference` です。|
|referenceCount|Int32|タスクに上に存在している外部への参照の数。|
|startDateTime|DateTimeOffset|タスクが開始される日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|title|String|タスクのタイトル。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| 読み取り専用。Null 許容型。assignedTo 別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| 読み取り専用。Null 許容型。バケット別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|
|詳細|[plannerTaskDetails](plannertaskdetails.md)| 読み取り専用。Null 許容型。タスクに関する追加の詳細。|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| 読み取り専用。Null 許容型。進捗状態別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "priority": 1024,
  "planId": "String",
  "previewType": "String",
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
  "suppressions": []
}
-->
