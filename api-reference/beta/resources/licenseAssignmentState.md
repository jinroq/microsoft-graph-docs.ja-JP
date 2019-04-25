---
title: license割り当て状態リソースの種類
description: 'user エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。 詳細には、次のような情報が含まれます。  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581108"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="4c5bc-105">license割り当て状態リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c5bc-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c5bc-106">[user](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="4c5bc-107">ユーザーへのライセンス割り当てに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="4c5bc-108">詳細には、次のような情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-108">The details includes information like:</span></span>  

 - <span data-ttu-id="4c5bc-109">ユーザーに対して無効になるプラン</span><span class="sxs-lookup"><span data-stu-id="4c5bc-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="4c5bc-110">ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="4c5bc-111">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="4c5bc-111">Current state of the assignment</span></span>
 - <span data-ttu-id="4c5bc-112">割り当ての状態がエラーの場合は、エラーの詳細がどのようなものですか。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="4c5bc-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c5bc-113">Properties</span></span>
| <span data-ttu-id="4c5bc-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c5bc-114">Property</span></span>     | <span data-ttu-id="4c5bc-115">型</span><span class="sxs-lookup"><span data-stu-id="4c5bc-115">Type</span></span>   |<span data-ttu-id="4c5bc-116">説明</span><span class="sxs-lookup"><span data-stu-id="4c5bc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c5bc-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="4c5bc-117">assignedByGroup</span></span>|<span data-ttu-id="4c5bc-118">string</span><span class="sxs-lookup"><span data-stu-id="4c5bc-118">string</span></span>|<span data-ttu-id="4c5bc-119">このライセンスを割り当てるグループの id。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="4c5bc-120">割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="4c5bc-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-121">Read-Only.</span></span>|
|<span data-ttu-id="4c5bc-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="4c5bc-122">disabledPlans</span></span>|<span data-ttu-id="4c5bc-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="4c5bc-123">Collection(String)</span></span>|<span data-ttu-id="4c5bc-124">この割り当てで無効になっているサービスプラン。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="4c5bc-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-125">Read-Only.</span></span>|
|<span data-ttu-id="4c5bc-126">error</span><span class="sxs-lookup"><span data-stu-id="4c5bc-126">error</span></span>|<span data-ttu-id="4c5bc-127">String</span><span class="sxs-lookup"><span data-stu-id="4c5bc-127">String</span></span>|<span data-ttu-id="4c5bc-128">ライセンスの割り当てエラーエラー。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-128">License assignment failure error.</span></span> <span data-ttu-id="4c5bc-129">ライセンスが正常に割り当てられた場合、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="4c5bc-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-130">Read-Only.</span></span> <span data-ttu-id="4c5bc-131">可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="4c5bc-132">ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="4c5bc-133">skuId</span><span class="sxs-lookup"><span data-stu-id="4c5bc-133">skuId</span></span>|<span data-ttu-id="4c5bc-134">String</span><span class="sxs-lookup"><span data-stu-id="4c5bc-134">String</span></span>|<span data-ttu-id="4c5bc-135">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="4c5bc-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-136">Read-Only.</span></span>|
|<span data-ttu-id="4c5bc-137">state</span><span class="sxs-lookup"><span data-stu-id="4c5bc-137">state</span></span>|<span data-ttu-id="4c5bc-138">String</span><span class="sxs-lookup"><span data-stu-id="4c5bc-138">String</span></span>|<span data-ttu-id="4c5bc-139">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="4c5bc-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-140">Read-Only.</span></span> <span data-ttu-id="4c5bc-141">使用可能な値: Active、activewitherror、Disabled、および error。</span><span class="sxs-lookup"><span data-stu-id="4c5bc-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c5bc-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c5bc-142">JSON representation</span></span>

<span data-ttu-id="4c5bc-143">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4c5bc-143">Here is a JSON representation of the resource</span></span>

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
