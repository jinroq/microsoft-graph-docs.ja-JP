---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b1a22e2b78719083279dca09a37207b2a1caa57f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839978"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="a1858-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1858-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="a1858-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1858-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1858-105">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="a1858-105">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="a1858-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1858-106">Methods</span></span>
|<span data-ttu-id="a1858-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1858-107">Method</span></span>|<span data-ttu-id="a1858-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1858-108">Return Type</span></span>|<span data-ttu-id="a1858-109">説明</span><span class="sxs-lookup"><span data-stu-id="a1858-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1858-110">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="a1858-110">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="a1858-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1858-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a1858-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a1858-112">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="a1858-113">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="a1858-113">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="a1858-114">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a1858-114">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="a1858-115">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1858-115">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="a1858-116">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="a1858-116">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="a1858-117">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a1858-117">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="a1858-118">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1858-118">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="a1858-119">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="a1858-119">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="a1858-120">なし</span><span class="sxs-lookup"><span data-stu-id="a1858-120">None</span></span>|<span data-ttu-id="a1858-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1858-121">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="a1858-122">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="a1858-122">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="a1858-123">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a1858-123">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="a1858-124">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1858-124">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1858-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1858-125">Properties</span></span>
|<span data-ttu-id="a1858-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1858-126">Property</span></span>|<span data-ttu-id="a1858-127">種類</span><span class="sxs-lookup"><span data-stu-id="a1858-127">Type</span></span>|<span data-ttu-id="a1858-128">説明</span><span class="sxs-lookup"><span data-stu-id="a1858-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1858-129">ID</span><span class="sxs-lookup"><span data-stu-id="a1858-129">id</span></span>|<span data-ttu-id="a1858-130">String</span><span class="sxs-lookup"><span data-stu-id="a1858-130">String</span></span>|<span data-ttu-id="a1858-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a1858-131">Key of the entity.</span></span>|
|<span data-ttu-id="a1858-132">target</span><span class="sxs-lookup"><span data-stu-id="a1858-132">target</span></span>|[<span data-ttu-id="a1858-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a1858-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a1858-134">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="a1858-134">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1858-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1858-135">Relationships</span></span>
<span data-ttu-id="a1858-136">なし</span><span class="sxs-lookup"><span data-stu-id="a1858-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1858-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1858-137">JSON Representation</span></span>
<span data-ttu-id="a1858-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1858-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



