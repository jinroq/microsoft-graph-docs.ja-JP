---
title: license割り当て状態リソースの種類
description: user エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585147"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="12c56-104">license割り当て状態リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12c56-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="12c56-105">[user](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="12c56-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="12c56-106">ユーザーへのライセンス割り当てに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="12c56-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="12c56-107">詳細には、次のような情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="12c56-107">The details include information such as:</span></span>  

 - <span data-ttu-id="12c56-108">ユーザーに対して無効になるプラン</span><span class="sxs-lookup"><span data-stu-id="12c56-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="12c56-109">ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。</span><span class="sxs-lookup"><span data-stu-id="12c56-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="12c56-110">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="12c56-110">The current state of the assignment</span></span>
 - <span data-ttu-id="12c56-111">割り当ての状態がエラーの場合のエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="12c56-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="12c56-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12c56-112">Properties</span></span>
| <span data-ttu-id="12c56-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12c56-113">Property</span></span>     | <span data-ttu-id="12c56-114">型</span><span class="sxs-lookup"><span data-stu-id="12c56-114">Type</span></span>   |<span data-ttu-id="12c56-115">説明</span><span class="sxs-lookup"><span data-stu-id="12c56-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12c56-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="12c56-116">assignedByGroup</span></span>|<span data-ttu-id="12c56-117">string</span><span class="sxs-lookup"><span data-stu-id="12c56-117">string</span></span>|<span data-ttu-id="12c56-118">このライセンスを割り当てるグループの id。</span><span class="sxs-lookup"><span data-stu-id="12c56-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="12c56-119">割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="12c56-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="12c56-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12c56-120">Read-Only.</span></span>|
|<span data-ttu-id="12c56-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="12c56-121">disabledPlans</span></span>|<span data-ttu-id="12c56-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="12c56-122">Collection(String)</span></span>|<span data-ttu-id="12c56-123">この割り当てで無効になっているサービスプラン。</span><span class="sxs-lookup"><span data-stu-id="12c56-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="12c56-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12c56-124">Read-Only.</span></span>|
|<span data-ttu-id="12c56-125">error</span><span class="sxs-lookup"><span data-stu-id="12c56-125">error</span></span>|<span data-ttu-id="12c56-126">String</span><span class="sxs-lookup"><span data-stu-id="12c56-126">String</span></span>|<span data-ttu-id="12c56-127">ライセンスの割り当てエラーエラー。</span><span class="sxs-lookup"><span data-stu-id="12c56-127">License assignment failure error.</span></span> <span data-ttu-id="12c56-128">ライセンスが正常に割り当てられた場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="12c56-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="12c56-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12c56-129">Read-Only.</span></span> <span data-ttu-id="12c56-130">可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。</span><span class="sxs-lookup"><span data-stu-id="12c56-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="12c56-131">ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12c56-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="12c56-132">skuId</span><span class="sxs-lookup"><span data-stu-id="12c56-132">skuId</span></span>|<span data-ttu-id="12c56-133">String</span><span class="sxs-lookup"><span data-stu-id="12c56-133">String</span></span>|<span data-ttu-id="12c56-134">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="12c56-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="12c56-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12c56-135">Read-Only.</span></span>|
|<span data-ttu-id="12c56-136">state</span><span class="sxs-lookup"><span data-stu-id="12c56-136">state</span></span>|<span data-ttu-id="12c56-137">String</span><span class="sxs-lookup"><span data-stu-id="12c56-137">String</span></span>|<span data-ttu-id="12c56-138">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="12c56-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="12c56-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12c56-139">Read-Only.</span></span> <span data-ttu-id="12c56-140">使用可能な値: Active、activewitherror、Disabled、および error。</span><span class="sxs-lookup"><span data-stu-id="12c56-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12c56-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12c56-141">JSON representation</span></span>

<span data-ttu-id="12c56-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="12c56-142">The following is a JSON representation of the resource.</span></span>

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
