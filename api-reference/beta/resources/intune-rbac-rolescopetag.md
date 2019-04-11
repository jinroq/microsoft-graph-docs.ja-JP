---
title: ロール copetag リソースの種類
description: 役割のスコープタグ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6916521c8edef1b1decfb6b006779a372d3ab4e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781954"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="63e35-103">ロール copetag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63e35-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="63e35-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63e35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63e35-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63e35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e35-106">役割のスコープタグ</span><span class="sxs-lookup"><span data-stu-id="63e35-106">Role Scope Tag</span></span>

## <a name="methods"></a><span data-ttu-id="63e35-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="63e35-107">Methods</span></span>
|<span data-ttu-id="63e35-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="63e35-108">Method</span></span>|<span data-ttu-id="63e35-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="63e35-109">Return Type</span></span>|<span data-ttu-id="63e35-110">説明</span><span class="sxs-lookup"><span data-stu-id="63e35-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63e35-111">リスト roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="63e35-111">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="63e35-112">[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="63e35-112">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="63e35-113">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="63e35-113">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="63e35-114">ロール copetag の取得</span><span class="sxs-lookup"><span data-stu-id="63e35-114">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="63e35-115">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="63e35-115">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="63e35-116">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="63e35-116">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="63e35-117">ロール copetag の作成</span><span class="sxs-lookup"><span data-stu-id="63e35-117">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="63e35-118">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="63e35-118">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="63e35-119">新しい[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="63e35-119">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="63e35-120">ロール copetag の削除</span><span class="sxs-lookup"><span data-stu-id="63e35-120">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="63e35-121">なし</span><span class="sxs-lookup"><span data-stu-id="63e35-121">None</span></span>|<span data-ttu-id="63e35-122">[ロール copetag](../resources/intune-rbac-rolescopetag.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="63e35-122">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="63e35-123">ロール copetag の更新</span><span class="sxs-lookup"><span data-stu-id="63e35-123">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="63e35-124">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="63e35-124">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="63e35-125">[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="63e35-125">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="63e35-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63e35-126">Properties</span></span>
|<span data-ttu-id="63e35-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63e35-127">Property</span></span>|<span data-ttu-id="63e35-128">型</span><span class="sxs-lookup"><span data-stu-id="63e35-128">Type</span></span>|<span data-ttu-id="63e35-129">説明</span><span class="sxs-lookup"><span data-stu-id="63e35-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e35-130">id</span><span class="sxs-lookup"><span data-stu-id="63e35-130">id</span></span>|<span data-ttu-id="63e35-131">String</span><span class="sxs-lookup"><span data-stu-id="63e35-131">String</span></span>|<span data-ttu-id="63e35-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="63e35-132">Key of the entity.</span></span> <span data-ttu-id="63e35-133">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="63e35-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="63e35-134">displayName</span><span class="sxs-lookup"><span data-stu-id="63e35-134">displayName</span></span>|<span data-ttu-id="63e35-135">String</span><span class="sxs-lookup"><span data-stu-id="63e35-135">String</span></span>|<span data-ttu-id="63e35-136">ロールスコープタグの表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="63e35-136">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="63e35-137">説明</span><span class="sxs-lookup"><span data-stu-id="63e35-137">description</span></span>|<span data-ttu-id="63e35-138">String</span><span class="sxs-lookup"><span data-stu-id="63e35-138">String</span></span>|<span data-ttu-id="63e35-139">役割の範囲タグの説明。</span><span class="sxs-lookup"><span data-stu-id="63e35-139">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63e35-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63e35-140">Relationships</span></span>
<span data-ttu-id="63e35-141">なし</span><span class="sxs-lookup"><span data-stu-id="63e35-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63e35-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63e35-142">JSON Representation</span></span>
<span data-ttu-id="63e35-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="63e35-143">Here is a JSON representation of the resource.</span></span>
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





