---
title: ロール Copetag リソースの種類
description: 役割のスコープタグ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a1a426265caaf2f05beb5678d49b9ae960d31c3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739268"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="0aa7c-103">ロール Copetag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0aa7c-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="0aa7c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aa7c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aa7c-106">役割のスコープタグ</span><span class="sxs-lookup"><span data-stu-id="0aa7c-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="0aa7c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0aa7c-107">Methods</span></span>
|<span data-ttu-id="0aa7c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0aa7c-108">Method</span></span>|<span data-ttu-id="0aa7c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0aa7c-109">Return Type</span></span>|<span data-ttu-id="0aa7c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0aa7c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0aa7c-111">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0aa7c-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="0aa7c-112">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0aa7c-113">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="0aa7c-114">ロール Copetag の取得</span><span class="sxs-lookup"><span data-stu-id="0aa7c-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="0aa7c-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0aa7c-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0aa7c-116">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0aa7c-117">ロール Copetag の作成</span><span class="sxs-lookup"><span data-stu-id="0aa7c-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="0aa7c-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0aa7c-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0aa7c-119">新しい[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0aa7c-120">ロール Copetag の削除</span><span class="sxs-lookup"><span data-stu-id="0aa7c-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="0aa7c-121">None</span><span class="sxs-lookup"><span data-stu-id="0aa7c-121">None</span></span>|<span data-ttu-id="0aa7c-122">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="0aa7c-123">ロール Copetag の更新</span><span class="sxs-lookup"><span data-stu-id="0aa7c-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="0aa7c-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0aa7c-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0aa7c-125">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0aa7c-126">assign アクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-126">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="0aa7c-127">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="0aa7c-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0aa7c-128">Not yet documented</span></span>|
|[<span data-ttu-id="0aa7c-129">getRoleScopeTagsById アクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-129">getRoleScopeTagsById action</span></span>](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|<span data-ttu-id="0aa7c-130">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-130">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0aa7c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0aa7c-131">Not yet documented</span></span>|
|[<span data-ttu-id="0aa7c-132">Hascustomロール Copetag 関数</span><span class="sxs-lookup"><span data-stu-id="0aa7c-132">hasCustomRoleScopeTag function</span></span>](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|<span data-ttu-id="0aa7c-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0aa7c-133">Boolean</span></span>|<span data-ttu-id="0aa7c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0aa7c-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0aa7c-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0aa7c-135">Properties</span></span>
|<span data-ttu-id="0aa7c-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0aa7c-136">Property</span></span>|<span data-ttu-id="0aa7c-137">型</span><span class="sxs-lookup"><span data-stu-id="0aa7c-137">Type</span></span>|<span data-ttu-id="0aa7c-138">説明</span><span class="sxs-lookup"><span data-stu-id="0aa7c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aa7c-139">id</span><span class="sxs-lookup"><span data-stu-id="0aa7c-139">id</span></span>|<span data-ttu-id="0aa7c-140">文字列</span><span class="sxs-lookup"><span data-stu-id="0aa7c-140">String</span></span>|<span data-ttu-id="0aa7c-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-141">Key of the entity.</span></span> <span data-ttu-id="0aa7c-142">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-142">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0aa7c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0aa7c-143">displayName</span></span>|<span data-ttu-id="0aa7c-144">String</span><span class="sxs-lookup"><span data-stu-id="0aa7c-144">String</span></span>|<span data-ttu-id="0aa7c-145">ロールスコープタグの表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-145">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0aa7c-146">description</span><span class="sxs-lookup"><span data-stu-id="0aa7c-146">description</span></span>|<span data-ttu-id="0aa7c-147">String</span><span class="sxs-lookup"><span data-stu-id="0aa7c-147">String</span></span>|<span data-ttu-id="0aa7c-148">役割の範囲タグの説明。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-148">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0aa7c-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0aa7c-149">Relationships</span></span>
|<span data-ttu-id="0aa7c-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0aa7c-150">Relationship</span></span>|<span data-ttu-id="0aa7c-151">型</span><span class="sxs-lookup"><span data-stu-id="0aa7c-151">Type</span></span>|<span data-ttu-id="0aa7c-152">説明</span><span class="sxs-lookup"><span data-stu-id="0aa7c-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aa7c-153">assignments</span><span class="sxs-lookup"><span data-stu-id="0aa7c-153">assignments</span></span>|<span data-ttu-id="0aa7c-154">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0aa7c-154">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="0aa7c-155">この役割スコープタグの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-155">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0aa7c-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0aa7c-156">JSON Representation</span></span>
<span data-ttu-id="0aa7c-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0aa7c-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





