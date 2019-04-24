---
title: プランワークプランの詳細リソースの種類
description: "\"plan/プランの**詳細**\" リソースは、プランに関する追加情報を表します。 各 plan オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522133"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="c0f37-104">プランワークプランの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0f37-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f37-105">"plan/プランの**詳細**" リソースは、プランに関する追加情報を表します。</span><span class="sxs-lookup"><span data-stu-id="c0f37-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="c0f37-106">各[plan](plannerplan.md)オブジェクトには details オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="c0f37-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="c0f37-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0f37-107">Methods</span></span>

| <span data-ttu-id="c0f37-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0f37-108">Method</span></span>           | <span data-ttu-id="c0f37-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c0f37-109">Return Type</span></span>    |<span data-ttu-id="c0f37-110">説明</span><span class="sxs-lookup"><span data-stu-id="c0f37-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0f37-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c0f37-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="c0f37-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c0f37-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="c0f37-113">**plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c0f37-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="c0f37-114">更新する</span><span class="sxs-lookup"><span data-stu-id="c0f37-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="c0f37-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c0f37-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="c0f37-116">"plan/プランの**詳細**" オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0f37-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0f37-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0f37-117">Properties</span></span>
| <span data-ttu-id="c0f37-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0f37-118">Property</span></span>     | <span data-ttu-id="c0f37-119">型</span><span class="sxs-lookup"><span data-stu-id="c0f37-119">Type</span></span>   |<span data-ttu-id="c0f37-120">説明</span><span class="sxs-lookup"><span data-stu-id="c0f37-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0f37-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="c0f37-121">categoryDescriptions</span></span>|[<span data-ttu-id="c0f37-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="c0f37-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="c0f37-123">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="c0f37-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="c0f37-124">id</span><span class="sxs-lookup"><span data-stu-id="c0f37-124">id</span></span>|<span data-ttu-id="c0f37-125">String</span><span class="sxs-lookup"><span data-stu-id="c0f37-125">String</span></span>| <span data-ttu-id="c0f37-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c0f37-126">Read-only.</span></span> <span data-ttu-id="c0f37-127">プランの詳細の ID。</span><span class="sxs-lookup"><span data-stu-id="c0f37-127">The ID of the plan details.</span></span> <span data-ttu-id="c0f37-128">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="c0f37-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c0f37-129">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="c0f37-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c0f37-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="c0f37-130">sharedWith</span></span>|[<span data-ttu-id="c0f37-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="c0f37-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="c0f37-132">このプランで共有される一連のユーザー id。</span><span class="sxs-lookup"><span data-stu-id="c0f37-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="c0f37-133">Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループ[の](group.md)計画を共有します。</span><span class="sxs-lookup"><span data-stu-id="c0f37-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="c0f37-134">グループの既存のメンバーをこのコレクションに追加することもできますが、グループが所有しているプランにアクセスするために必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="c0f37-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="c0f37-135">contextdetails</span><span class="sxs-lookup"><span data-stu-id="c0f37-135">contextDetails</span></span>|[<span data-ttu-id="c0f37-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="c0f37-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="c0f37-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c0f37-137">Read-only.</span></span> <span data-ttu-id="c0f37-138">プランに関連付けられている追加情報のコレクション。 plan の[プラン](plannerplan.md)コンテナーに対して定義された[コンテキスト](plannerplancontext.md)エントリ。</span><span class="sxs-lookup"><span data-stu-id="c0f37-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c0f37-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0f37-139">Relationships</span></span>
<span data-ttu-id="c0f37-140">なし。</span><span class="sxs-lookup"><span data-stu-id="c0f37-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c0f37-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0f37-141">JSON representation</span></span>
<span data-ttu-id="c0f37-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0f37-142">The following is a JSON representation of the resource.</span></span>

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
