---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb90240e83bb3e811b0eff09966346f801a1637
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415608"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="cf13c-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf13c-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="cf13c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf13c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf13c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf13c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf13c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf13c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf13c-107">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="cf13c-107">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="cf13c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf13c-108">Methods</span></span>
|<span data-ttu-id="cf13c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf13c-109">Method</span></span>|<span data-ttu-id="cf13c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cf13c-110">Return Type</span></span>|<span data-ttu-id="cf13c-111">説明</span><span class="sxs-lookup"><span data-stu-id="cf13c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf13c-112">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="cf13c-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="cf13c-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf13c-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="cf13c-114">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cf13c-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="cf13c-115">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="cf13c-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="cf13c-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cf13c-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="cf13c-117">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cf13c-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="cf13c-118">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="cf13c-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="cf13c-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cf13c-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="cf13c-120">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf13c-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="cf13c-121">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="cf13c-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="cf13c-122">なし</span><span class="sxs-lookup"><span data-stu-id="cf13c-122">None</span></span>|<span data-ttu-id="cf13c-123">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="cf13c-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="cf13c-124">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="cf13c-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="cf13c-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cf13c-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="cf13c-126">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf13c-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf13c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf13c-127">Properties</span></span>
|<span data-ttu-id="cf13c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf13c-128">Property</span></span>|<span data-ttu-id="cf13c-129">型</span><span class="sxs-lookup"><span data-stu-id="cf13c-129">Type</span></span>|<span data-ttu-id="cf13c-130">説明</span><span class="sxs-lookup"><span data-stu-id="cf13c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf13c-131">id</span><span class="sxs-lookup"><span data-stu-id="cf13c-131">id</span></span>|<span data-ttu-id="cf13c-132">String</span><span class="sxs-lookup"><span data-stu-id="cf13c-132">String</span></span>|<span data-ttu-id="cf13c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf13c-133">Key of the entity.</span></span>|
|<span data-ttu-id="cf13c-134">target</span><span class="sxs-lookup"><span data-stu-id="cf13c-134">target</span></span>|[<span data-ttu-id="cf13c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cf13c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cf13c-136">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="cf13c-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf13c-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf13c-137">Relationships</span></span>
<span data-ttu-id="cf13c-138">なし</span><span class="sxs-lookup"><span data-stu-id="cf13c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf13c-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf13c-139">JSON Representation</span></span>
<span data-ttu-id="cf13c-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf13c-140">Here is a JSON representation of the resource.</span></span>
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




