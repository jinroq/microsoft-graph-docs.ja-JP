---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258430"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="940b3-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="940b3-106">roleAssignment resource type</span></span>

> <span data-ttu-id="940b3-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="940b3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940b3-108">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="940b3-108">The Role Assignment resource.</span></span> <span data-ttu-id="940b3-109">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="940b3-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="940b3-110">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="940b3-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="940b3-111">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="940b3-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="940b3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="940b3-112">Methods</span></span>
|<span data-ttu-id="940b3-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="940b3-113">Method</span></span>|<span data-ttu-id="940b3-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="940b3-114">Return Type</span></span>|<span data-ttu-id="940b3-115">説明</span><span class="sxs-lookup"><span data-stu-id="940b3-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="940b3-116">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="940b3-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="940b3-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="940b3-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="940b3-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="940b3-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="940b3-119">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="940b3-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="940b3-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="940b3-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="940b3-121">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="940b3-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="940b3-122">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="940b3-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="940b3-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="940b3-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="940b3-124">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="940b3-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="940b3-125">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="940b3-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="940b3-126">なし</span><span class="sxs-lookup"><span data-stu-id="940b3-126">None</span></span>|<span data-ttu-id="940b3-127">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="940b3-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="940b3-128">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="940b3-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="940b3-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="940b3-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="940b3-130">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="940b3-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="940b3-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="940b3-131">Properties</span></span>
|<span data-ttu-id="940b3-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="940b3-132">Property</span></span>|<span data-ttu-id="940b3-133">型</span><span class="sxs-lookup"><span data-stu-id="940b3-133">Type</span></span>|<span data-ttu-id="940b3-134">説明</span><span class="sxs-lookup"><span data-stu-id="940b3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940b3-135">id</span><span class="sxs-lookup"><span data-stu-id="940b3-135">id</span></span>|<span data-ttu-id="940b3-136">String</span><span class="sxs-lookup"><span data-stu-id="940b3-136">String</span></span>|<span data-ttu-id="940b3-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="940b3-137">Key of the entity.</span></span> <span data-ttu-id="940b3-138">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="940b3-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="940b3-139">displayName</span><span class="sxs-lookup"><span data-stu-id="940b3-139">displayName</span></span>|<span data-ttu-id="940b3-140">String</span><span class="sxs-lookup"><span data-stu-id="940b3-140">String</span></span>|<span data-ttu-id="940b3-141">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="940b3-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="940b3-142">説明</span><span class="sxs-lookup"><span data-stu-id="940b3-142">description</span></span>|<span data-ttu-id="940b3-143">String</span><span class="sxs-lookup"><span data-stu-id="940b3-143">String</span></span>|<span data-ttu-id="940b3-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="940b3-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="940b3-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="940b3-145">resourceScopes</span></span>|<span data-ttu-id="940b3-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="940b3-146">String collection</span></span>|<span data-ttu-id="940b3-147">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="940b3-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="940b3-148">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="940b3-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="940b3-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="940b3-149">Relationships</span></span>
|<span data-ttu-id="940b3-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="940b3-150">Relationship</span></span>|<span data-ttu-id="940b3-151">型</span><span class="sxs-lookup"><span data-stu-id="940b3-151">Type</span></span>|<span data-ttu-id="940b3-152">説明</span><span class="sxs-lookup"><span data-stu-id="940b3-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940b3-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="940b3-153">roleDefinition</span></span>|[<span data-ttu-id="940b3-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="940b3-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="940b3-155">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="940b3-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="940b3-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="940b3-156">JSON Representation</span></span>
<span data-ttu-id="940b3-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="940b3-157">Here is a JSON representation of the resource.</span></span>
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
  "resourceScopes": [
    "String"
  ]
}
```



