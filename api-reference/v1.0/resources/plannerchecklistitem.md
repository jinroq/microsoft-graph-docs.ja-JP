---
title: plannerChecklistItem リソースの種類
description: '**PlannerChecklistItem**リソースは、タスクのチェックリストの項目を表します。 タスクのチェックリストは、checklistItems オブジェクトによって表されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 554391577fb0d48c2e0fd9fe265298e1dc1dd4fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941668"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="bfd82-104">plannerChecklistItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfd82-104">plannerChecklistItem resource type</span></span>


<span data-ttu-id="bfd82-p102">**PlannerChecklistItem**リソースはタスクのチェックリスト内の項目を表します。タスクのチェックリストは、[checklistItems オブジェクト](plannerchecklistitems.md)で表されます。</span><span class="sxs-lookup"><span data-stu-id="bfd82-p102">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="bfd82-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfd82-107">Properties</span></span>
| <span data-ttu-id="bfd82-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfd82-108">Property</span></span>     | <span data-ttu-id="bfd82-109">種類</span><span class="sxs-lookup"><span data-stu-id="bfd82-109">Type</span></span>   |<span data-ttu-id="bfd82-110">説明</span><span class="sxs-lookup"><span data-stu-id="bfd82-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfd82-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="bfd82-111">isChecked</span></span>|<span data-ttu-id="bfd82-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfd82-112">Boolean</span></span>|<span data-ttu-id="bfd82-113">項目がチェックされた場合は `true`、それ以外の場合は `false` です。</span><span class="sxs-lookup"><span data-stu-id="bfd82-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="bfd82-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bfd82-114">lastModifiedBy</span></span>|[<span data-ttu-id="bfd82-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="bfd82-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="bfd82-p103">読み取り専用です。これを最後に変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="bfd82-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="bfd82-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfd82-118">lastModifiedDateTime</span></span>|<span data-ttu-id="bfd82-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfd82-119">DateTimeOffset</span></span>|<span data-ttu-id="bfd82-p104">読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfd82-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfd82-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="bfd82-124">orderHint</span></span>|<span data-ttu-id="bfd82-125">String</span><span class="sxs-lookup"><span data-stu-id="bfd82-125">String</span></span>|<span data-ttu-id="bfd82-p105">チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="bfd82-p105">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="bfd82-128">タイトル</span><span class="sxs-lookup"><span data-stu-id="bfd82-128">title</span></span>|<span data-ttu-id="bfd82-129">String</span><span class="sxs-lookup"><span data-stu-id="bfd82-129">String</span></span>|<span data-ttu-id="bfd82-130">チェックリスト項目のタイトル</span><span class="sxs-lookup"><span data-stu-id="bfd82-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfd82-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfd82-131">JSON representation</span></span>
<span data-ttu-id="bfd82-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bfd82-132">Here is a JSON representation of the resource.</span></span>

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
