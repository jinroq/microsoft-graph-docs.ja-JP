---
title: licenseAssignmentState リソースの種類
description: ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**オブジェクトのコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649437"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="4ab56-104">licenseAssignmentState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ab56-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="4ab56-105">[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4ab56-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="4ab56-106">ユーザー ライセンスの割り当てに関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4ab56-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="4ab56-107">詳細情報には、次のような情報があります。</span><span class="sxs-lookup"><span data-stu-id="4ab56-107">The details include information such as:</span></span>  

 - <span data-ttu-id="4ab56-108">ユーザーに対してどのようなプランが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="4ab56-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="4ab56-109">ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか</span><span class="sxs-lookup"><span data-stu-id="4ab56-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="4ab56-110">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="4ab56-110">The current state of the assignment</span></span>
 - <span data-ttu-id="4ab56-111">割り当ての状態がエラーの場合、エラーの詳細</span><span class="sxs-lookup"><span data-stu-id="4ab56-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="4ab56-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ab56-112">Properties</span></span>
| <span data-ttu-id="4ab56-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ab56-113">Property</span></span>     | <span data-ttu-id="4ab56-114">型</span><span class="sxs-lookup"><span data-stu-id="4ab56-114">Type</span></span>   |<span data-ttu-id="4ab56-115">説明</span><span class="sxs-lookup"><span data-stu-id="4ab56-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ab56-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="4ab56-116">assignedByGroup</span></span>|<span data-ttu-id="4ab56-117">string</span><span class="sxs-lookup"><span data-stu-id="4ab56-117">string</span></span>|<span data-ttu-id="4ab56-118">このライセンスを割り当てられるグループの id。</span><span class="sxs-lookup"><span data-stu-id="4ab56-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="4ab56-119">割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="4ab56-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="4ab56-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ab56-120">Read-Only.</span></span>|
|<span data-ttu-id="4ab56-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="4ab56-121">disabledPlans</span></span>|<span data-ttu-id="4ab56-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="4ab56-122">Collection(String)</span></span>|<span data-ttu-id="4ab56-123">この割り当て内で無効になっているサービス プランです。</span><span class="sxs-lookup"><span data-stu-id="4ab56-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="4ab56-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ab56-124">Read-Only.</span></span>|
|<span data-ttu-id="4ab56-125">エラー</span><span class="sxs-lookup"><span data-stu-id="4ab56-125">error</span></span>|<span data-ttu-id="4ab56-126">文字列</span><span class="sxs-lookup"><span data-stu-id="4ab56-126">String</span></span>|<span data-ttu-id="4ab56-127">ライセンスの割り当てエラーです。</span><span class="sxs-lookup"><span data-stu-id="4ab56-127">License assignment failure error.</span></span> <span data-ttu-id="4ab56-128">ライセンスが正常に割り当てられると、このフィールドが Null になります。</span><span class="sxs-lookup"><span data-stu-id="4ab56-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="4ab56-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ab56-129">Read-Only.</span></span> <span data-ttu-id="4ab56-130">使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。</span><span class="sxs-lookup"><span data-stu-id="4ab56-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="4ab56-131">エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="4ab56-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="4ab56-132">skuId</span><span class="sxs-lookup"><span data-stu-id="4ab56-132">skuId</span></span>|<span data-ttu-id="4ab56-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4ab56-133">String</span></span>|<span data-ttu-id="4ab56-134">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4ab56-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="4ab56-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ab56-135">Read-Only.</span></span>|
|<span data-ttu-id="4ab56-136">state</span><span class="sxs-lookup"><span data-stu-id="4ab56-136">state</span></span>|<span data-ttu-id="4ab56-137">文字列</span><span class="sxs-lookup"><span data-stu-id="4ab56-137">String</span></span>|<span data-ttu-id="4ab56-138">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4ab56-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="4ab56-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ab56-139">Read-Only.</span></span> <span data-ttu-id="4ab56-140">使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。</span><span class="sxs-lookup"><span data-stu-id="4ab56-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ab56-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ab56-141">JSON representation</span></span>

<span data-ttu-id="4ab56-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ab56-142">The following is a JSON representation of the resource.</span></span>

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
