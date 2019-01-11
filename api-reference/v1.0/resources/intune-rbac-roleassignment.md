---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8506b87975b69f90cf561e776e557bb472f1ffd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846152"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="bcf0e-106">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcf0e-106">roleAssignment resource type</span></span>

> <span data-ttu-id="bcf0e-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcf0e-108">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-108">The Role Assignment resource.</span></span> <span data-ttu-id="bcf0e-109">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="bcf0e-110">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="bcf0e-111">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="bcf0e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcf0e-112">Methods</span></span>
|<span data-ttu-id="bcf0e-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcf0e-113">Method</span></span>|<span data-ttu-id="bcf0e-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bcf0e-114">Return Type</span></span>|<span data-ttu-id="bcf0e-115">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0e-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcf0e-116">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="bcf0e-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="bcf0e-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0e-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="bcf0e-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="bcf0e-119">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="bcf0e-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="bcf0e-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="bcf0e-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="bcf0e-121">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="bcf0e-122">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="bcf0e-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="bcf0e-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="bcf0e-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="bcf0e-124">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="bcf0e-125">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="bcf0e-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="bcf0e-126">なし</span><span class="sxs-lookup"><span data-stu-id="bcf0e-126">None</span></span>|<span data-ttu-id="bcf0e-127">[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="bcf0e-128">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="bcf0e-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="bcf0e-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="bcf0e-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="bcf0e-130">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcf0e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcf0e-131">Properties</span></span>
|<span data-ttu-id="bcf0e-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcf0e-132">Property</span></span>|<span data-ttu-id="bcf0e-133">種類</span><span class="sxs-lookup"><span data-stu-id="bcf0e-133">Type</span></span>|<span data-ttu-id="bcf0e-134">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf0e-135">ID</span><span class="sxs-lookup"><span data-stu-id="bcf0e-135">id</span></span>|<span data-ttu-id="bcf0e-136">String</span><span class="sxs-lookup"><span data-stu-id="bcf0e-136">String</span></span>|<span data-ttu-id="bcf0e-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-137">Key of the entity.</span></span> <span data-ttu-id="bcf0e-138">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="bcf0e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bcf0e-139">displayName</span></span>|<span data-ttu-id="bcf0e-140">String</span><span class="sxs-lookup"><span data-stu-id="bcf0e-140">String</span></span>|<span data-ttu-id="bcf0e-141">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="bcf0e-142">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0e-142">description</span></span>|<span data-ttu-id="bcf0e-143">String</span><span class="sxs-lookup"><span data-stu-id="bcf0e-143">String</span></span>|<span data-ttu-id="bcf0e-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="bcf0e-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="bcf0e-145">resourceScopes</span></span>|<span data-ttu-id="bcf0e-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0e-146">String collection</span></span>|<span data-ttu-id="bcf0e-147">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bcf0e-148">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcf0e-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcf0e-149">Relationships</span></span>
|<span data-ttu-id="bcf0e-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcf0e-150">Relationship</span></span>|<span data-ttu-id="bcf0e-151">型</span><span class="sxs-lookup"><span data-stu-id="bcf0e-151">Type</span></span>|<span data-ttu-id="bcf0e-152">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0e-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf0e-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bcf0e-153">roleDefinition</span></span>|[<span data-ttu-id="bcf0e-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bcf0e-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="bcf0e-155">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcf0e-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcf0e-156">JSON Representation</span></span>
<span data-ttu-id="bcf0e-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcf0e-157">Here is a JSON representation of the resource.</span></span>
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



