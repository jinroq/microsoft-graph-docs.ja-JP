---
title: License割り当て状態リソースの種類
description: User エンティティの**License割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 358c54ae2562479734cc496b1fe9ab8eb34812fa
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778692"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="d4d2c-104">License割り当て状態リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4d2c-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="d4d2c-105">[User](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="d4d2c-106">ユーザーへのライセンス割り当てに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="d4d2c-107">詳細には、次のような情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-107">The details include information such as:</span></span>  

- <span data-ttu-id="d4d2c-108">ユーザーに対して無効になるプラン</span><span class="sxs-lookup"><span data-stu-id="d4d2c-108">What plans are disabled for a user</span></span>
- <span data-ttu-id="d4d2c-109">ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="d4d2c-110">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="d4d2c-110">The current state of the assignment</span></span>
- <span data-ttu-id="d4d2c-111">割り当ての状態がエラーの場合のエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="d4d2c-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="d4d2c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4d2c-112">Properties</span></span>
| <span data-ttu-id="d4d2c-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4d2c-113">Property</span></span>     | <span data-ttu-id="d4d2c-114">型</span><span class="sxs-lookup"><span data-stu-id="d4d2c-114">Type</span></span>   |<span data-ttu-id="d4d2c-115">説明</span><span class="sxs-lookup"><span data-stu-id="d4d2c-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4d2c-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="d4d2c-116">assignedByGroup</span></span>|<span data-ttu-id="d4d2c-117">string</span><span class="sxs-lookup"><span data-stu-id="d4d2c-117">string</span></span>|<span data-ttu-id="d4d2c-118">このライセンスを割り当てるグループの id。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="d4d2c-119">割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="d4d2c-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-120">Read-Only.</span></span>|
|<span data-ttu-id="d4d2c-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="d4d2c-121">disabledPlans</span></span>|<span data-ttu-id="d4d2c-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="d4d2c-122">Collection(String)</span></span>|<span data-ttu-id="d4d2c-123">この割り当てで無効になっているサービスプラン。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="d4d2c-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-124">Read-Only.</span></span>|
|<span data-ttu-id="d4d2c-125">error</span><span class="sxs-lookup"><span data-stu-id="d4d2c-125">error</span></span>|<span data-ttu-id="d4d2c-126">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-126">String</span></span>|<span data-ttu-id="d4d2c-127">ライセンスの割り当てエラーエラー。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-127">License assignment failure error.</span></span> <span data-ttu-id="d4d2c-128">ライセンスが正常に割り当てられた場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="d4d2c-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-129">Read-Only.</span></span> <span data-ttu-id="d4d2c-130">可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="d4d2c-131">ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="d4d2c-132">skuId</span><span class="sxs-lookup"><span data-stu-id="d4d2c-132">skuId</span></span>|<span data-ttu-id="d4d2c-133">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-133">String</span></span>|<span data-ttu-id="d4d2c-134">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="d4d2c-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-135">Read-Only.</span></span>|
|<span data-ttu-id="d4d2c-136">state</span><span class="sxs-lookup"><span data-stu-id="d4d2c-136">state</span></span>|<span data-ttu-id="d4d2c-137">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-137">String</span></span>|<span data-ttu-id="d4d2c-138">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="d4d2c-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-139">Read-Only.</span></span> <span data-ttu-id="d4d2c-140">使用可能な値: Active、ActiveWithError、Disabled、および Error。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4d2c-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4d2c-141">JSON representation</span></span>

<span data-ttu-id="d4d2c-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4d2c-142">The following is a JSON representation of the resource.</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
