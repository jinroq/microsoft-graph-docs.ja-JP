---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d327288ca08f43c36b20cefd8608b860529420
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534249"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="e1625-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1625-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="e1625-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1625-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1625-105">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="e1625-105">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="e1625-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1625-106">Methods</span></span>
|<span data-ttu-id="e1625-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1625-107">Method</span></span>|<span data-ttu-id="e1625-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1625-108">Return Type</span></span>|<span data-ttu-id="e1625-109">説明</span><span class="sxs-lookup"><span data-stu-id="e1625-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1625-110">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="e1625-110">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="e1625-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1625-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="e1625-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e1625-112">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="e1625-113">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="e1625-113">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="e1625-114">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e1625-114">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e1625-115">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1625-115">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="e1625-116">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="e1625-116">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="e1625-117">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e1625-117">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e1625-118">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1625-118">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="e1625-119">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="e1625-119">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="e1625-120">なし</span><span class="sxs-lookup"><span data-stu-id="e1625-120">None</span></span>|<span data-ttu-id="e1625-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e1625-121">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="e1625-122">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e1625-122">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="e1625-123">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e1625-123">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e1625-124">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e1625-124">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1625-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1625-125">Properties</span></span>
|<span data-ttu-id="e1625-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1625-126">Property</span></span>|<span data-ttu-id="e1625-127">型</span><span class="sxs-lookup"><span data-stu-id="e1625-127">Type</span></span>|<span data-ttu-id="e1625-128">説明</span><span class="sxs-lookup"><span data-stu-id="e1625-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1625-129">id</span><span class="sxs-lookup"><span data-stu-id="e1625-129">id</span></span>|<span data-ttu-id="e1625-130">String</span><span class="sxs-lookup"><span data-stu-id="e1625-130">String</span></span>|<span data-ttu-id="e1625-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e1625-131">Key of the entity.</span></span>|
|<span data-ttu-id="e1625-132">target</span><span class="sxs-lookup"><span data-stu-id="e1625-132">target</span></span>|[<span data-ttu-id="e1625-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e1625-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e1625-134">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="e1625-134">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1625-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1625-135">Relationships</span></span>
<span data-ttu-id="e1625-136">なし</span><span class="sxs-lookup"><span data-stu-id="e1625-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1625-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1625-137">JSON Representation</span></span>
<span data-ttu-id="e1625-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1625-138">Here is a JSON representation of the resource.</span></span>
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



