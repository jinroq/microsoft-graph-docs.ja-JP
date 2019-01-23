---
title: targetedManagedAppPolicyAssignment リソースの種類
description: グループまたはアプリの展開の種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c40c2d7c8c998fc4a271e1efeff10062388522f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395945"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="59ed2-103">targetedManagedAppPolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59ed2-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="59ed2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59ed2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59ed2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59ed2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59ed2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59ed2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59ed2-107">グループまたはアプリの展開の種類。</span><span class="sxs-lookup"><span data-stu-id="59ed2-107">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="59ed2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="59ed2-108">Methods</span></span>
|<span data-ttu-id="59ed2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="59ed2-109">Method</span></span>|<span data-ttu-id="59ed2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59ed2-110">Return Type</span></span>|<span data-ttu-id="59ed2-111">説明</span><span class="sxs-lookup"><span data-stu-id="59ed2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59ed2-112">List targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="59ed2-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="59ed2-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59ed2-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="59ed2-114">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="59ed2-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="59ed2-115">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="59ed2-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="59ed2-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="59ed2-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="59ed2-117">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="59ed2-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="59ed2-118">Delete targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="59ed2-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="59ed2-119">なし</span><span class="sxs-lookup"><span data-stu-id="59ed2-119">None</span></span>|<span data-ttu-id="59ed2-120">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="59ed2-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="59ed2-121">Update targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="59ed2-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="59ed2-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="59ed2-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="59ed2-123">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="59ed2-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59ed2-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59ed2-124">Properties</span></span>
|<span data-ttu-id="59ed2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59ed2-125">Property</span></span>|<span data-ttu-id="59ed2-126">型</span><span class="sxs-lookup"><span data-stu-id="59ed2-126">Type</span></span>|<span data-ttu-id="59ed2-127">説明</span><span class="sxs-lookup"><span data-stu-id="59ed2-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59ed2-128">id</span><span class="sxs-lookup"><span data-stu-id="59ed2-128">id</span></span>|<span data-ttu-id="59ed2-129">String</span><span class="sxs-lookup"><span data-stu-id="59ed2-129">String</span></span>|<span data-ttu-id="59ed2-130">ID</span><span class="sxs-lookup"><span data-stu-id="59ed2-130">Id</span></span>|
|<span data-ttu-id="59ed2-131">target</span><span class="sxs-lookup"><span data-stu-id="59ed2-131">target</span></span>|[<span data-ttu-id="59ed2-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="59ed2-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="59ed2-133">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="59ed2-133">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="59ed2-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59ed2-134">Relationships</span></span>
<span data-ttu-id="59ed2-135">なし</span><span class="sxs-lookup"><span data-stu-id="59ed2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59ed2-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59ed2-136">JSON Representation</span></span>
<span data-ttu-id="59ed2-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59ed2-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




