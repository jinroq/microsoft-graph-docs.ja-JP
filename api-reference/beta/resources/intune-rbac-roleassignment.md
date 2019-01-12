---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d3f50e028bed17daf9acfe0eaf62776476b1bb61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927570"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="a6548-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6548-106">roleAssignment resource type</span></span>

> <span data-ttu-id="a6548-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6548-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6548-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6548-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6548-109">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6548-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6548-110">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="a6548-110">The Role Assignment resource.</span></span> <span data-ttu-id="a6548-111">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="a6548-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="a6548-112">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="a6548-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="a6548-113">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6548-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="a6548-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6548-114">Methods</span></span>
|<span data-ttu-id="a6548-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6548-115">Method</span></span>|<span data-ttu-id="a6548-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6548-116">Return Type</span></span>|<span data-ttu-id="a6548-117">説明</span><span class="sxs-lookup"><span data-stu-id="a6548-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6548-118">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="a6548-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="a6548-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6548-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="a6548-120">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a6548-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="a6548-121">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="a6548-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="a6548-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6548-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6548-123">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a6548-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a6548-124">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="a6548-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="a6548-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6548-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6548-126">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a6548-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a6548-127">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="a6548-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="a6548-128">なし</span><span class="sxs-lookup"><span data-stu-id="a6548-128">None</span></span>|<span data-ttu-id="a6548-129">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a6548-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="a6548-130">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="a6548-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="a6548-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6548-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a6548-132">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6548-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6548-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6548-133">Properties</span></span>
|<span data-ttu-id="a6548-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6548-134">Property</span></span>|<span data-ttu-id="a6548-135">種類</span><span class="sxs-lookup"><span data-stu-id="a6548-135">Type</span></span>|<span data-ttu-id="a6548-136">説明</span><span class="sxs-lookup"><span data-stu-id="a6548-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6548-137">ID</span><span class="sxs-lookup"><span data-stu-id="a6548-137">id</span></span>|<span data-ttu-id="a6548-138">String</span><span class="sxs-lookup"><span data-stu-id="a6548-138">String</span></span>|<span data-ttu-id="a6548-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6548-139">Key of the entity.</span></span> <span data-ttu-id="a6548-140">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="a6548-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a6548-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a6548-141">displayName</span></span>|<span data-ttu-id="a6548-142">String</span><span class="sxs-lookup"><span data-stu-id="a6548-142">String</span></span>|<span data-ttu-id="a6548-143">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="a6548-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a6548-144">説明</span><span class="sxs-lookup"><span data-stu-id="a6548-144">description</span></span>|<span data-ttu-id="a6548-145">String</span><span class="sxs-lookup"><span data-stu-id="a6548-145">String</span></span>|<span data-ttu-id="a6548-146">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="a6548-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a6548-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="a6548-147">scopeMembers</span></span>|<span data-ttu-id="a6548-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6548-148">String collection</span></span>|<span data-ttu-id="a6548-149">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="a6548-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a6548-150">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="a6548-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="a6548-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="a6548-151">scopeType</span></span>|[<span data-ttu-id="a6548-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="a6548-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="a6548-153">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6548-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="a6548-154">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a6548-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="a6548-155">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="a6548-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="a6548-156">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="a6548-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="a6548-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a6548-157">resourceScopes</span></span>|<span data-ttu-id="a6548-158">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6548-158">String collection</span></span>|<span data-ttu-id="a6548-159">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="a6548-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a6548-160">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="a6548-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6548-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6548-161">Relationships</span></span>
|<span data-ttu-id="a6548-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6548-162">Relationship</span></span>|<span data-ttu-id="a6548-163">型</span><span class="sxs-lookup"><span data-stu-id="a6548-163">Type</span></span>|<span data-ttu-id="a6548-164">説明</span><span class="sxs-lookup"><span data-stu-id="a6548-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6548-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6548-165">roleDefinition</span></span>|[<span data-ttu-id="a6548-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6548-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a6548-167">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="a6548-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6548-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6548-168">JSON Representation</span></span>
<span data-ttu-id="a6548-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6548-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```





