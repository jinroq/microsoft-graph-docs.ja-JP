---
title: resourceOperation リソース タイプ
description: ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceoperation リソース (エンティティ) について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c203b47235d94a3742c5cb0cee401d824feafb46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553989"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="8f2aa-103">resourceOperation リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8f2aa-103">resourceOperation resource type</span></span>

> <span data-ttu-id="8f2aa-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f2aa-105">Intune リソース (またはエンティティ) で実行できる操作またはアクションを定義します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-105">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="8f2aa-106">一般的な操作は Read、Delete、Update、Create です。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-106">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="8f2aa-107">これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-107">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="8f2aa-108">場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-108">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="8f2aa-109">たとえば、Assign 操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-109">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="8f2aa-110">組み込みのロールについては、リソース操作を変更できません。これは、Intune リソース (またはエンティティ) に実行できる操作またはアクションを定義します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-110">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="8f2aa-111">一般的な操作は Get、List、Delete、Update、Create です。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-111">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="8f2aa-112">これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-112">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="8f2aa-113">場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-113">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="8f2aa-114">たとえば、「Assign」操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-114">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="8f2aa-115">組み込みのロールについては、リソース操作を変更できません。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-115">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="8f2aa-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f2aa-116">Methods</span></span>
|<span data-ttu-id="8f2aa-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f2aa-117">Method</span></span>|<span data-ttu-id="8f2aa-118">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f2aa-118">Return Type</span></span>|<span data-ttu-id="8f2aa-119">説明</span><span class="sxs-lookup"><span data-stu-id="8f2aa-119">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f2aa-120">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="8f2aa-120">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="8f2aa-121">[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8f2aa-121">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="8f2aa-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-122">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="8f2aa-123">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-123">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="8f2aa-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8f2aa-125">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-125">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="8f2aa-126">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-126">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="8f2aa-127">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-127">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8f2aa-128">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-128">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="8f2aa-129">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-129">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="8f2aa-130">なし</span><span class="sxs-lookup"><span data-stu-id="8f2aa-130">None</span></span>|<span data-ttu-id="8f2aa-131">[resourceOperation](../resources/intune-rbac-resourceoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-131">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="8f2aa-132">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-132">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="8f2aa-133">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8f2aa-133">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8f2aa-134">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-134">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f2aa-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f2aa-135">Properties</span></span>
|<span data-ttu-id="8f2aa-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f2aa-136">Property</span></span>|<span data-ttu-id="8f2aa-137">型</span><span class="sxs-lookup"><span data-stu-id="8f2aa-137">Type</span></span>|<span data-ttu-id="8f2aa-138">説明</span><span class="sxs-lookup"><span data-stu-id="8f2aa-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f2aa-139">id</span><span class="sxs-lookup"><span data-stu-id="8f2aa-139">id</span></span>|<span data-ttu-id="8f2aa-140">String</span><span class="sxs-lookup"><span data-stu-id="8f2aa-140">String</span></span>|<span data-ttu-id="8f2aa-141">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-141">Key of the Resource Operation.</span></span> <span data-ttu-id="8f2aa-142">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-142">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="8f2aa-143">resourceName</span><span class="sxs-lookup"><span data-stu-id="8f2aa-143">resourceName</span></span>|<span data-ttu-id="8f2aa-144">String</span><span class="sxs-lookup"><span data-stu-id="8f2aa-144">String</span></span>|<span data-ttu-id="8f2aa-145">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-145">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="8f2aa-146">actionName</span><span class="sxs-lookup"><span data-stu-id="8f2aa-146">actionName</span></span>|<span data-ttu-id="8f2aa-147">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8f2aa-147">String</span></span>|<span data-ttu-id="8f2aa-148">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-148">Type of action this operation is going to perform.</span></span> <span data-ttu-id="8f2aa-149">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-149">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="8f2aa-150">description</span><span class="sxs-lookup"><span data-stu-id="8f2aa-150">description</span></span>|<span data-ttu-id="8f2aa-151">String</span><span class="sxs-lookup"><span data-stu-id="8f2aa-151">String</span></span>|<span data-ttu-id="8f2aa-152">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-152">Description of the resource operation.</span></span> <span data-ttu-id="8f2aa-153">Azure Portal で操作にカーソルを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-153">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f2aa-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f2aa-154">Relationships</span></span>
<span data-ttu-id="8f2aa-155">なし</span><span class="sxs-lookup"><span data-stu-id="8f2aa-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f2aa-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f2aa-156">JSON Representation</span></span>
<span data-ttu-id="8f2aa-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f2aa-157">Here is a JSON representation of the resource.</span></span>
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
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```



