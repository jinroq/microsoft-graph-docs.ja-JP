---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 609d4202069f6e4258c9824a65b72ab769c365b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981855"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="3b4c7-103">roleScopeTag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b4c7-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="3b4c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b4c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b4c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b4c7-107">ロールのスコープのタグ</span><span class="sxs-lookup"><span data-stu-id="3b4c7-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="3b4c7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b4c7-108">Methods</span></span>
|<span data-ttu-id="3b4c7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b4c7-109">Method</span></span>|<span data-ttu-id="3b4c7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b4c7-110">Return Type</span></span>|<span data-ttu-id="3b4c7-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b4c7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b4c7-112">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b4c7-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="3b4c7-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3b4c7-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="3b4c7-114">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="3b4c7-115">RoleScopeTag を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="3b4c7-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3b4c7-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3b4c7-117">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="3b4c7-118">RoleScopeTag を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="3b4c7-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3b4c7-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3b4c7-120">新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="3b4c7-121">RoleScopeTag を削除します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="3b4c7-122">なし</span><span class="sxs-lookup"><span data-stu-id="3b4c7-122">None</span></span>|<span data-ttu-id="3b4c7-123">の[roleScopeTag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="3b4c7-124">RoleScopeTag を更新します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="3b4c7-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3b4c7-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3b4c7-126">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b4c7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b4c7-127">Properties</span></span>
|<span data-ttu-id="3b4c7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b4c7-128">Property</span></span>|<span data-ttu-id="3b4c7-129">型</span><span class="sxs-lookup"><span data-stu-id="3b4c7-129">Type</span></span>|<span data-ttu-id="3b4c7-130">説明</span><span class="sxs-lookup"><span data-stu-id="3b4c7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b4c7-131">ID</span><span class="sxs-lookup"><span data-stu-id="3b4c7-131">id</span></span>|<span data-ttu-id="3b4c7-132">String</span><span class="sxs-lookup"><span data-stu-id="3b4c7-132">String</span></span>|<span data-ttu-id="3b4c7-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-133">Key of the entity.</span></span> <span data-ttu-id="3b4c7-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3b4c7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3b4c7-135">displayName</span></span>|<span data-ttu-id="3b4c7-136">String</span><span class="sxs-lookup"><span data-stu-id="3b4c7-136">String</span></span>|<span data-ttu-id="3b4c7-137">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="3b4c7-138">説明</span><span class="sxs-lookup"><span data-stu-id="3b4c7-138">description</span></span>|<span data-ttu-id="3b4c7-139">String</span><span class="sxs-lookup"><span data-stu-id="3b4c7-139">String</span></span>|<span data-ttu-id="3b4c7-140">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b4c7-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b4c7-141">Relationships</span></span>
<span data-ttu-id="3b4c7-142">なし</span><span class="sxs-lookup"><span data-stu-id="3b4c7-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b4c7-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b4c7-143">JSON Representation</span></span>
<span data-ttu-id="3b4c7-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b4c7-144">Here is a JSON representation of the resource.</span></span>
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





