---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d327288ca08f43c36b20cefd8608b860529420
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252666"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="d57b4-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d57b4-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="d57b4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d57b4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57b4-105">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="d57b4-105">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="d57b4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d57b4-106">Methods</span></span>
|<span data-ttu-id="d57b4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d57b4-107">Method</span></span>|<span data-ttu-id="d57b4-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d57b4-108">Return Type</span></span>|<span data-ttu-id="d57b4-109">説明</span><span class="sxs-lookup"><span data-stu-id="d57b4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d57b4-110">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="d57b4-110">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="d57b4-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d57b4-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d57b4-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d57b4-112">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="d57b4-113">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="d57b4-113">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="d57b4-114">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d57b4-114">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d57b4-115">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d57b4-115">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d57b4-116">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="d57b4-116">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="d57b4-117">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d57b4-117">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d57b4-118">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d57b4-118">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d57b4-119">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="d57b4-119">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="d57b4-120">なし</span><span class="sxs-lookup"><span data-stu-id="d57b4-120">None</span></span>|<span data-ttu-id="d57b4-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d57b4-121">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="d57b4-122">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="d57b4-122">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="d57b4-123">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d57b4-123">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d57b4-124">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d57b4-124">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d57b4-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d57b4-125">Properties</span></span>
|<span data-ttu-id="d57b4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d57b4-126">Property</span></span>|<span data-ttu-id="d57b4-127">型</span><span class="sxs-lookup"><span data-stu-id="d57b4-127">Type</span></span>|<span data-ttu-id="d57b4-128">説明</span><span class="sxs-lookup"><span data-stu-id="d57b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57b4-129">id</span><span class="sxs-lookup"><span data-stu-id="d57b4-129">id</span></span>|<span data-ttu-id="d57b4-130">String</span><span class="sxs-lookup"><span data-stu-id="d57b4-130">String</span></span>|<span data-ttu-id="d57b4-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d57b4-131">Key of the entity.</span></span>|
|<span data-ttu-id="d57b4-132">target</span><span class="sxs-lookup"><span data-stu-id="d57b4-132">target</span></span>|[<span data-ttu-id="d57b4-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d57b4-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d57b4-134">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="d57b4-134">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d57b4-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d57b4-135">Relationships</span></span>
<span data-ttu-id="d57b4-136">なし</span><span class="sxs-lookup"><span data-stu-id="d57b4-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d57b4-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d57b4-137">JSON Representation</span></span>
<span data-ttu-id="d57b4-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d57b4-138">Here is a JSON representation of the resource.</span></span>
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



