---
title: プラン、Listitem リソースの種類
description: '**Plan**は、タスクのチェックリストの項目を表します。 タスクのチェックリストは、checklistItems オブジェクトによって表されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9bce6b0089f9e713e66e0354ce58d68cfd17fa7c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009077"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="fa226-104">プラン、Listitem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa226-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa226-105">**Plan**は、タスクのチェックリストの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="fa226-105">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="fa226-106">タスクのチェックリストは、 [checklistItems オブジェクト](plannerchecklistitems.md)によって表されます。</span><span class="sxs-lookup"><span data-stu-id="fa226-106">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="fa226-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa226-107">Properties</span></span>
| <span data-ttu-id="fa226-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa226-108">Property</span></span>     | <span data-ttu-id="fa226-109">型</span><span class="sxs-lookup"><span data-stu-id="fa226-109">Type</span></span>   |<span data-ttu-id="fa226-110">説明</span><span class="sxs-lookup"><span data-stu-id="fa226-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa226-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="fa226-111">isChecked</span></span>|<span data-ttu-id="fa226-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa226-112">Boolean</span></span>|<span data-ttu-id="fa226-113">値は`true` 、アイテムがチェックされ`false`ているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fa226-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="fa226-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fa226-114">lastModifiedBy</span></span>|[<span data-ttu-id="fa226-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa226-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="fa226-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fa226-116">Read-only.</span></span> <span data-ttu-id="fa226-117">これを最後に変更するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="fa226-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="fa226-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa226-118">lastModifiedDateTime</span></span>|<span data-ttu-id="fa226-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa226-119">DateTimeOffset</span></span>|<span data-ttu-id="fa226-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fa226-120">Read-only.</span></span> <span data-ttu-id="fa226-121">この時刻が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="fa226-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="fa226-122">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="fa226-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa226-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fa226-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fa226-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="fa226-124">orderHint</span></span>|<span data-ttu-id="fa226-125">String</span><span class="sxs-lookup"><span data-stu-id="fa226-125">String</span></span>|<span data-ttu-id="fa226-126">チェックリストの項目の相対的な順序を設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="fa226-126">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="fa226-127">この形式は、[ここで](planner-order-hint-format.md)説明するように定義されています。</span><span class="sxs-lookup"><span data-stu-id="fa226-127">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="fa226-128">title</span><span class="sxs-lookup"><span data-stu-id="fa226-128">title</span></span>|<span data-ttu-id="fa226-129">String</span><span class="sxs-lookup"><span data-stu-id="fa226-129">String</span></span>|<span data-ttu-id="fa226-130">チェックリストアイテムのタイトル</span><span class="sxs-lookup"><span data-stu-id="fa226-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa226-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa226-131">JSON representation</span></span>
<span data-ttu-id="fa226-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa226-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
