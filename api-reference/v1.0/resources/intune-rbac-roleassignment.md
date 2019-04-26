---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554038"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="f7d0a-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7d0a-106">roleAssignment resource type</span></span>

> <span data-ttu-id="f7d0a-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d0a-108">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-108">The Role Assignment resource.</span></span> <span data-ttu-id="f7d0a-109">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="f7d0a-110">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="f7d0a-111">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="f7d0a-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7d0a-112">Methods</span></span>
|<span data-ttu-id="f7d0a-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7d0a-113">Method</span></span>|<span data-ttu-id="f7d0a-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f7d0a-114">Return Type</span></span>|<span data-ttu-id="f7d0a-115">説明</span><span class="sxs-lookup"><span data-stu-id="f7d0a-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7d0a-116">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="f7d0a-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="f7d0a-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f7d0a-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="f7d0a-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="f7d0a-119">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="f7d0a-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="f7d0a-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f7d0a-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f7d0a-121">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="f7d0a-122">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="f7d0a-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="f7d0a-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f7d0a-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f7d0a-124">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="f7d0a-125">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="f7d0a-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="f7d0a-126">なし</span><span class="sxs-lookup"><span data-stu-id="f7d0a-126">None</span></span>|<span data-ttu-id="f7d0a-127">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="f7d0a-128">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="f7d0a-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="f7d0a-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f7d0a-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f7d0a-130">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7d0a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7d0a-131">Properties</span></span>
|<span data-ttu-id="f7d0a-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7d0a-132">Property</span></span>|<span data-ttu-id="f7d0a-133">型</span><span class="sxs-lookup"><span data-stu-id="f7d0a-133">Type</span></span>|<span data-ttu-id="f7d0a-134">説明</span><span class="sxs-lookup"><span data-stu-id="f7d0a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d0a-135">id</span><span class="sxs-lookup"><span data-stu-id="f7d0a-135">id</span></span>|<span data-ttu-id="f7d0a-136">String</span><span class="sxs-lookup"><span data-stu-id="f7d0a-136">String</span></span>|<span data-ttu-id="f7d0a-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-137">Key of the entity.</span></span> <span data-ttu-id="f7d0a-138">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f7d0a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f7d0a-139">displayName</span></span>|<span data-ttu-id="f7d0a-140">String</span><span class="sxs-lookup"><span data-stu-id="f7d0a-140">String</span></span>|<span data-ttu-id="f7d0a-141">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="f7d0a-142">description</span><span class="sxs-lookup"><span data-stu-id="f7d0a-142">description</span></span>|<span data-ttu-id="f7d0a-143">String</span><span class="sxs-lookup"><span data-stu-id="f7d0a-143">String</span></span>|<span data-ttu-id="f7d0a-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="f7d0a-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f7d0a-145">resourceScopes</span></span>|<span data-ttu-id="f7d0a-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f7d0a-146">String collection</span></span>|<span data-ttu-id="f7d0a-147">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f7d0a-148">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d0a-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7d0a-149">Relationships</span></span>
|<span data-ttu-id="f7d0a-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7d0a-150">Relationship</span></span>|<span data-ttu-id="f7d0a-151">型</span><span class="sxs-lookup"><span data-stu-id="f7d0a-151">Type</span></span>|<span data-ttu-id="f7d0a-152">説明</span><span class="sxs-lookup"><span data-stu-id="f7d0a-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d0a-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f7d0a-153">roleDefinition</span></span>|[<span data-ttu-id="f7d0a-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f7d0a-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="f7d0a-155">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7d0a-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7d0a-156">JSON Representation</span></span>
<span data-ttu-id="f7d0a-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7d0a-157">Here is a JSON representation of the resource.</span></span>
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



