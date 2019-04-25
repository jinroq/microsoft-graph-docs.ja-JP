---
title: ロール copetag リソースの種類
description: 役割のスコープタグ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6916521c8edef1b1decfb6b006779a372d3ab4e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566326"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="0925f-103">ロール copetag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0925f-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="0925f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0925f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0925f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0925f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0925f-106">役割のスコープタグ</span><span class="sxs-lookup"><span data-stu-id="0925f-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="0925f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0925f-107">Methods</span></span>
|<span data-ttu-id="0925f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0925f-108">Method</span></span>|<span data-ttu-id="0925f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0925f-109">Return Type</span></span>|<span data-ttu-id="0925f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0925f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0925f-111">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0925f-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="0925f-112">[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0925f-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0925f-113">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0925f-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="0925f-114">ロール copetag の取得</span><span class="sxs-lookup"><span data-stu-id="0925f-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="0925f-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0925f-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0925f-116">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0925f-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0925f-117">ロール copetag の作成</span><span class="sxs-lookup"><span data-stu-id="0925f-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="0925f-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0925f-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0925f-119">新しい[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0925f-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0925f-120">ロール copetag の削除</span><span class="sxs-lookup"><span data-stu-id="0925f-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="0925f-121">なし</span><span class="sxs-lookup"><span data-stu-id="0925f-121">None</span></span>|<span data-ttu-id="0925f-122">[ロール copetag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0925f-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="0925f-123">ロール copetag の更新</span><span class="sxs-lookup"><span data-stu-id="0925f-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="0925f-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0925f-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0925f-125">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0925f-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0925f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0925f-126">Properties</span></span>
|<span data-ttu-id="0925f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0925f-127">Property</span></span>|<span data-ttu-id="0925f-128">型</span><span class="sxs-lookup"><span data-stu-id="0925f-128">Type</span></span>|<span data-ttu-id="0925f-129">説明</span><span class="sxs-lookup"><span data-stu-id="0925f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0925f-130">id</span><span class="sxs-lookup"><span data-stu-id="0925f-130">id</span></span>|<span data-ttu-id="0925f-131">String</span><span class="sxs-lookup"><span data-stu-id="0925f-131">String</span></span>|<span data-ttu-id="0925f-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0925f-132">Key of the entity.</span></span> <span data-ttu-id="0925f-133">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="0925f-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0925f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0925f-134">displayName</span></span>|<span data-ttu-id="0925f-135">String</span><span class="sxs-lookup"><span data-stu-id="0925f-135">String</span></span>|<span data-ttu-id="0925f-136">ロールスコープタグの表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="0925f-136">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0925f-137">説明</span><span class="sxs-lookup"><span data-stu-id="0925f-137">description</span></span>|<span data-ttu-id="0925f-138">String</span><span class="sxs-lookup"><span data-stu-id="0925f-138">String</span></span>|<span data-ttu-id="0925f-139">役割の範囲タグの説明。</span><span class="sxs-lookup"><span data-stu-id="0925f-139">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0925f-140">関係</span><span class="sxs-lookup"><span data-stu-id="0925f-140">Relationships</span></span>
<span data-ttu-id="0925f-141">なし</span><span class="sxs-lookup"><span data-stu-id="0925f-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0925f-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0925f-142">JSON Representation</span></span>
<span data-ttu-id="0925f-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0925f-143">Here is a JSON representation of the resource.</span></span>
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





