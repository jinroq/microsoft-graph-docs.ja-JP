---
title: ロール Copetagautoassignment リソースの種類
description: デバイスに適用する役割スコープタグをグループに自動割り当てるためのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a308c91eb2a78c50012c348a19b613335915af47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369186"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="3586f-103">ロール Copetagautoassignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3586f-103">roleScopeTagAutoAssignment resource type</span></span>

> <span data-ttu-id="3586f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3586f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3586f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3586f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3586f-106">デバイスに適用する役割スコープタグをグループに自動割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3586f-106">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="3586f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3586f-107">Methods</span></span>
|<span data-ttu-id="3586f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3586f-108">Method</span></span>|<span data-ttu-id="3586f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3586f-109">Return Type</span></span>|<span data-ttu-id="3586f-110">説明</span><span class="sxs-lookup"><span data-stu-id="3586f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3586f-111">ロールの Copetagautoassignments を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3586f-111">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="3586f-112">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3586f-112">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="3586f-113">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3586f-113">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="3586f-114">ロールの Copetagautoassignment の取得</span><span class="sxs-lookup"><span data-stu-id="3586f-114">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="3586f-115">ロール Copetagautoassignment</span><span class="sxs-lookup"><span data-stu-id="3586f-115">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="3586f-116">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3586f-116">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="3586f-117">ロールの Copetagautoassignment の作成</span><span class="sxs-lookup"><span data-stu-id="3586f-117">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="3586f-118">ロール Copetagautoassignment</span><span class="sxs-lookup"><span data-stu-id="3586f-118">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="3586f-119">新しい[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3586f-119">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="3586f-120">ロール Copetagautoassignment の削除</span><span class="sxs-lookup"><span data-stu-id="3586f-120">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="3586f-121">None</span><span class="sxs-lookup"><span data-stu-id="3586f-121">None</span></span>|<span data-ttu-id="3586f-122">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3586f-122">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="3586f-123">ロールの Copetagautoassignment の更新</span><span class="sxs-lookup"><span data-stu-id="3586f-123">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="3586f-124">ロール Copetagautoassignment</span><span class="sxs-lookup"><span data-stu-id="3586f-124">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="3586f-125">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3586f-125">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3586f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3586f-126">Properties</span></span>
|<span data-ttu-id="3586f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3586f-127">Property</span></span>|<span data-ttu-id="3586f-128">型</span><span class="sxs-lookup"><span data-stu-id="3586f-128">Type</span></span>|<span data-ttu-id="3586f-129">説明</span><span class="sxs-lookup"><span data-stu-id="3586f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3586f-130">id</span><span class="sxs-lookup"><span data-stu-id="3586f-130">id</span></span>|<span data-ttu-id="3586f-131">String</span><span class="sxs-lookup"><span data-stu-id="3586f-131">String</span></span>|<span data-ttu-id="3586f-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3586f-132">Key of the entity.</span></span>|
|<span data-ttu-id="3586f-133">target</span><span class="sxs-lookup"><span data-stu-id="3586f-133">target</span></span>|[<span data-ttu-id="3586f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3586f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3586f-135">特定の役割スコープタグの自動割り当てターゲット。</span><span class="sxs-lookup"><span data-stu-id="3586f-135">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3586f-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3586f-136">Relationships</span></span>
<span data-ttu-id="3586f-137">なし</span><span class="sxs-lookup"><span data-stu-id="3586f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3586f-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3586f-138">JSON Representation</span></span>
<span data-ttu-id="3586f-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3586f-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



