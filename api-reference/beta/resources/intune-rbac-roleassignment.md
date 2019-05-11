---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d2ad221405546aad502ec71a4b7403caa9306e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940079"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="ba031-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba031-106">roleAssignment resource type</span></span>

> <span data-ttu-id="ba031-107">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba031-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba031-108">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba031-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba031-109">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="ba031-109">The Role Assignment resource.</span></span> <span data-ttu-id="ba031-110">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="ba031-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="ba031-111">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="ba031-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="ba031-112">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ba031-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ba031-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba031-113">Methods</span></span>
|<span data-ttu-id="ba031-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba031-114">Method</span></span>|<span data-ttu-id="ba031-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ba031-115">Return Type</span></span>|<span data-ttu-id="ba031-116">説明</span><span class="sxs-lookup"><span data-stu-id="ba031-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba031-117">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ba031-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="ba031-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ba031-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="ba031-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ba031-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="ba031-120">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="ba031-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="ba031-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ba031-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ba031-122">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ba031-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ba031-123">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ba031-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="ba031-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ba031-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ba031-125">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ba031-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ba031-126">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="ba031-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="ba031-127">なし</span><span class="sxs-lookup"><span data-stu-id="ba031-127">None</span></span>|<span data-ttu-id="ba031-128">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ba031-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="ba031-129">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="ba031-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="ba031-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ba031-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ba031-131">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ba031-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba031-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba031-132">Properties</span></span>
|<span data-ttu-id="ba031-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba031-133">Property</span></span>|<span data-ttu-id="ba031-134">種類</span><span class="sxs-lookup"><span data-stu-id="ba031-134">Type</span></span>|<span data-ttu-id="ba031-135">説明</span><span class="sxs-lookup"><span data-stu-id="ba031-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba031-136">id</span><span class="sxs-lookup"><span data-stu-id="ba031-136">id</span></span>|<span data-ttu-id="ba031-137">文字列</span><span class="sxs-lookup"><span data-stu-id="ba031-137">String</span></span>|<span data-ttu-id="ba031-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ba031-138">Key of the entity.</span></span> <span data-ttu-id="ba031-139">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="ba031-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ba031-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ba031-140">displayName</span></span>|<span data-ttu-id="ba031-141">String</span><span class="sxs-lookup"><span data-stu-id="ba031-141">String</span></span>|<span data-ttu-id="ba031-142">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="ba031-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="ba031-143">description</span><span class="sxs-lookup"><span data-stu-id="ba031-143">description</span></span>|<span data-ttu-id="ba031-144">String</span><span class="sxs-lookup"><span data-stu-id="ba031-144">String</span></span>|<span data-ttu-id="ba031-145">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="ba031-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="ba031-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="ba031-146">scopeMembers</span></span>|<span data-ttu-id="ba031-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ba031-147">String collection</span></span>|<span data-ttu-id="ba031-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="ba031-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ba031-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="ba031-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="ba031-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="ba031-150">scopeType</span></span>|[<span data-ttu-id="ba031-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="ba031-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="ba031-152">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba031-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="ba031-153">既定の種類 ' ResourceScope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="ba031-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="ba031-154">' AllDevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba031-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="ba031-155">使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="ba031-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="ba031-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ba031-156">resourceScopes</span></span>|<span data-ttu-id="ba031-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ba031-157">String collection</span></span>|<span data-ttu-id="ba031-158">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="ba031-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ba031-159">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="ba031-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba031-160">関係</span><span class="sxs-lookup"><span data-stu-id="ba031-160">Relationships</span></span>
|<span data-ttu-id="ba031-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ba031-161">Relationship</span></span>|<span data-ttu-id="ba031-162">型</span><span class="sxs-lookup"><span data-stu-id="ba031-162">Type</span></span>|<span data-ttu-id="ba031-163">説明</span><span class="sxs-lookup"><span data-stu-id="ba031-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba031-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ba031-164">roleDefinition</span></span>|[<span data-ttu-id="ba031-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ba031-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="ba031-166">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="ba031-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba031-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba031-167">JSON Representation</span></span>
<span data-ttu-id="ba031-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba031-168">Here is a JSON representation of the resource.</span></span>
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




