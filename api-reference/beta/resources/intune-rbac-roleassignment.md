---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cffebe54ba79d9b013068b9162f9e3a17447b15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566359"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="7f32f-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f32f-106">roleAssignment resource type</span></span>

> <span data-ttu-id="7f32f-107">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f32f-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f32f-108">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f32f-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f32f-109">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="7f32f-109">The Role Assignment resource.</span></span> <span data-ttu-id="7f32f-110">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="7f32f-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="7f32f-111">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="7f32f-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="7f32f-112">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7f32f-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="7f32f-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f32f-113">Methods</span></span>
|<span data-ttu-id="7f32f-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f32f-114">Method</span></span>|<span data-ttu-id="7f32f-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f32f-115">Return Type</span></span>|<span data-ttu-id="7f32f-116">説明</span><span class="sxs-lookup"><span data-stu-id="7f32f-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f32f-117">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="7f32f-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="7f32f-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7f32f-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7f32f-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7f32f-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="7f32f-120">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="7f32f-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="7f32f-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f32f-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="7f32f-122">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f32f-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="7f32f-123">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7f32f-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="7f32f-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f32f-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="7f32f-125">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f32f-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="7f32f-126">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="7f32f-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="7f32f-127">なし</span><span class="sxs-lookup"><span data-stu-id="7f32f-127">None</span></span>|<span data-ttu-id="7f32f-128">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7f32f-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="7f32f-129">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7f32f-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="7f32f-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f32f-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="7f32f-131">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f32f-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f32f-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f32f-132">Properties</span></span>
|<span data-ttu-id="7f32f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f32f-133">Property</span></span>|<span data-ttu-id="7f32f-134">型</span><span class="sxs-lookup"><span data-stu-id="7f32f-134">Type</span></span>|<span data-ttu-id="7f32f-135">説明</span><span class="sxs-lookup"><span data-stu-id="7f32f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f32f-136">id</span><span class="sxs-lookup"><span data-stu-id="7f32f-136">id</span></span>|<span data-ttu-id="7f32f-137">String</span><span class="sxs-lookup"><span data-stu-id="7f32f-137">String</span></span>|<span data-ttu-id="7f32f-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f32f-138">Key of the entity.</span></span> <span data-ttu-id="7f32f-139">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="7f32f-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7f32f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7f32f-140">displayName</span></span>|<span data-ttu-id="7f32f-141">String</span><span class="sxs-lookup"><span data-stu-id="7f32f-141">String</span></span>|<span data-ttu-id="7f32f-142">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="7f32f-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="7f32f-143">説明</span><span class="sxs-lookup"><span data-stu-id="7f32f-143">description</span></span>|<span data-ttu-id="7f32f-144">String</span><span class="sxs-lookup"><span data-stu-id="7f32f-144">String</span></span>|<span data-ttu-id="7f32f-145">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="7f32f-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="7f32f-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="7f32f-146">scopeMembers</span></span>|<span data-ttu-id="7f32f-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7f32f-147">String collection</span></span>|<span data-ttu-id="7f32f-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="7f32f-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7f32f-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="7f32f-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="7f32f-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="7f32f-150">scopeType</span></span>|[<span data-ttu-id="7f32f-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="7f32f-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="7f32f-152">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f32f-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="7f32f-153">既定の種類 ' resourcescope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="7f32f-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="7f32f-154">' alldevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f32f-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="7f32f-155">使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="7f32f-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="7f32f-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7f32f-156">resourceScopes</span></span>|<span data-ttu-id="7f32f-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7f32f-157">String collection</span></span>|<span data-ttu-id="7f32f-158">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="7f32f-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7f32f-159">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="7f32f-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f32f-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f32f-160">Relationships</span></span>
|<span data-ttu-id="7f32f-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f32f-161">Relationship</span></span>|<span data-ttu-id="7f32f-162">型</span><span class="sxs-lookup"><span data-stu-id="7f32f-162">Type</span></span>|<span data-ttu-id="7f32f-163">説明</span><span class="sxs-lookup"><span data-stu-id="7f32f-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f32f-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f32f-164">roleDefinition</span></span>|[<span data-ttu-id="7f32f-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f32f-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7f32f-166">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="7f32f-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f32f-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f32f-167">JSON Representation</span></span>
<span data-ttu-id="7f32f-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f32f-168">Here is a JSON representation of the resource.</span></span>
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





