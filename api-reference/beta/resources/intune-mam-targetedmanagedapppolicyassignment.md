---
title: targetedManagedAppPolicyAssignment リソースの種類
description: グループまたはアプリの展開の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75090a45f7a9b56946df28b8328704cb58cfcbde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951244"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="4e8b3-103">targetedManagedAppPolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e8b3-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="4e8b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e8b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e8b3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e8b3-107">グループまたはアプリの展開の種類。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-107">The type for deployment of groups or apps.</span></span>
## <a name="methods"></a><span data-ttu-id="4e8b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4e8b3-108">Methods</span></span>
|<span data-ttu-id="4e8b3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4e8b3-109">Method</span></span>|<span data-ttu-id="4e8b3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4e8b3-110">Return Type</span></span>|<span data-ttu-id="4e8b3-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e8b3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e8b3-112">List targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="4e8b3-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="4e8b3-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4e8b3-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="4e8b3-114">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="4e8b3-115">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e8b3-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="4e8b3-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e8b3-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="4e8b3-117">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="4e8b3-118">Delete targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e8b3-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="4e8b3-119">なし</span><span class="sxs-lookup"><span data-stu-id="4e8b3-119">None</span></span>|<span data-ttu-id="4e8b3-120">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="4e8b3-121">Update targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e8b3-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="4e8b3-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e8b3-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="4e8b3-123">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e8b3-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e8b3-124">Properties</span></span>
|<span data-ttu-id="4e8b3-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e8b3-125">Property</span></span>|<span data-ttu-id="4e8b3-126">種類</span><span class="sxs-lookup"><span data-stu-id="4e8b3-126">Type</span></span>|<span data-ttu-id="4e8b3-127">説明</span><span class="sxs-lookup"><span data-stu-id="4e8b3-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e8b3-128">ID</span><span class="sxs-lookup"><span data-stu-id="4e8b3-128">id</span></span>|<span data-ttu-id="4e8b3-129">String</span><span class="sxs-lookup"><span data-stu-id="4e8b3-129">String</span></span>|<span data-ttu-id="4e8b3-130">ID</span><span class="sxs-lookup"><span data-stu-id="4e8b3-130">Id</span></span>|
|<span data-ttu-id="4e8b3-131">ターゲット</span><span class="sxs-lookup"><span data-stu-id="4e8b3-131">target</span></span>|[<span data-ttu-id="4e8b3-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4e8b3-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4e8b3-133">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="4e8b3-133">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e8b3-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e8b3-134">Relationships</span></span>
<span data-ttu-id="4e8b3-135">なし</span><span class="sxs-lookup"><span data-stu-id="4e8b3-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e8b3-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e8b3-136">JSON Representation</span></span>
<span data-ttu-id="4e8b3-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e8b3-137">Here is a JSON representation of the resource.</span></span>
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





