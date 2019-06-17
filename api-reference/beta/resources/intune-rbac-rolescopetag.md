---
title: ロール Copetag リソースの種類
description: 役割のスコープタグ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54aa59e99a9697924512da0072e7b4e05e4fa12a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993537"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="a67e2-103">ロール Copetag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a67e2-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="a67e2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a67e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a67e2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a67e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a67e2-106">役割のスコープタグ</span><span class="sxs-lookup"><span data-stu-id="a67e2-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="a67e2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a67e2-107">Methods</span></span>
|<span data-ttu-id="a67e2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a67e2-108">Method</span></span>|<span data-ttu-id="a67e2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a67e2-109">Return Type</span></span>|<span data-ttu-id="a67e2-110">説明</span><span class="sxs-lookup"><span data-stu-id="a67e2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a67e2-111">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a67e2-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="a67e2-112">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a67e2-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="a67e2-113">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a67e2-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="a67e2-114">ロール Copetag の取得</span><span class="sxs-lookup"><span data-stu-id="a67e2-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="a67e2-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a67e2-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a67e2-116">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a67e2-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="a67e2-117">ロール Copetag の作成</span><span class="sxs-lookup"><span data-stu-id="a67e2-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="a67e2-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a67e2-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a67e2-119">新しい[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a67e2-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="a67e2-120">ロール Copetag の削除</span><span class="sxs-lookup"><span data-stu-id="a67e2-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="a67e2-121">None</span><span class="sxs-lookup"><span data-stu-id="a67e2-121">None</span></span>|<span data-ttu-id="a67e2-122">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a67e2-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="a67e2-123">ロール Copetag の更新</span><span class="sxs-lookup"><span data-stu-id="a67e2-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="a67e2-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="a67e2-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="a67e2-125">[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a67e2-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="a67e2-126">assign アクション</span><span class="sxs-lookup"><span data-stu-id="a67e2-126">assign action</span></span>](../api/intune-rbac-rolescopetag-assign.md)|<span data-ttu-id="a67e2-127">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a67e2-127">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="a67e2-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a67e2-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a67e2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a67e2-129">Properties</span></span>
|<span data-ttu-id="a67e2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a67e2-130">Property</span></span>|<span data-ttu-id="a67e2-131">型</span><span class="sxs-lookup"><span data-stu-id="a67e2-131">Type</span></span>|<span data-ttu-id="a67e2-132">説明</span><span class="sxs-lookup"><span data-stu-id="a67e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a67e2-133">id</span><span class="sxs-lookup"><span data-stu-id="a67e2-133">id</span></span>|<span data-ttu-id="a67e2-134">文字列</span><span class="sxs-lookup"><span data-stu-id="a67e2-134">String</span></span>|<span data-ttu-id="a67e2-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a67e2-135">Key of the entity.</span></span> <span data-ttu-id="a67e2-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="a67e2-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a67e2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a67e2-137">displayName</span></span>|<span data-ttu-id="a67e2-138">String</span><span class="sxs-lookup"><span data-stu-id="a67e2-138">String</span></span>|<span data-ttu-id="a67e2-139">ロールスコープタグの表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="a67e2-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="a67e2-140">description</span><span class="sxs-lookup"><span data-stu-id="a67e2-140">description</span></span>|<span data-ttu-id="a67e2-141">String</span><span class="sxs-lookup"><span data-stu-id="a67e2-141">String</span></span>|<span data-ttu-id="a67e2-142">役割の範囲タグの説明。</span><span class="sxs-lookup"><span data-stu-id="a67e2-142">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a67e2-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a67e2-143">Relationships</span></span>
|<span data-ttu-id="a67e2-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a67e2-144">Relationship</span></span>|<span data-ttu-id="a67e2-145">型</span><span class="sxs-lookup"><span data-stu-id="a67e2-145">Type</span></span>|<span data-ttu-id="a67e2-146">説明</span><span class="sxs-lookup"><span data-stu-id="a67e2-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a67e2-147">assignments</span><span class="sxs-lookup"><span data-stu-id="a67e2-147">assignments</span></span>|<span data-ttu-id="a67e2-148">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a67e2-148">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="a67e2-149">この役割スコープタグの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a67e2-149">The list of assignments for this Role Scope Tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a67e2-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a67e2-150">JSON Representation</span></span>
<span data-ttu-id="a67e2-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a67e2-151">Here is a JSON representation of the resource.</span></span>
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





