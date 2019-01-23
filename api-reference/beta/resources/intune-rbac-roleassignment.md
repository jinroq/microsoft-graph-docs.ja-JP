---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11fc37502fa017494ff884cb70f0006277a42600
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415125"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="fb03f-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb03f-106">roleAssignment resource type</span></span>

> <span data-ttu-id="fb03f-107">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb03f-107">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb03f-108">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb03f-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb03f-109">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb03f-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb03f-110">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="fb03f-110">The Role Assignment resource.</span></span> <span data-ttu-id="fb03f-111">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="fb03f-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="fb03f-112">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="fb03f-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="fb03f-113">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fb03f-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="fb03f-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb03f-114">Methods</span></span>
|<span data-ttu-id="fb03f-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb03f-115">Method</span></span>|<span data-ttu-id="fb03f-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fb03f-116">Return Type</span></span>|<span data-ttu-id="fb03f-117">説明</span><span class="sxs-lookup"><span data-stu-id="fb03f-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fb03f-118">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="fb03f-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="fb03f-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fb03f-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="fb03f-120">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fb03f-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="fb03f-121">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="fb03f-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="fb03f-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb03f-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fb03f-123">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fb03f-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fb03f-124">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="fb03f-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="fb03f-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb03f-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fb03f-126">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fb03f-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fb03f-127">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="fb03f-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="fb03f-128">なし</span><span class="sxs-lookup"><span data-stu-id="fb03f-128">None</span></span>|<span data-ttu-id="fb03f-129">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fb03f-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="fb03f-130">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="fb03f-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="fb03f-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb03f-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fb03f-132">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb03f-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb03f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb03f-133">Properties</span></span>
|<span data-ttu-id="fb03f-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb03f-134">Property</span></span>|<span data-ttu-id="fb03f-135">型</span><span class="sxs-lookup"><span data-stu-id="fb03f-135">Type</span></span>|<span data-ttu-id="fb03f-136">説明</span><span class="sxs-lookup"><span data-stu-id="fb03f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb03f-137">id</span><span class="sxs-lookup"><span data-stu-id="fb03f-137">id</span></span>|<span data-ttu-id="fb03f-138">String</span><span class="sxs-lookup"><span data-stu-id="fb03f-138">String</span></span>|<span data-ttu-id="fb03f-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fb03f-139">Key of the entity.</span></span> <span data-ttu-id="fb03f-140">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="fb03f-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fb03f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="fb03f-141">displayName</span></span>|<span data-ttu-id="fb03f-142">String</span><span class="sxs-lookup"><span data-stu-id="fb03f-142">String</span></span>|<span data-ttu-id="fb03f-143">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="fb03f-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fb03f-144">説明</span><span class="sxs-lookup"><span data-stu-id="fb03f-144">description</span></span>|<span data-ttu-id="fb03f-145">String</span><span class="sxs-lookup"><span data-stu-id="fb03f-145">String</span></span>|<span data-ttu-id="fb03f-146">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="fb03f-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fb03f-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="fb03f-147">scopeMembers</span></span>|<span data-ttu-id="fb03f-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb03f-148">String collection</span></span>|<span data-ttu-id="fb03f-149">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="fb03f-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fb03f-150">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="fb03f-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="fb03f-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="fb03f-151">scopeType</span></span>|[<span data-ttu-id="fb03f-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="fb03f-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="fb03f-153">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb03f-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="fb03f-154">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="fb03f-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="fb03f-155">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="fb03f-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="fb03f-156">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="fb03f-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="fb03f-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fb03f-157">resourceScopes</span></span>|<span data-ttu-id="fb03f-158">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb03f-158">String collection</span></span>|<span data-ttu-id="fb03f-159">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="fb03f-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fb03f-160">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="fb03f-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb03f-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb03f-161">Relationships</span></span>
|<span data-ttu-id="fb03f-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb03f-162">Relationship</span></span>|<span data-ttu-id="fb03f-163">型</span><span class="sxs-lookup"><span data-stu-id="fb03f-163">Type</span></span>|<span data-ttu-id="fb03f-164">説明</span><span class="sxs-lookup"><span data-stu-id="fb03f-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb03f-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fb03f-165">roleDefinition</span></span>|[<span data-ttu-id="fb03f-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fb03f-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="fb03f-167">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="fb03f-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb03f-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb03f-168">JSON Representation</span></span>
<span data-ttu-id="fb03f-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb03f-169">Here is a JSON representation of the resource.</span></span>
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




