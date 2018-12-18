---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
author: tfitzmac
ms.openlocfilehash: 49059ceddcd043f39f51c563c85ba8986b6fc61b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354769"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="9f884-103">roleScopeTag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f884-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="9f884-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f884-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f884-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f884-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f884-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f884-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f884-107">ロールのスコープのタグ</span><span class="sxs-lookup"><span data-stu-id="9f884-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="9f884-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f884-108">Methods</span></span>
|<span data-ttu-id="9f884-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f884-109">Method</span></span>|<span data-ttu-id="9f884-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f884-110">Return Type</span></span>|<span data-ttu-id="9f884-111">説明</span><span class="sxs-lookup"><span data-stu-id="9f884-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f884-112">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f884-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="9f884-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f884-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="9f884-114">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9f884-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="9f884-115">RoleScopeTag を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f884-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="9f884-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9f884-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9f884-117">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f884-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="9f884-118">RoleScopeTag を作成します。</span><span class="sxs-lookup"><span data-stu-id="9f884-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="9f884-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9f884-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9f884-120">新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f884-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="9f884-121">RoleScopeTag を削除します。</span><span class="sxs-lookup"><span data-stu-id="9f884-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="9f884-122">なし</span><span class="sxs-lookup"><span data-stu-id="9f884-122">None</span></span>|<span data-ttu-id="9f884-123">の[roleScopeTag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="9f884-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="9f884-124">RoleScopeTag を更新します。</span><span class="sxs-lookup"><span data-stu-id="9f884-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="9f884-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9f884-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="9f884-126">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f884-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f884-127">Properties</span><span class="sxs-lookup"><span data-stu-id="9f884-127">Properties</span></span>
|<span data-ttu-id="9f884-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f884-128">Property</span></span>|<span data-ttu-id="9f884-129">種類</span><span class="sxs-lookup"><span data-stu-id="9f884-129">Type</span></span>|<span data-ttu-id="9f884-130">説明</span><span class="sxs-lookup"><span data-stu-id="9f884-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f884-131">ID</span><span class="sxs-lookup"><span data-stu-id="9f884-131">id</span></span>|<span data-ttu-id="9f884-132">String</span><span class="sxs-lookup"><span data-stu-id="9f884-132">String</span></span>|<span data-ttu-id="9f884-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f884-133">Key of the entity.</span></span> <span data-ttu-id="9f884-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="9f884-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9f884-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9f884-135">displayName</span></span>|<span data-ttu-id="9f884-136">String</span><span class="sxs-lookup"><span data-stu-id="9f884-136">String</span></span>|<span data-ttu-id="9f884-137">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="9f884-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="9f884-138">説明</span><span class="sxs-lookup"><span data-stu-id="9f884-138">description</span></span>|<span data-ttu-id="9f884-139">String</span><span class="sxs-lookup"><span data-stu-id="9f884-139">String</span></span>|<span data-ttu-id="9f884-140">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="9f884-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f884-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f884-141">Relationships</span></span>
<span data-ttu-id="9f884-142">なし</span><span class="sxs-lookup"><span data-stu-id="9f884-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f884-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f884-143">JSON Representation</span></span>
<span data-ttu-id="9f884-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f884-144">Here is a JSON representation of the resource.</span></span>
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





