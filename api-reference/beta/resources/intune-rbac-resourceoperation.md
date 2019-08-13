---
title: resourceOperation リソース タイプ
description: ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b83ad1c902e8455d42ae0e9805bf6881b49ef3b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369284"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="415ce-103">resourceOperation リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="415ce-103">resourceOperation resource type</span></span>

> <span data-ttu-id="415ce-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="415ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="415ce-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="415ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="415ce-106">ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。</span><span class="sxs-lookup"><span data-stu-id="415ce-106">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="415ce-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="415ce-107">Methods</span></span>
|<span data-ttu-id="415ce-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="415ce-108">Method</span></span>|<span data-ttu-id="415ce-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="415ce-109">Return Type</span></span>|<span data-ttu-id="415ce-110">説明</span><span class="sxs-lookup"><span data-stu-id="415ce-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="415ce-111">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="415ce-111">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="415ce-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="415ce-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="415ce-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="415ce-113">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="415ce-114">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-114">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="415ce-115">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-115">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="415ce-116">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="415ce-116">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="415ce-117">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-117">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="415ce-118">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-118">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="415ce-119">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="415ce-119">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="415ce-120">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-120">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="415ce-121">なし</span><span class="sxs-lookup"><span data-stu-id="415ce-121">None</span></span>|<span data-ttu-id="415ce-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="415ce-122">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="415ce-123">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-123">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="415ce-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="415ce-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="415ce-125">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="415ce-125">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="415ce-126">getScopesForUser 関数</span><span class="sxs-lookup"><span data-stu-id="415ce-126">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="415ce-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="415ce-127">String collection</span></span>|<span data-ttu-id="415ce-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="415ce-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="415ce-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="415ce-129">Properties</span></span>
|<span data-ttu-id="415ce-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="415ce-130">Property</span></span>|<span data-ttu-id="415ce-131">型</span><span class="sxs-lookup"><span data-stu-id="415ce-131">Type</span></span>|<span data-ttu-id="415ce-132">説明</span><span class="sxs-lookup"><span data-stu-id="415ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415ce-133">id</span><span class="sxs-lookup"><span data-stu-id="415ce-133">id</span></span>|<span data-ttu-id="415ce-134">String</span><span class="sxs-lookup"><span data-stu-id="415ce-134">String</span></span>|<span data-ttu-id="415ce-135">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="415ce-135">Key of the Resource Operation.</span></span> <span data-ttu-id="415ce-136">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="415ce-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="415ce-137">リソース</span><span class="sxs-lookup"><span data-stu-id="415ce-137">resource</span></span>|<span data-ttu-id="415ce-138">String</span><span class="sxs-lookup"><span data-stu-id="415ce-138">String</span></span>|<span data-ttu-id="415ce-139">この操作が属するリソースカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="415ce-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="415ce-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="415ce-140">resourceName</span></span>|<span data-ttu-id="415ce-141">String</span><span class="sxs-lookup"><span data-stu-id="415ce-141">String</span></span>|<span data-ttu-id="415ce-142">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="415ce-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="415ce-143">actionName</span><span class="sxs-lookup"><span data-stu-id="415ce-143">actionName</span></span>|<span data-ttu-id="415ce-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="415ce-144">String</span></span>|<span data-ttu-id="415ce-145">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="415ce-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="415ce-146">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="415ce-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="415ce-147">description</span><span class="sxs-lookup"><span data-stu-id="415ce-147">description</span></span>|<span data-ttu-id="415ce-148">String</span><span class="sxs-lookup"><span data-stu-id="415ce-148">String</span></span>|<span data-ttu-id="415ce-149">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="415ce-149">Description of the resource operation.</span></span> <span data-ttu-id="415ce-150">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="415ce-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="415ce-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="415ce-151">enabledForScopeValidation</span></span>|<span data-ttu-id="415ce-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="415ce-152">Boolean</span></span>|<span data-ttu-id="415ce-153">権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="415ce-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="415ce-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="415ce-154">Relationships</span></span>
<span data-ttu-id="415ce-155">なし</span><span class="sxs-lookup"><span data-stu-id="415ce-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="415ce-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="415ce-156">JSON Representation</span></span>
<span data-ttu-id="415ce-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="415ce-157">Here is a JSON representation of the resource.</span></span>
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



