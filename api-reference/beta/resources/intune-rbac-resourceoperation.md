---
title: resourceOperation リソース タイプ
description: テナント組織の役割ベースのアクセス制御 (RBAC) シナリオをサポートする Intune (REST) 用 Microsoft Graph API の resourceoperation リソース (エンティティ) について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a299247815993a6ac1e99fe11ecead7ab66e2f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165003"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="68fdd-103">resourceOperation リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="68fdd-103">resourceOperation resource type</span></span>

> <span data-ttu-id="68fdd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68fdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68fdd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68fdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68fdd-106">Intune リソース (またはエンティティ) で実行できる操作またはアクションを定義します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-106">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="68fdd-107">一般的な操作は Read、Delete、Update、Create です。</span><span class="sxs-lookup"><span data-stu-id="68fdd-107">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="68fdd-108">これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-108">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="68fdd-109">場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="68fdd-109">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="68fdd-110">たとえば、Assign 操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="68fdd-110">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="68fdd-111">組み込みのロールについては、リソース操作を変更できません。これは、Intune リソース (またはエンティティ) に実行できる操作またはアクションを定義します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-111">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="68fdd-112">一般的な操作は Get、List、Delete、Update、Create です。</span><span class="sxs-lookup"><span data-stu-id="68fdd-112">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="68fdd-113">これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-113">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="68fdd-114">場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="68fdd-114">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="68fdd-115">たとえば、「Assign」操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="68fdd-115">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="68fdd-116">組み込みのロールについては、リソース操作を変更できません。</span><span class="sxs-lookup"><span data-stu-id="68fdd-116">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="68fdd-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="68fdd-117">Methods</span></span>
|<span data-ttu-id="68fdd-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="68fdd-118">Method</span></span>|<span data-ttu-id="68fdd-119">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68fdd-119">Return Type</span></span>|<span data-ttu-id="68fdd-120">説明</span><span class="sxs-lookup"><span data-stu-id="68fdd-120">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68fdd-121">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="68fdd-121">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="68fdd-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="68fdd-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="68fdd-123">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="68fdd-123">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="68fdd-124">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-124">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="68fdd-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="68fdd-126">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68fdd-126">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="68fdd-127">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-127">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="68fdd-128">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-128">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="68fdd-129">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-129">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="68fdd-130">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-130">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="68fdd-131">なし</span><span class="sxs-lookup"><span data-stu-id="68fdd-131">None</span></span>|<span data-ttu-id="68fdd-132">[resourceOperation](../resources/intune-rbac-resourceoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-132">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="68fdd-133">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-133">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="68fdd-134">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68fdd-134">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="68fdd-135">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-135">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="68fdd-136">getScopesForUser 関数</span><span class="sxs-lookup"><span data-stu-id="68fdd-136">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="68fdd-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="68fdd-137">String collection</span></span>|<span data-ttu-id="68fdd-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="68fdd-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="68fdd-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68fdd-139">Properties</span></span>
|<span data-ttu-id="68fdd-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68fdd-140">Property</span></span>|<span data-ttu-id="68fdd-141">型</span><span class="sxs-lookup"><span data-stu-id="68fdd-141">Type</span></span>|<span data-ttu-id="68fdd-142">説明</span><span class="sxs-lookup"><span data-stu-id="68fdd-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68fdd-143">id</span><span class="sxs-lookup"><span data-stu-id="68fdd-143">id</span></span>|<span data-ttu-id="68fdd-144">文字列</span><span class="sxs-lookup"><span data-stu-id="68fdd-144">String</span></span>|<span data-ttu-id="68fdd-145">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="68fdd-145">Key of the Resource Operation.</span></span> <span data-ttu-id="68fdd-146">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="68fdd-146">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="68fdd-147">リソース</span><span class="sxs-lookup"><span data-stu-id="68fdd-147">resource</span></span>|<span data-ttu-id="68fdd-148">String</span><span class="sxs-lookup"><span data-stu-id="68fdd-148">String</span></span>|<span data-ttu-id="68fdd-149">この操作が属するリソースカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="68fdd-149">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="68fdd-150">resourceName</span><span class="sxs-lookup"><span data-stu-id="68fdd-150">resourceName</span></span>|<span data-ttu-id="68fdd-151">String</span><span class="sxs-lookup"><span data-stu-id="68fdd-151">String</span></span>|<span data-ttu-id="68fdd-152">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="68fdd-152">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="68fdd-153">actionName</span><span class="sxs-lookup"><span data-stu-id="68fdd-153">actionName</span></span>|<span data-ttu-id="68fdd-154">String</span><span class="sxs-lookup"><span data-stu-id="68fdd-154">String</span></span>|<span data-ttu-id="68fdd-155">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="68fdd-155">Type of action this operation is going to perform.</span></span> <span data-ttu-id="68fdd-156">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="68fdd-156">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="68fdd-157">説明</span><span class="sxs-lookup"><span data-stu-id="68fdd-157">description</span></span>|<span data-ttu-id="68fdd-158">String</span><span class="sxs-lookup"><span data-stu-id="68fdd-158">String</span></span>|<span data-ttu-id="68fdd-159">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="68fdd-159">Description of the resource operation.</span></span> <span data-ttu-id="68fdd-160">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="68fdd-160">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="68fdd-161">enabledforscopevalidation</span><span class="sxs-lookup"><span data-stu-id="68fdd-161">enabledForScopeValidation</span></span>|<span data-ttu-id="68fdd-162">ブール値</span><span class="sxs-lookup"><span data-stu-id="68fdd-162">Boolean</span></span>|<span data-ttu-id="68fdd-163">権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="68fdd-163">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68fdd-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68fdd-164">Relationships</span></span>
<span data-ttu-id="68fdd-165">なし</span><span class="sxs-lookup"><span data-stu-id="68fdd-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68fdd-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68fdd-166">JSON Representation</span></span>
<span data-ttu-id="68fdd-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68fdd-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```




