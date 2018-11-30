---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
ms.openlocfilehash: 94ba5391db5059ca3386ea600098f66d87716bab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022873"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="6753e-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6753e-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="6753e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6753e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6753e-105">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="6753e-105">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="6753e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6753e-106">Methods</span></span>
|<span data-ttu-id="6753e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6753e-107">Method</span></span>|<span data-ttu-id="6753e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6753e-108">Return Type</span></span>|<span data-ttu-id="6753e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6753e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6753e-110">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="6753e-110">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="6753e-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6753e-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="6753e-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6753e-112">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="6753e-113">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="6753e-113">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="6753e-114">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6753e-114">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="6753e-115">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6753e-115">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="6753e-116">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="6753e-116">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="6753e-117">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6753e-117">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="6753e-118">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6753e-118">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="6753e-119">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="6753e-119">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="6753e-120">なし</span><span class="sxs-lookup"><span data-stu-id="6753e-120">None</span></span>|<span data-ttu-id="6753e-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6753e-121">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="6753e-122">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="6753e-122">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="6753e-123">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6753e-123">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="6753e-124">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6753e-124">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6753e-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6753e-125">Properties</span></span>
|<span data-ttu-id="6753e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6753e-126">Property</span></span>|<span data-ttu-id="6753e-127">型</span><span class="sxs-lookup"><span data-stu-id="6753e-127">Type</span></span>|<span data-ttu-id="6753e-128">説明</span><span class="sxs-lookup"><span data-stu-id="6753e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6753e-129">id</span><span class="sxs-lookup"><span data-stu-id="6753e-129">id</span></span>|<span data-ttu-id="6753e-130">String</span><span class="sxs-lookup"><span data-stu-id="6753e-130">String</span></span>|<span data-ttu-id="6753e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6753e-131">Key of the entity.</span></span>|
|<span data-ttu-id="6753e-132">target</span><span class="sxs-lookup"><span data-stu-id="6753e-132">target</span></span>|[<span data-ttu-id="6753e-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6753e-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6753e-134">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="6753e-134">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6753e-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6753e-135">Relationships</span></span>
<span data-ttu-id="6753e-136">なし</span><span class="sxs-lookup"><span data-stu-id="6753e-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6753e-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6753e-137">JSON Representation</span></span>
<span data-ttu-id="6753e-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6753e-138">Here is a JSON representation of the resource.</span></span>
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


