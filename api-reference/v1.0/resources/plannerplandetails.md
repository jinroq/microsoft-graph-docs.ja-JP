---
title: plannerPlanDetails リソースの種類
description: '**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 plan オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5661477ff59036e633eb82c23e9c50d7c2c8b4a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934675"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="5cbc6-104">plannerPlanDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5cbc6-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="5cbc6-p102">**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="5cbc6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5cbc6-107">Methods</span></span>

| <span data-ttu-id="5cbc6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5cbc6-108">Method</span></span>           | <span data-ttu-id="5cbc6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5cbc6-109">Return Type</span></span>    |<span data-ttu-id="5cbc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="5cbc6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cbc6-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="5cbc6-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="5cbc6-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="5cbc6-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="5cbc6-113">**plannerPlanDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="5cbc6-114">Update</span><span class="sxs-lookup"><span data-stu-id="5cbc6-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="5cbc6-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="5cbc6-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="5cbc6-116">**plannerPlanDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cbc6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cbc6-117">Properties</span></span>
| <span data-ttu-id="5cbc6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cbc6-118">Property</span></span>     | <span data-ttu-id="5cbc6-119">型</span><span class="sxs-lookup"><span data-stu-id="5cbc6-119">Type</span></span>   |<span data-ttu-id="5cbc6-120">説明</span><span class="sxs-lookup"><span data-stu-id="5cbc6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cbc6-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="5cbc6-121">categoryDescriptions</span></span>|[<span data-ttu-id="5cbc6-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="5cbc6-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="5cbc6-123">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="5cbc6-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="5cbc6-124">id</span><span class="sxs-lookup"><span data-stu-id="5cbc6-124">id</span></span>|<span data-ttu-id="5cbc6-125">String</span><span class="sxs-lookup"><span data-stu-id="5cbc6-125">String</span></span>| <span data-ttu-id="5cbc6-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-126">Read-only.</span></span> <span data-ttu-id="5cbc6-127">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-127">ID of the plan details.</span></span> <span data-ttu-id="5cbc6-128">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5cbc6-129">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5cbc6-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="5cbc6-130">sharedWith</span></span>|[<span data-ttu-id="5cbc6-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="5cbc6-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="5cbc6-p104">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5cbc6-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5cbc6-135">Relationships</span></span>
<span data-ttu-id="5cbc6-136">なし</span><span class="sxs-lookup"><span data-stu-id="5cbc6-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5cbc6-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5cbc6-137">JSON representation</span></span>
<span data-ttu-id="5cbc6-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5cbc6-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
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
