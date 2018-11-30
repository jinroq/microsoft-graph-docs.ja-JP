---
title: plannerPlanDetails リソースの種類
description: '**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 plan オブジェクトには詳細オブジェクトがあります。'
ms.openlocfilehash: 1cce5727666bca705da67fccd1a3edf370c68127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073090"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="d44a3-104">plannerPlanDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d44a3-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="d44a3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d44a3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d44a3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d44a3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d44a3-p103">**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="d44a3-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d44a3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d44a3-109">Methods</span></span>

| <span data-ttu-id="d44a3-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d44a3-110">Method</span></span>           | <span data-ttu-id="d44a3-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d44a3-111">Return Type</span></span>    |<span data-ttu-id="d44a3-112">説明</span><span class="sxs-lookup"><span data-stu-id="d44a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d44a3-113">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d44a3-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="d44a3-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d44a3-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="d44a3-115">プロパティと、 **plannerPlanDetails**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d44a3-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="d44a3-116">Update</span><span class="sxs-lookup"><span data-stu-id="d44a3-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="d44a3-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d44a3-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="d44a3-118">**PlannerPlanDetails**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d44a3-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d44a3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d44a3-119">Properties</span></span>
| <span data-ttu-id="d44a3-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d44a3-120">Property</span></span>     | <span data-ttu-id="d44a3-121">型</span><span class="sxs-lookup"><span data-stu-id="d44a3-121">Type</span></span>   |<span data-ttu-id="d44a3-122">説明</span><span class="sxs-lookup"><span data-stu-id="d44a3-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d44a3-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d44a3-123">categoryDescriptions</span></span>|[<span data-ttu-id="d44a3-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d44a3-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="d44a3-125">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="d44a3-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="d44a3-126">id</span><span class="sxs-lookup"><span data-stu-id="d44a3-126">id</span></span>|<span data-ttu-id="d44a3-127">String</span><span class="sxs-lookup"><span data-stu-id="d44a3-127">String</span></span>| <span data-ttu-id="d44a3-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d44a3-128">Read-only.</span></span> <span data-ttu-id="d44a3-129">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="d44a3-129">The ID of the plan details.</span></span> <span data-ttu-id="d44a3-130">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d44a3-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d44a3-131">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="d44a3-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d44a3-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="d44a3-132">sharedWith</span></span>|[<span data-ttu-id="d44a3-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="d44a3-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="d44a3-134">一連のユーザーと共有は、この計画の Id。</span><span class="sxs-lookup"><span data-stu-id="d44a3-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="d44a3-135">Office 365 のグループを使用する場合は、[グループ](group.md)の計画を共有するグループ メンバーシップを管理するグループの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d44a3-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="d44a3-136">グループによって所有されているプランにアクセスするために必要はありませんが、このコレクションにグループの既存のメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="d44a3-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="d44a3-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="d44a3-137">contextDetails</span></span>|[<span data-ttu-id="d44a3-138">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="d44a3-138">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="d44a3-139">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d44a3-139">Read-only.</span></span> <span data-ttu-id="d44a3-140">[PlannerPlan](plannerplan.md)コンテナーに定義されている[plannerPlanContext](plannerplancontext.md)のエントリに関連付けられているその他の情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d44a3-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d44a3-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d44a3-141">Relationships</span></span>
<span data-ttu-id="d44a3-142">なし。</span><span class="sxs-lookup"><span data-stu-id="d44a3-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d44a3-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d44a3-143">JSON representation</span></span>
<span data-ttu-id="d44a3-144">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d44a3-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
