---
title: deviceAndAppManagementRoleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfbb4e3b51f56e447ba69caefbf2b0b5226a5d4f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264086"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="73c0a-106">deviceAndAppManagementRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73c0a-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="73c0a-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73c0a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73c0a-108">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="73c0a-108">The Role Assignment resource.</span></span> <span data-ttu-id="73c0a-109">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="73c0a-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="73c0a-110">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="73c0a-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="73c0a-111">カスタムおよび組み込みのロールに適用されます。</span><span class="sxs-lookup"><span data-stu-id="73c0a-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="73c0a-112">[roleAssignment](../resources/intune-rbac-roleassignment.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="73c0a-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="73c0a-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="73c0a-113">Methods</span></span>
|<span data-ttu-id="73c0a-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="73c0a-114">Method</span></span>|<span data-ttu-id="73c0a-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="73c0a-115">Return Type</span></span>|<span data-ttu-id="73c0a-116">説明</span><span class="sxs-lookup"><span data-stu-id="73c0a-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73c0a-117">List deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="73c0a-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="73c0a-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="73c0a-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="73c0a-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="73c0a-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="73c0a-120">Get deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="73c0a-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="73c0a-122">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="73c0a-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="73c0a-123">Create deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="73c0a-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="73c0a-125">新しい [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="73c0a-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="73c0a-126">Delete deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="73c0a-127">なし</span><span class="sxs-lookup"><span data-stu-id="73c0a-127">None</span></span>|<span data-ttu-id="73c0a-128">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="73c0a-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="73c0a-129">Update deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="73c0a-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73c0a-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="73c0a-131">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="73c0a-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73c0a-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73c0a-132">Properties</span></span>
|<span data-ttu-id="73c0a-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73c0a-133">Property</span></span>|<span data-ttu-id="73c0a-134">型</span><span class="sxs-lookup"><span data-stu-id="73c0a-134">Type</span></span>|<span data-ttu-id="73c0a-135">説明</span><span class="sxs-lookup"><span data-stu-id="73c0a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c0a-136">id</span><span class="sxs-lookup"><span data-stu-id="73c0a-136">id</span></span>|<span data-ttu-id="73c0a-137">String</span><span class="sxs-lookup"><span data-stu-id="73c0a-137">String</span></span>|<span data-ttu-id="73c0a-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="73c0a-138">Key of the entity.</span></span> <span data-ttu-id="73c0a-139">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="73c0a-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="73c0a-140">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c0a-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="73c0a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="73c0a-141">displayName</span></span>|<span data-ttu-id="73c0a-142">String</span><span class="sxs-lookup"><span data-stu-id="73c0a-142">String</span></span>|<span data-ttu-id="73c0a-143">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="73c0a-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="73c0a-144">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c0a-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="73c0a-145">説明</span><span class="sxs-lookup"><span data-stu-id="73c0a-145">description</span></span>|<span data-ttu-id="73c0a-146">String</span><span class="sxs-lookup"><span data-stu-id="73c0a-146">String</span></span>|<span data-ttu-id="73c0a-147">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="73c0a-147">Description of the Role Assignment.</span></span> <span data-ttu-id="73c0a-148">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c0a-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="73c0a-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="73c0a-149">resourceScopes</span></span>|<span data-ttu-id="73c0a-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="73c0a-150">String collection</span></span>|<span data-ttu-id="73c0a-151">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="73c0a-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="73c0a-152">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="73c0a-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="73c0a-153">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c0a-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="73c0a-154">members</span><span class="sxs-lookup"><span data-stu-id="73c0a-154">members</span></span>|<span data-ttu-id="73c0a-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="73c0a-155">String collection</span></span>|<span data-ttu-id="73c0a-156">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="73c0a-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="73c0a-157">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="73c0a-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73c0a-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73c0a-158">Relationships</span></span>
|<span data-ttu-id="73c0a-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73c0a-159">Relationship</span></span>|<span data-ttu-id="73c0a-160">型</span><span class="sxs-lookup"><span data-stu-id="73c0a-160">Type</span></span>|<span data-ttu-id="73c0a-161">説明</span><span class="sxs-lookup"><span data-stu-id="73c0a-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c0a-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c0a-162">roleDefinition</span></span>|[<span data-ttu-id="73c0a-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c0a-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="73c0a-164">対象割り当てが含まれるロール定義。</span><span class="sxs-lookup"><span data-stu-id="73c0a-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="73c0a-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="73c0a-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73c0a-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73c0a-166">JSON Representation</span></span>
<span data-ttu-id="73c0a-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73c0a-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



