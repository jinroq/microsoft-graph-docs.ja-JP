---
title: License割り当て状態リソースの種類
description: 'User エンティティの**License割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。 詳細には、次のような情報が含まれます。  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778430"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="eb984-105">License割り当て状態リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb984-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb984-106">[User](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="eb984-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="eb984-107">ユーザーへのライセンス割り当てに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb984-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="eb984-108">詳細には、次のような情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="eb984-108">The details includes information like:</span></span>  

- <span data-ttu-id="eb984-109">ユーザーに対して無効になるプラン</span><span class="sxs-lookup"><span data-stu-id="eb984-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="eb984-110">ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。</span><span class="sxs-lookup"><span data-stu-id="eb984-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="eb984-111">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="eb984-111">Current state of the assignment</span></span>
- <span data-ttu-id="eb984-112">割り当ての状態がエラーの場合は、エラーの詳細がどのようなものですか。</span><span class="sxs-lookup"><span data-stu-id="eb984-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="eb984-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb984-113">Properties</span></span>
| <span data-ttu-id="eb984-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb984-114">Property</span></span>     | <span data-ttu-id="eb984-115">型</span><span class="sxs-lookup"><span data-stu-id="eb984-115">Type</span></span>   |<span data-ttu-id="eb984-116">説明</span><span class="sxs-lookup"><span data-stu-id="eb984-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb984-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="eb984-117">assignedByGroup</span></span>|<span data-ttu-id="eb984-118">string</span><span class="sxs-lookup"><span data-stu-id="eb984-118">string</span></span>|<span data-ttu-id="eb984-119">このライセンスを割り当てるグループの id。</span><span class="sxs-lookup"><span data-stu-id="eb984-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="eb984-120">割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="eb984-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="eb984-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb984-121">Read-Only.</span></span>|
|<span data-ttu-id="eb984-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="eb984-122">disabledPlans</span></span>|<span data-ttu-id="eb984-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="eb984-123">Collection(String)</span></span>|<span data-ttu-id="eb984-124">この割り当てで無効になっているサービスプラン。</span><span class="sxs-lookup"><span data-stu-id="eb984-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="eb984-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb984-125">Read-Only.</span></span>|
|<span data-ttu-id="eb984-126">error</span><span class="sxs-lookup"><span data-stu-id="eb984-126">error</span></span>|<span data-ttu-id="eb984-127">String</span><span class="sxs-lookup"><span data-stu-id="eb984-127">String</span></span>|<span data-ttu-id="eb984-128">ライセンスの割り当てエラーエラー。</span><span class="sxs-lookup"><span data-stu-id="eb984-128">License assignment failure error.</span></span> <span data-ttu-id="eb984-129">ライセンスが正常に割り当てられた場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="eb984-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="eb984-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb984-130">Read-Only.</span></span> <span data-ttu-id="eb984-131">可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。</span><span class="sxs-lookup"><span data-stu-id="eb984-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="eb984-132">ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb984-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="eb984-133">skuId</span><span class="sxs-lookup"><span data-stu-id="eb984-133">skuId</span></span>|<span data-ttu-id="eb984-134">String</span><span class="sxs-lookup"><span data-stu-id="eb984-134">String</span></span>|<span data-ttu-id="eb984-135">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="eb984-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="eb984-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb984-136">Read-Only.</span></span>|
|<span data-ttu-id="eb984-137">state</span><span class="sxs-lookup"><span data-stu-id="eb984-137">state</span></span>|<span data-ttu-id="eb984-138">String</span><span class="sxs-lookup"><span data-stu-id="eb984-138">String</span></span>|<span data-ttu-id="eb984-139">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="eb984-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="eb984-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb984-140">Read-Only.</span></span> <span data-ttu-id="eb984-141">使用可能な値: Active、ActiveWithError、Disabled、および Error。</span><span class="sxs-lookup"><span data-stu-id="eb984-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb984-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb984-142">JSON representation</span></span>

<span data-ttu-id="eb984-143">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="eb984-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
