---
title: plannerChecklistItem リソースの種類
description: '**PlannerChecklistItem**リソースは、タスクのチェックリストの項目を表します。 タスクのチェックリストは、checklistItems オブジェクトによって表されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fef935dfc2683e04b0ccec9ab5a7885927f8a13c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962983"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="78859-104">plannerChecklistItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78859-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="78859-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78859-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78859-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78859-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78859-p103">**PlannerChecklistItem**リソースはタスクのチェックリスト内の項目を表します。タスクのチェックリストは、[checklistItems オブジェクト](plannerchecklistitems.md)で表されます。</span><span class="sxs-lookup"><span data-stu-id="78859-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="78859-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78859-109">Properties</span></span>
| <span data-ttu-id="78859-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78859-110">Property</span></span>     | <span data-ttu-id="78859-111">型</span><span class="sxs-lookup"><span data-stu-id="78859-111">Type</span></span>   |<span data-ttu-id="78859-112">説明</span><span class="sxs-lookup"><span data-stu-id="78859-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78859-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="78859-113">isChecked</span></span>|<span data-ttu-id="78859-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="78859-114">Boolean</span></span>|<span data-ttu-id="78859-115">項目がチェックされた場合は `true`、それ以外の場合は `false` です。</span><span class="sxs-lookup"><span data-stu-id="78859-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="78859-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="78859-116">lastModifiedBy</span></span>|[<span data-ttu-id="78859-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="78859-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="78859-p104">読み取り専用です。これを最後に変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="78859-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="78859-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78859-120">lastModifiedDateTime</span></span>|<span data-ttu-id="78859-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78859-121">DateTimeOffset</span></span>|<span data-ttu-id="78859-p105">読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78859-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78859-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="78859-126">orderHint</span></span>|<span data-ttu-id="78859-127">String</span><span class="sxs-lookup"><span data-stu-id="78859-127">String</span></span>|<span data-ttu-id="78859-p106">チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="78859-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="78859-130">タイトル</span><span class="sxs-lookup"><span data-stu-id="78859-130">title</span></span>|<span data-ttu-id="78859-131">String</span><span class="sxs-lookup"><span data-stu-id="78859-131">String</span></span>|<span data-ttu-id="78859-132">チェックリスト項目のタイトル</span><span class="sxs-lookup"><span data-stu-id="78859-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78859-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78859-133">JSON representation</span></span>
<span data-ttu-id="78859-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78859-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
