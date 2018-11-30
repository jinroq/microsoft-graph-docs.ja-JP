---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
ms.openlocfilehash: 8af3c9778fefd2485948a48f1621c9d9e034c6db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022235"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="31de5-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31de5-106">roleAssignment resource type</span></span>

> <span data-ttu-id="31de5-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31de5-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31de5-108">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="31de5-108">The Role Assignment resource.</span></span> <span data-ttu-id="31de5-109">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="31de5-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="31de5-110">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="31de5-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="31de5-111">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="31de5-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="31de5-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="31de5-112">Methods</span></span>
|<span data-ttu-id="31de5-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="31de5-113">Method</span></span>|<span data-ttu-id="31de5-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31de5-114">Return Type</span></span>|<span data-ttu-id="31de5-115">説明</span><span class="sxs-lookup"><span data-stu-id="31de5-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31de5-116">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="31de5-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="31de5-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="31de5-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="31de5-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="31de5-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="31de5-119">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="31de5-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="31de5-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31de5-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31de5-121">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="31de5-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="31de5-122">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="31de5-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="31de5-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31de5-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31de5-124">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31de5-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="31de5-125">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="31de5-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="31de5-126">なし</span><span class="sxs-lookup"><span data-stu-id="31de5-126">None</span></span>|<span data-ttu-id="31de5-127">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="31de5-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="31de5-128">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="31de5-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="31de5-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31de5-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31de5-130">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31de5-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31de5-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31de5-131">Properties</span></span>
|<span data-ttu-id="31de5-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31de5-132">Property</span></span>|<span data-ttu-id="31de5-133">型</span><span class="sxs-lookup"><span data-stu-id="31de5-133">Type</span></span>|<span data-ttu-id="31de5-134">説明</span><span class="sxs-lookup"><span data-stu-id="31de5-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31de5-135">id</span><span class="sxs-lookup"><span data-stu-id="31de5-135">id</span></span>|<span data-ttu-id="31de5-136">String</span><span class="sxs-lookup"><span data-stu-id="31de5-136">String</span></span>|<span data-ttu-id="31de5-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31de5-137">Key of the entity.</span></span> <span data-ttu-id="31de5-138">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="31de5-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="31de5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="31de5-139">displayName</span></span>|<span data-ttu-id="31de5-140">String</span><span class="sxs-lookup"><span data-stu-id="31de5-140">String</span></span>|<span data-ttu-id="31de5-141">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="31de5-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="31de5-142">説明</span><span class="sxs-lookup"><span data-stu-id="31de5-142">description</span></span>|<span data-ttu-id="31de5-143">String</span><span class="sxs-lookup"><span data-stu-id="31de5-143">String</span></span>|<span data-ttu-id="31de5-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="31de5-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="31de5-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="31de5-145">resourceScopes</span></span>|<span data-ttu-id="31de5-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="31de5-146">String collection</span></span>|<span data-ttu-id="31de5-147">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="31de5-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="31de5-148">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="31de5-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31de5-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31de5-149">Relationships</span></span>
|<span data-ttu-id="31de5-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31de5-150">Relationship</span></span>|<span data-ttu-id="31de5-151">型</span><span class="sxs-lookup"><span data-stu-id="31de5-151">Type</span></span>|<span data-ttu-id="31de5-152">説明</span><span class="sxs-lookup"><span data-stu-id="31de5-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31de5-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31de5-153">roleDefinition</span></span>|[<span data-ttu-id="31de5-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31de5-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="31de5-155">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="31de5-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31de5-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31de5-156">JSON Representation</span></span>
<span data-ttu-id="31de5-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31de5-157">Here is a JSON representation of the resource.</span></span>
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



