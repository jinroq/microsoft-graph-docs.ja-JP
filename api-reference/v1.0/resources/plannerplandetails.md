---
title: プランワークプランの詳細リソースの種類
description: "\"plan/プランの**詳細**\" リソースは、プランに関する追加情報を表します。 各 plan オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5661477ff59036e633eb82c23e9c50d7c2c8b4a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462332"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="3609d-104">プランワークプランの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3609d-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="3609d-105">"plan/プランの**詳細**" リソースは、プランに関する追加情報を表します。</span><span class="sxs-lookup"><span data-stu-id="3609d-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="3609d-106">各[plan](plannerplan.md)オブジェクトには details オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="3609d-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="3609d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3609d-107">Methods</span></span>

| <span data-ttu-id="3609d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3609d-108">Method</span></span>           | <span data-ttu-id="3609d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3609d-109">Return Type</span></span>    |<span data-ttu-id="3609d-110">説明</span><span class="sxs-lookup"><span data-stu-id="3609d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3609d-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="3609d-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="3609d-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="3609d-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="3609d-113">**plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3609d-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="3609d-114">Update</span><span class="sxs-lookup"><span data-stu-id="3609d-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="3609d-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="3609d-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="3609d-116">**プランの詳細**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3609d-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3609d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3609d-117">Properties</span></span>
| <span data-ttu-id="3609d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3609d-118">Property</span></span>     | <span data-ttu-id="3609d-119">型</span><span class="sxs-lookup"><span data-stu-id="3609d-119">Type</span></span>   |<span data-ttu-id="3609d-120">説明</span><span class="sxs-lookup"><span data-stu-id="3609d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3609d-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="3609d-121">categoryDescriptions</span></span>|[<span data-ttu-id="3609d-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="3609d-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="3609d-123">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="3609d-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="3609d-124">id</span><span class="sxs-lookup"><span data-stu-id="3609d-124">id</span></span>|<span data-ttu-id="3609d-125">String</span><span class="sxs-lookup"><span data-stu-id="3609d-125">String</span></span>| <span data-ttu-id="3609d-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3609d-126">Read-only.</span></span> <span data-ttu-id="3609d-127">プランの詳細の ID。</span><span class="sxs-lookup"><span data-stu-id="3609d-127">ID of the plan details.</span></span> <span data-ttu-id="3609d-128">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="3609d-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3609d-129">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="3609d-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3609d-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="3609d-130">sharedWith</span></span>|[<span data-ttu-id="3609d-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="3609d-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="3609d-p104">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="3609d-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3609d-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3609d-135">Relationships</span></span>
<span data-ttu-id="3609d-136">なし</span><span class="sxs-lookup"><span data-stu-id="3609d-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3609d-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3609d-137">JSON representation</span></span>
<span data-ttu-id="3609d-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3609d-138">Here is a JSON representation of the resource.</span></span>

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
