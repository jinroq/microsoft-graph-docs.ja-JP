---
title: targetedManagedAppPolicyAssignment リソースの種類
description: グループまたはアプリの展開の種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41229dec8a87d27b8d4e9203847f4f13647c04d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861174"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="df5d1-103">targetedManagedAppPolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df5d1-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="df5d1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df5d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df5d1-105">グループまたはアプリの展開の種類。</span><span class="sxs-lookup"><span data-stu-id="df5d1-105">The type for deployment of groups or apps.</span></span>
## <a name="methods"></a><span data-ttu-id="df5d1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="df5d1-106">Methods</span></span>
|<span data-ttu-id="df5d1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="df5d1-107">Method</span></span>|<span data-ttu-id="df5d1-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="df5d1-108">Return Type</span></span>|<span data-ttu-id="df5d1-109">説明</span><span class="sxs-lookup"><span data-stu-id="df5d1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df5d1-110">List targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="df5d1-110">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="df5d1-111">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="df5d1-111">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="df5d1-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="df5d1-112">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="df5d1-113">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="df5d1-113">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="df5d1-114">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="df5d1-114">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="df5d1-115">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="df5d1-115">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="df5d1-116">Delete targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="df5d1-116">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="df5d1-117">なし</span><span class="sxs-lookup"><span data-stu-id="df5d1-117">None</span></span>|<span data-ttu-id="df5d1-118">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="df5d1-118">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="df5d1-119">Update targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="df5d1-119">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="df5d1-120">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="df5d1-120">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="df5d1-121">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="df5d1-121">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df5d1-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df5d1-122">Properties</span></span>
|<span data-ttu-id="df5d1-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df5d1-123">Property</span></span>|<span data-ttu-id="df5d1-124">種類</span><span class="sxs-lookup"><span data-stu-id="df5d1-124">Type</span></span>|<span data-ttu-id="df5d1-125">説明</span><span class="sxs-lookup"><span data-stu-id="df5d1-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5d1-126">ID</span><span class="sxs-lookup"><span data-stu-id="df5d1-126">id</span></span>|<span data-ttu-id="df5d1-127">String</span><span class="sxs-lookup"><span data-stu-id="df5d1-127">String</span></span>|<span data-ttu-id="df5d1-128">ID</span><span class="sxs-lookup"><span data-stu-id="df5d1-128">Id</span></span>|
|<span data-ttu-id="df5d1-129">ターゲット</span><span class="sxs-lookup"><span data-stu-id="df5d1-129">target</span></span>|[<span data-ttu-id="df5d1-130">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="df5d1-130">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="df5d1-131">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="df5d1-131">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="df5d1-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df5d1-132">Relationships</span></span>
<span data-ttu-id="df5d1-133">なし</span><span class="sxs-lookup"><span data-stu-id="df5d1-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df5d1-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df5d1-134">JSON Representation</span></span>
<span data-ttu-id="df5d1-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df5d1-135">Here is a JSON representation of the resource.</span></span>
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



