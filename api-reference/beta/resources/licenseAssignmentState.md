---
title: licenseAssignmentState リソースの種類
description: 'ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  '
localization_priority: Normal
ms.openlocfilehash: 51ff878f356902362487eda36d17c1894c33e5f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855630"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="b7687-105">licenseAssignmentState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7687-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="b7687-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7687-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7687-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7687-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7687-108">[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b7687-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="b7687-109">ユーザー ライセンスの割り当てに関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b7687-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="b7687-110">詳細には、ような情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7687-110">The details includes information like:</span></span>  

 - <span data-ttu-id="b7687-111">ユーザーに対してどのようなプランが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="b7687-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="b7687-112">ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか</span><span class="sxs-lookup"><span data-stu-id="b7687-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="b7687-113">割り当ての現在の状態</span><span class="sxs-lookup"><span data-stu-id="b7687-113">Current state of the assignment</span></span>
 - <span data-ttu-id="b7687-114">代入の状態がエラーの場合は、エラーのエラーの詳細は?</span><span class="sxs-lookup"><span data-stu-id="b7687-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="b7687-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7687-115">Properties</span></span>
| <span data-ttu-id="b7687-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7687-116">Property</span></span>     | <span data-ttu-id="b7687-117">種類</span><span class="sxs-lookup"><span data-stu-id="b7687-117">Type</span></span>   |<span data-ttu-id="b7687-118">説明</span><span class="sxs-lookup"><span data-stu-id="b7687-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7687-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="b7687-119">assignedByGroup</span></span>|<span data-ttu-id="b7687-120">文字列</span><span class="sxs-lookup"><span data-stu-id="b7687-120">string</span></span>|<span data-ttu-id="b7687-121">このライセンスを割り当てられるグループの id。</span><span class="sxs-lookup"><span data-stu-id="b7687-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="b7687-122">割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。</span><span class="sxs-lookup"><span data-stu-id="b7687-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="b7687-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7687-123">Read-Only.</span></span>|
|<span data-ttu-id="b7687-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="b7687-124">disabledPlans</span></span>|<span data-ttu-id="b7687-125">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="b7687-125">Collection(String)</span></span>|<span data-ttu-id="b7687-126">この割り当て内で無効になっているサービス プランです。</span><span class="sxs-lookup"><span data-stu-id="b7687-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="b7687-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7687-127">Read-Only.</span></span>|
|<span data-ttu-id="b7687-128">エラー</span><span class="sxs-lookup"><span data-stu-id="b7687-128">error</span></span>|<span data-ttu-id="b7687-129">String</span><span class="sxs-lookup"><span data-stu-id="b7687-129">String</span></span>|<span data-ttu-id="b7687-130">ライセンスの割り当てエラーです。</span><span class="sxs-lookup"><span data-stu-id="b7687-130">License assignment failure error.</span></span> <span data-ttu-id="b7687-131">ライセンスが正常に割り当てられると、このフィールドが Null になります。</span><span class="sxs-lookup"><span data-stu-id="b7687-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="b7687-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7687-132">Read-Only.</span></span> <span data-ttu-id="b7687-133">使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。</span><span class="sxs-lookup"><span data-stu-id="b7687-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="b7687-134">エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="b7687-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="b7687-135">skuId</span><span class="sxs-lookup"><span data-stu-id="b7687-135">skuId</span></span>|<span data-ttu-id="b7687-136">String</span><span class="sxs-lookup"><span data-stu-id="b7687-136">String</span></span>|<span data-ttu-id="b7687-137">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b7687-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="b7687-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7687-138">Read-Only.</span></span>|
|<span data-ttu-id="b7687-139">state</span><span class="sxs-lookup"><span data-stu-id="b7687-139">state</span></span>|<span data-ttu-id="b7687-140">String</span><span class="sxs-lookup"><span data-stu-id="b7687-140">String</span></span>|<span data-ttu-id="b7687-141">この割り当ての現在の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="b7687-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="b7687-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7687-142">Read-Only.</span></span> <span data-ttu-id="b7687-143">使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。</span><span class="sxs-lookup"><span data-stu-id="b7687-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7687-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7687-144">JSON representation</span></span>

<span data-ttu-id="b7687-145">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b7687-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
