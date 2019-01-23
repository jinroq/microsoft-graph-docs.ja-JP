---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400565"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="fe619-103">roleScopeTag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe619-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="fe619-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe619-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe619-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe619-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe619-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe619-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe619-107">ロールのスコープのタグ</span><span class="sxs-lookup"><span data-stu-id="fe619-107">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="fe619-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe619-108">Methods</span></span>
|<span data-ttu-id="fe619-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe619-109">Method</span></span>|<span data-ttu-id="fe619-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe619-110">Return Type</span></span>|<span data-ttu-id="fe619-111">説明</span><span class="sxs-lookup"><span data-stu-id="fe619-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe619-112">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe619-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="fe619-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe619-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="fe619-114">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="fe619-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="fe619-115">RoleScopeTag を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe619-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="fe619-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="fe619-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="fe619-117">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe619-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="fe619-118">RoleScopeTag を作成します。</span><span class="sxs-lookup"><span data-stu-id="fe619-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="fe619-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="fe619-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="fe619-120">新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe619-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="fe619-121">RoleScopeTag を削除します。</span><span class="sxs-lookup"><span data-stu-id="fe619-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="fe619-122">なし</span><span class="sxs-lookup"><span data-stu-id="fe619-122">None</span></span>|<span data-ttu-id="fe619-123">の[roleScopeTag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="fe619-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="fe619-124">RoleScopeTag を更新します。</span><span class="sxs-lookup"><span data-stu-id="fe619-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="fe619-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="fe619-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="fe619-126">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe619-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe619-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe619-127">Properties</span></span>
|<span data-ttu-id="fe619-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe619-128">Property</span></span>|<span data-ttu-id="fe619-129">型</span><span class="sxs-lookup"><span data-stu-id="fe619-129">Type</span></span>|<span data-ttu-id="fe619-130">説明</span><span class="sxs-lookup"><span data-stu-id="fe619-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe619-131">id</span><span class="sxs-lookup"><span data-stu-id="fe619-131">id</span></span>|<span data-ttu-id="fe619-132">String</span><span class="sxs-lookup"><span data-stu-id="fe619-132">String</span></span>|<span data-ttu-id="fe619-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe619-133">Key of the entity.</span></span> <span data-ttu-id="fe619-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="fe619-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fe619-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fe619-135">displayName</span></span>|<span data-ttu-id="fe619-136">String</span><span class="sxs-lookup"><span data-stu-id="fe619-136">String</span></span>|<span data-ttu-id="fe619-137">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="fe619-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="fe619-138">説明</span><span class="sxs-lookup"><span data-stu-id="fe619-138">description</span></span>|<span data-ttu-id="fe619-139">String</span><span class="sxs-lookup"><span data-stu-id="fe619-139">String</span></span>|<span data-ttu-id="fe619-140">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="fe619-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe619-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe619-141">Relationships</span></span>
<span data-ttu-id="fe619-142">なし</span><span class="sxs-lookup"><span data-stu-id="fe619-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe619-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe619-143">JSON Representation</span></span>
<span data-ttu-id="fe619-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe619-144">Here is a JSON representation of the resource.</span></span>
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




