---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a48f74b9ecdb7a5f6eec87581fb0826160c4334b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830066"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="00082-103">roleScopeTag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00082-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="00082-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00082-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00082-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00082-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00082-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00082-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00082-107">ロールのスコープのタグ</span><span class="sxs-lookup"><span data-stu-id="00082-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="00082-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="00082-108">Methods</span></span>
|<span data-ttu-id="00082-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="00082-109">Method</span></span>|<span data-ttu-id="00082-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="00082-110">Return Type</span></span>|<span data-ttu-id="00082-111">説明</span><span class="sxs-lookup"><span data-stu-id="00082-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00082-112">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="00082-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="00082-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="00082-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="00082-114">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="00082-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="00082-115">RoleScopeTag を取得します。</span><span class="sxs-lookup"><span data-stu-id="00082-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="00082-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="00082-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="00082-117">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00082-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="00082-118">RoleScopeTag を作成します。</span><span class="sxs-lookup"><span data-stu-id="00082-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="00082-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="00082-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="00082-120">新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="00082-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="00082-121">RoleScopeTag を削除します。</span><span class="sxs-lookup"><span data-stu-id="00082-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="00082-122">なし</span><span class="sxs-lookup"><span data-stu-id="00082-122">None</span></span>|<span data-ttu-id="00082-123">の[roleScopeTag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="00082-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="00082-124">RoleScopeTag を更新します。</span><span class="sxs-lookup"><span data-stu-id="00082-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="00082-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="00082-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="00082-126">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="00082-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00082-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00082-127">Properties</span></span>
|<span data-ttu-id="00082-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00082-128">Property</span></span>|<span data-ttu-id="00082-129">種類</span><span class="sxs-lookup"><span data-stu-id="00082-129">Type</span></span>|<span data-ttu-id="00082-130">説明</span><span class="sxs-lookup"><span data-stu-id="00082-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00082-131">ID</span><span class="sxs-lookup"><span data-stu-id="00082-131">id</span></span>|<span data-ttu-id="00082-132">String</span><span class="sxs-lookup"><span data-stu-id="00082-132">String</span></span>|<span data-ttu-id="00082-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="00082-133">Key of the entity.</span></span> <span data-ttu-id="00082-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="00082-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="00082-135">displayName</span><span class="sxs-lookup"><span data-stu-id="00082-135">displayName</span></span>|<span data-ttu-id="00082-136">String</span><span class="sxs-lookup"><span data-stu-id="00082-136">String</span></span>|<span data-ttu-id="00082-137">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="00082-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="00082-138">説明</span><span class="sxs-lookup"><span data-stu-id="00082-138">description</span></span>|<span data-ttu-id="00082-139">String</span><span class="sxs-lookup"><span data-stu-id="00082-139">String</span></span>|<span data-ttu-id="00082-140">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="00082-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00082-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="00082-141">Relationships</span></span>
<span data-ttu-id="00082-142">なし</span><span class="sxs-lookup"><span data-stu-id="00082-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00082-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00082-143">JSON Representation</span></span>
<span data-ttu-id="00082-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00082-144">Here is a JSON representation of the resource.</span></span>
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





