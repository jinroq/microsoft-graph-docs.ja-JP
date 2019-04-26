---
title: targetedManagedAppPolicyAssignment リソースの種類
description: グループまたはアプリの展開の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced81e320608e34fba6d4b2b96b101f61aebaa59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553905"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="e0177-103">targetedManagedAppPolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0177-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="e0177-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0177-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0177-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0177-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0177-106">グループまたはアプリの展開の種類。</span><span class="sxs-lookup"><span data-stu-id="e0177-106">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e0177-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0177-107">Methods</span></span>
|<span data-ttu-id="e0177-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0177-108">Method</span></span>|<span data-ttu-id="e0177-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e0177-109">Return Type</span></span>|<span data-ttu-id="e0177-110">説明</span><span class="sxs-lookup"><span data-stu-id="e0177-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0177-111">List targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="e0177-111">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="e0177-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0177-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e0177-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e0177-113">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="e0177-114">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e0177-114">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="e0177-115">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e0177-115">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="e0177-116">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e0177-116">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="e0177-117">Delete targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e0177-117">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="e0177-118">なし</span><span class="sxs-lookup"><span data-stu-id="e0177-118">None</span></span>|<span data-ttu-id="e0177-119">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="e0177-119">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="e0177-120">Update targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e0177-120">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="e0177-121">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e0177-121">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="e0177-122">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0177-122">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0177-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0177-123">Properties</span></span>
|<span data-ttu-id="e0177-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0177-124">Property</span></span>|<span data-ttu-id="e0177-125">型</span><span class="sxs-lookup"><span data-stu-id="e0177-125">Type</span></span>|<span data-ttu-id="e0177-126">説明</span><span class="sxs-lookup"><span data-stu-id="e0177-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0177-127">id</span><span class="sxs-lookup"><span data-stu-id="e0177-127">id</span></span>|<span data-ttu-id="e0177-128">String</span><span class="sxs-lookup"><span data-stu-id="e0177-128">String</span></span>|<span data-ttu-id="e0177-129">ID</span><span class="sxs-lookup"><span data-stu-id="e0177-129">Id</span></span>|
|<span data-ttu-id="e0177-130">target</span><span class="sxs-lookup"><span data-stu-id="e0177-130">target</span></span>|[<span data-ttu-id="e0177-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0177-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0177-132">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="e0177-132">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0177-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0177-133">Relationships</span></span>
<span data-ttu-id="e0177-134">なし</span><span class="sxs-lookup"><span data-stu-id="e0177-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0177-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0177-135">JSON Representation</span></span>
<span data-ttu-id="e0177-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0177-136">Here is a JSON representation of the resource.</span></span>
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





