---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aae3cc295c031c1f2045d39b45084e2577f39755
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155749"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="ffcb0-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ffcb0-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="ffcb0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffcb0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffcb0-106">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="ffcb0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ffcb0-107">Methods</span></span>
|<span data-ttu-id="ffcb0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ffcb0-108">Method</span></span>|<span data-ttu-id="ffcb0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ffcb0-109">Return Type</span></span>|<span data-ttu-id="ffcb0-110">説明</span><span class="sxs-lookup"><span data-stu-id="ffcb0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ffcb0-111">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ffcb0-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="ffcb0-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ffcb0-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="ffcb0-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="ffcb0-114">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="ffcb0-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="ffcb0-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcb0-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="ffcb0-116">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="ffcb0-117">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ffcb0-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="ffcb0-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcb0-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="ffcb0-119">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="ffcb0-120">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="ffcb0-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="ffcb0-121">なし</span><span class="sxs-lookup"><span data-stu-id="ffcb0-121">None</span></span>|<span data-ttu-id="ffcb0-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="ffcb0-123">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="ffcb0-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="ffcb0-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcb0-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="ffcb0-125">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ffcb0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffcb0-126">Properties</span></span>
|<span data-ttu-id="ffcb0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffcb0-127">Property</span></span>|<span data-ttu-id="ffcb0-128">型</span><span class="sxs-lookup"><span data-stu-id="ffcb0-128">Type</span></span>|<span data-ttu-id="ffcb0-129">説明</span><span class="sxs-lookup"><span data-stu-id="ffcb0-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffcb0-130">id</span><span class="sxs-lookup"><span data-stu-id="ffcb0-130">id</span></span>|<span data-ttu-id="ffcb0-131">String</span><span class="sxs-lookup"><span data-stu-id="ffcb0-131">String</span></span>|<span data-ttu-id="ffcb0-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-132">Key of the entity.</span></span>|
|<span data-ttu-id="ffcb0-133">target</span><span class="sxs-lookup"><span data-stu-id="ffcb0-133">target</span></span>|[<span data-ttu-id="ffcb0-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ffcb0-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ffcb0-135">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-135">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffcb0-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ffcb0-136">Relationships</span></span>
<span data-ttu-id="ffcb0-137">なし</span><span class="sxs-lookup"><span data-stu-id="ffcb0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffcb0-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ffcb0-138">JSON Representation</span></span>
<span data-ttu-id="ffcb0-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ffcb0-139">Here is a JSON representation of the resource.</span></span>
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




