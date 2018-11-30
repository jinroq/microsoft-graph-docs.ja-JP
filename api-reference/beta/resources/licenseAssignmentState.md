---
title: licenseAssignmentState リソースの種類
description: 'ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072227"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="3c112-105">licenseAssignmentState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c112-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="3c112-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c112-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c112-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c112-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c112-108">[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3c112-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="3c112-109">ユーザー ライセンスの割り当てに関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3c112-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="3c112-110">詳細には、ような情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c112-110">The details includes information like:</span></span>  

 - <span data-ttu-id="3c112-111">ユーザーに対してどのようなプランが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="3c112-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="3c112-112">ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか</span><span class="sxs-lookup"><span data-stu-id="3c112-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="3c112-113">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="3c112-113">Current state of the assignment</span></span>
 - <span data-ttu-id="3c112-114">代入の状態がエラーの場合は、エラーのエラーの詳細は?</span><span class="sxs-lookup"><span data-stu-id="3c112-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="3c112-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c112-115">Properties</span></span>
| <span data-ttu-id="3c112-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c112-116">Property</span></span>     | <span data-ttu-id="3c112-117">型</span><span class="sxs-lookup"><span data-stu-id="3c112-117">Type</span></span>   |<span data-ttu-id="3c112-118">説明</span><span class="sxs-lookup"><span data-stu-id="3c112-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c112-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="3c112-119">assignedByGroup</span></span>|<span data-ttu-id="3c112-120">文字列</span><span class="sxs-lookup"><span data-stu-id="3c112-120">string</span></span>|<span data-ttu-id="3c112-121">このライセンスを割り当てられるグループの id。</span><span class="sxs-lookup"><span data-stu-id="3c112-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="3c112-122">割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="3c112-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="3c112-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c112-123">Read-Only.</span></span>|
|<span data-ttu-id="3c112-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="3c112-124">disabledPlans</span></span>|<span data-ttu-id="3c112-125">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="3c112-125">Collection(String)</span></span>|<span data-ttu-id="3c112-126">この割り当て内で無効になっているサービス プランです。</span><span class="sxs-lookup"><span data-stu-id="3c112-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="3c112-127">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c112-127">Read-Only.</span></span>|
|<span data-ttu-id="3c112-128">エラー</span><span class="sxs-lookup"><span data-stu-id="3c112-128">error</span></span>|<span data-ttu-id="3c112-129">String</span><span class="sxs-lookup"><span data-stu-id="3c112-129">String</span></span>|<span data-ttu-id="3c112-130">ライセンスの割り当てエラーです。</span><span class="sxs-lookup"><span data-stu-id="3c112-130">License assignment failure error.</span></span> <span data-ttu-id="3c112-131">ライセンスが正常に割り当てられると、このフィールドが Null になります。</span><span class="sxs-lookup"><span data-stu-id="3c112-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="3c112-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c112-132">Read-Only.</span></span> <span data-ttu-id="3c112-133">使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。</span><span class="sxs-lookup"><span data-stu-id="3c112-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="3c112-134">エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="3c112-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="3c112-135">skuId</span><span class="sxs-lookup"><span data-stu-id="3c112-135">skuId</span></span>|<span data-ttu-id="3c112-136">String</span><span class="sxs-lookup"><span data-stu-id="3c112-136">String</span></span>|<span data-ttu-id="3c112-137">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3c112-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="3c112-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c112-138">Read-Only.</span></span>|
|<span data-ttu-id="3c112-139">state</span><span class="sxs-lookup"><span data-stu-id="3c112-139">state</span></span>|<span data-ttu-id="3c112-140">String</span><span class="sxs-lookup"><span data-stu-id="3c112-140">String</span></span>|<span data-ttu-id="3c112-141">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="3c112-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="3c112-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c112-142">Read-Only.</span></span> <span data-ttu-id="3c112-143">使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。</span><span class="sxs-lookup"><span data-stu-id="3c112-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c112-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c112-144">JSON representation</span></span>

<span data-ttu-id="3c112-145">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3c112-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```