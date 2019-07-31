---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c72b6ee403a4a0b06cd1181da584dbb7b4729f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967603"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="6bb44-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bb44-106">roleAssignment resource type</span></span>

> <span data-ttu-id="6bb44-107">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bb44-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bb44-108">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6bb44-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bb44-109">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="6bb44-109">The Role Assignment resource.</span></span> <span data-ttu-id="6bb44-110">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="6bb44-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="6bb44-111">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="6bb44-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="6bb44-112">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6bb44-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="6bb44-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bb44-113">Methods</span></span>
|<span data-ttu-id="6bb44-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bb44-114">Method</span></span>|<span data-ttu-id="6bb44-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6bb44-115">Return Type</span></span>|<span data-ttu-id="6bb44-116">説明</span><span class="sxs-lookup"><span data-stu-id="6bb44-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bb44-117">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="6bb44-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="6bb44-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6bb44-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="6bb44-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6bb44-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="6bb44-120">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="6bb44-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="6bb44-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bb44-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="6bb44-122">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6bb44-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="6bb44-123">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="6bb44-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="6bb44-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bb44-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="6bb44-125">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6bb44-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="6bb44-126">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="6bb44-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="6bb44-127">なし</span><span class="sxs-lookup"><span data-stu-id="6bb44-127">None</span></span>|<span data-ttu-id="6bb44-128">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6bb44-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="6bb44-129">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="6bb44-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="6bb44-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bb44-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="6bb44-131">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6bb44-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bb44-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bb44-132">Properties</span></span>
|<span data-ttu-id="6bb44-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bb44-133">Property</span></span>|<span data-ttu-id="6bb44-134">型</span><span class="sxs-lookup"><span data-stu-id="6bb44-134">Type</span></span>|<span data-ttu-id="6bb44-135">説明</span><span class="sxs-lookup"><span data-stu-id="6bb44-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bb44-136">id</span><span class="sxs-lookup"><span data-stu-id="6bb44-136">id</span></span>|<span data-ttu-id="6bb44-137">文字列</span><span class="sxs-lookup"><span data-stu-id="6bb44-137">String</span></span>|<span data-ttu-id="6bb44-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6bb44-138">Key of the entity.</span></span> <span data-ttu-id="6bb44-139">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="6bb44-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="6bb44-140">displayName</span><span class="sxs-lookup"><span data-stu-id="6bb44-140">displayName</span></span>|<span data-ttu-id="6bb44-141">String</span><span class="sxs-lookup"><span data-stu-id="6bb44-141">String</span></span>|<span data-ttu-id="6bb44-142">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="6bb44-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="6bb44-143">description</span><span class="sxs-lookup"><span data-stu-id="6bb44-143">description</span></span>|<span data-ttu-id="6bb44-144">String</span><span class="sxs-lookup"><span data-stu-id="6bb44-144">String</span></span>|<span data-ttu-id="6bb44-145">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="6bb44-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="6bb44-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="6bb44-146">scopeMembers</span></span>|<span data-ttu-id="6bb44-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6bb44-147">String collection</span></span>|<span data-ttu-id="6bb44-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="6bb44-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6bb44-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="6bb44-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="6bb44-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="6bb44-150">scopeType</span></span>|[<span data-ttu-id="6bb44-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="6bb44-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="6bb44-152">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bb44-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="6bb44-153">既定の種類 ' ResourceScope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="6bb44-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="6bb44-154">' AllDevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6bb44-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="6bb44-155">使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="6bb44-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="6bb44-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6bb44-156">resourceScopes</span></span>|<span data-ttu-id="6bb44-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6bb44-157">String collection</span></span>|<span data-ttu-id="6bb44-158">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="6bb44-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6bb44-159">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="6bb44-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bb44-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bb44-160">Relationships</span></span>
|<span data-ttu-id="6bb44-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bb44-161">Relationship</span></span>|<span data-ttu-id="6bb44-162">型</span><span class="sxs-lookup"><span data-stu-id="6bb44-162">Type</span></span>|<span data-ttu-id="6bb44-163">説明</span><span class="sxs-lookup"><span data-stu-id="6bb44-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bb44-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bb44-164">roleDefinition</span></span>|[<span data-ttu-id="6bb44-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bb44-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="6bb44-166">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="6bb44-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bb44-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bb44-167">JSON Representation</span></span>
<span data-ttu-id="6bb44-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6bb44-168">Here is a JSON representation of the resource.</span></span>
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





