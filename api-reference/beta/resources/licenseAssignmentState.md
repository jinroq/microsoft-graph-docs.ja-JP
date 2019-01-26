---
title: licenseAssignmentState リソースの種類
description: 'ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  '
localization_priority: Normal
ms.openlocfilehash: f2f905baaba4dddd65266ffafab44febe7a61139
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575182"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="ae385-105">licenseAssignmentState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae385-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae385-106">[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ae385-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="ae385-107">ユーザー ライセンスの割り当てに関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ae385-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="ae385-108">詳細には、ような情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae385-108">The details includes information like:</span></span>  

 - <span data-ttu-id="ae385-109">ユーザーに対してどのようなプランが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="ae385-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="ae385-110">ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか</span><span class="sxs-lookup"><span data-stu-id="ae385-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="ae385-111">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="ae385-111">Current state of the assignment</span></span>
 - <span data-ttu-id="ae385-112">代入の状態がエラーの場合は、エラーのエラーの詳細は?</span><span class="sxs-lookup"><span data-stu-id="ae385-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="ae385-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae385-113">Properties</span></span>
| <span data-ttu-id="ae385-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae385-114">Property</span></span>     | <span data-ttu-id="ae385-115">型</span><span class="sxs-lookup"><span data-stu-id="ae385-115">Type</span></span>   |<span data-ttu-id="ae385-116">説明</span><span class="sxs-lookup"><span data-stu-id="ae385-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae385-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="ae385-117">assignedByGroup</span></span>|<span data-ttu-id="ae385-118">文字列</span><span class="sxs-lookup"><span data-stu-id="ae385-118">string</span></span>|<span data-ttu-id="ae385-119">このライセンスを割り当てられるグループの id。</span><span class="sxs-lookup"><span data-stu-id="ae385-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="ae385-120">割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="ae385-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="ae385-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae385-121">Read-Only.</span></span>|
|<span data-ttu-id="ae385-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="ae385-122">disabledPlans</span></span>| <span data-ttu-id="ae385-123">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ae385-123">String collection</span></span> |<span data-ttu-id="ae385-124">この割り当て内で無効になっているサービス プランです。</span><span class="sxs-lookup"><span data-stu-id="ae385-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="ae385-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae385-125">Read-Only.</span></span>|
|<span data-ttu-id="ae385-126">エラー</span><span class="sxs-lookup"><span data-stu-id="ae385-126">error</span></span>|<span data-ttu-id="ae385-127">String</span><span class="sxs-lookup"><span data-stu-id="ae385-127">String</span></span>|<span data-ttu-id="ae385-128">ライセンスの割り当てエラーです。</span><span class="sxs-lookup"><span data-stu-id="ae385-128">License assignment failure error.</span></span> <span data-ttu-id="ae385-129">ライセンスが正常に割り当てられると、このフィールドが Null になります。</span><span class="sxs-lookup"><span data-stu-id="ae385-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="ae385-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae385-130">Read-Only.</span></span> <span data-ttu-id="ae385-131">使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。</span><span class="sxs-lookup"><span data-stu-id="ae385-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="ae385-132">エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="ae385-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="ae385-133">skuId</span><span class="sxs-lookup"><span data-stu-id="ae385-133">skuId</span></span>|<span data-ttu-id="ae385-134">String</span><span class="sxs-lookup"><span data-stu-id="ae385-134">String</span></span>|<span data-ttu-id="ae385-135">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ae385-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="ae385-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae385-136">Read-Only.</span></span>|
|<span data-ttu-id="ae385-137">state</span><span class="sxs-lookup"><span data-stu-id="ae385-137">state</span></span>|<span data-ttu-id="ae385-138">String</span><span class="sxs-lookup"><span data-stu-id="ae385-138">String</span></span>|<span data-ttu-id="ae385-139">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="ae385-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="ae385-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae385-140">Read-Only.</span></span> <span data-ttu-id="ae385-141">使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。</span><span class="sxs-lookup"><span data-stu-id="ae385-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae385-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae385-142">JSON representation</span></span>

<span data-ttu-id="ae385-143">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ae385-143">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
