---
title: resourceOperation リソース タイプ
description: ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2ac5cdcfbf444a0cc8642da16ca93aac9ccca65
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993579"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="399cd-103">resourceOperation リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="399cd-103">resourceOperation resource type</span></span>

> <span data-ttu-id="399cd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="399cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="399cd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="399cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="399cd-106">ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。</span><span class="sxs-lookup"><span data-stu-id="399cd-106">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="399cd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="399cd-107">Methods</span></span>
|<span data-ttu-id="399cd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="399cd-108">Method</span></span>|<span data-ttu-id="399cd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="399cd-109">Return Type</span></span>|<span data-ttu-id="399cd-110">説明</span><span class="sxs-lookup"><span data-stu-id="399cd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="399cd-111">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="399cd-111">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="399cd-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="399cd-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="399cd-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="399cd-113">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="399cd-114">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-114">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="399cd-115">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-115">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="399cd-116">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="399cd-116">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="399cd-117">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-117">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="399cd-118">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-118">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="399cd-119">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="399cd-119">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="399cd-120">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-120">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="399cd-121">なし</span><span class="sxs-lookup"><span data-stu-id="399cd-121">None</span></span>|<span data-ttu-id="399cd-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="399cd-122">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="399cd-123">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-123">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="399cd-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="399cd-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="399cd-125">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="399cd-125">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="399cd-126">getScopesForUser 関数</span><span class="sxs-lookup"><span data-stu-id="399cd-126">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="399cd-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="399cd-127">String collection</span></span>|<span data-ttu-id="399cd-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="399cd-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="399cd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399cd-129">Properties</span></span>
|<span data-ttu-id="399cd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399cd-130">Property</span></span>|<span data-ttu-id="399cd-131">型</span><span class="sxs-lookup"><span data-stu-id="399cd-131">Type</span></span>|<span data-ttu-id="399cd-132">説明</span><span class="sxs-lookup"><span data-stu-id="399cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399cd-133">id</span><span class="sxs-lookup"><span data-stu-id="399cd-133">id</span></span>|<span data-ttu-id="399cd-134">String</span><span class="sxs-lookup"><span data-stu-id="399cd-134">String</span></span>|<span data-ttu-id="399cd-135">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="399cd-135">Key of the Resource Operation.</span></span> <span data-ttu-id="399cd-136">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="399cd-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="399cd-137">リソース</span><span class="sxs-lookup"><span data-stu-id="399cd-137">resource</span></span>|<span data-ttu-id="399cd-138">String</span><span class="sxs-lookup"><span data-stu-id="399cd-138">String</span></span>|<span data-ttu-id="399cd-139">この操作が属するリソースカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="399cd-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="399cd-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="399cd-140">resourceName</span></span>|<span data-ttu-id="399cd-141">String</span><span class="sxs-lookup"><span data-stu-id="399cd-141">String</span></span>|<span data-ttu-id="399cd-142">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="399cd-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="399cd-143">actionName</span><span class="sxs-lookup"><span data-stu-id="399cd-143">actionName</span></span>|<span data-ttu-id="399cd-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="399cd-144">String</span></span>|<span data-ttu-id="399cd-145">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="399cd-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="399cd-146">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="399cd-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="399cd-147">description</span><span class="sxs-lookup"><span data-stu-id="399cd-147">description</span></span>|<span data-ttu-id="399cd-148">String</span><span class="sxs-lookup"><span data-stu-id="399cd-148">String</span></span>|<span data-ttu-id="399cd-149">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="399cd-149">Description of the resource operation.</span></span> <span data-ttu-id="399cd-150">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="399cd-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="399cd-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="399cd-151">enabledForScopeValidation</span></span>|<span data-ttu-id="399cd-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="399cd-152">Boolean</span></span>|<span data-ttu-id="399cd-153">権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="399cd-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="399cd-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="399cd-154">Relationships</span></span>
<span data-ttu-id="399cd-155">なし</span><span class="sxs-lookup"><span data-stu-id="399cd-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="399cd-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="399cd-156">JSON Representation</span></span>
<span data-ttu-id="399cd-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="399cd-157">Here is a JSON representation of the resource.</span></span>
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





