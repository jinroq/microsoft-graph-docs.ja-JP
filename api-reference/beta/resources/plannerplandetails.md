---
title: plannerPlanDetails リソースの種類
description: '**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 plan オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529881"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="e7b59-104">plannerPlanDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7b59-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7b59-p102">**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="e7b59-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="e7b59-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7b59-107">Methods</span></span>

| <span data-ttu-id="e7b59-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7b59-108">Method</span></span>           | <span data-ttu-id="e7b59-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7b59-109">Return Type</span></span>    |<span data-ttu-id="e7b59-110">説明</span><span class="sxs-lookup"><span data-stu-id="e7b59-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7b59-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e7b59-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="e7b59-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e7b59-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="e7b59-113">プロパティと、 **plannerPlanDetails**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7b59-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="e7b59-114">Update</span><span class="sxs-lookup"><span data-stu-id="e7b59-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="e7b59-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e7b59-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="e7b59-116">**PlannerPlanDetails**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7b59-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7b59-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7b59-117">Properties</span></span>
| <span data-ttu-id="e7b59-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7b59-118">Property</span></span>     | <span data-ttu-id="e7b59-119">型</span><span class="sxs-lookup"><span data-stu-id="e7b59-119">Type</span></span>   |<span data-ttu-id="e7b59-120">説明</span><span class="sxs-lookup"><span data-stu-id="e7b59-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7b59-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e7b59-121">categoryDescriptions</span></span>|[<span data-ttu-id="e7b59-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="e7b59-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="e7b59-123">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="e7b59-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="e7b59-124">id</span><span class="sxs-lookup"><span data-stu-id="e7b59-124">id</span></span>|<span data-ttu-id="e7b59-125">String</span><span class="sxs-lookup"><span data-stu-id="e7b59-125">String</span></span>| <span data-ttu-id="e7b59-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e7b59-126">Read-only.</span></span> <span data-ttu-id="e7b59-127">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="e7b59-127">The ID of the plan details.</span></span> <span data-ttu-id="e7b59-128">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e7b59-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e7b59-129">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="e7b59-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e7b59-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="e7b59-130">sharedWith</span></span>|[<span data-ttu-id="e7b59-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="e7b59-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="e7b59-132">一連のユーザーと共有は、この計画の Id。</span><span class="sxs-lookup"><span data-stu-id="e7b59-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="e7b59-133">Office 365 のグループを使用する場合は、[グループ](group.md)の計画を共有するグループ メンバーシップを管理するグループの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="e7b59-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="e7b59-134">グループによって所有されているプランにアクセスするために必要はありませんが、このコレクションにグループの既存のメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="e7b59-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="e7b59-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="e7b59-135">contextDetails</span></span>|[<span data-ttu-id="e7b59-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="e7b59-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="e7b59-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e7b59-137">Read-only.</span></span> <span data-ttu-id="e7b59-138">[PlannerPlan](plannerplan.md)コンテナーに定義されている[plannerPlanContext](plannerplancontext.md)のエントリに関連付けられているその他の情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e7b59-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e7b59-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7b59-139">Relationships</span></span>
<span data-ttu-id="e7b59-140">なし。</span><span class="sxs-lookup"><span data-stu-id="e7b59-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e7b59-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7b59-141">JSON representation</span></span>
<span data-ttu-id="e7b59-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7b59-142">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
