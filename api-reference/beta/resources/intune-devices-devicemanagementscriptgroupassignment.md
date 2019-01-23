---
title: deviceManagementScriptGroupAssignment リソースの種類
description: デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ab4cdc6565841623c16bb46b0e0e36c01c68a9de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410575"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="d97e2-103">deviceManagementScriptGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d97e2-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="d97e2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d97e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d97e2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d97e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d97e2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d97e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d97e2-107">デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d97e2-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="d97e2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d97e2-108">Methods</span></span>
|<span data-ttu-id="d97e2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d97e2-109">Method</span></span>|<span data-ttu-id="d97e2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d97e2-110">Return Type</span></span>|<span data-ttu-id="d97e2-111">説明</span><span class="sxs-lookup"><span data-stu-id="d97e2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d97e2-112">リスト deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d97e2-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="d97e2-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d97e2-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="d97e2-114">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="d97e2-115">DeviceManagementScriptGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="d97e2-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d97e2-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="d97e2-117">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d97e2-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d97e2-118">DeviceManagementScriptGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="d97e2-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d97e2-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="d97e2-120">新しい[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d97e2-121">DeviceManagementScriptGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="d97e2-122">なし</span><span class="sxs-lookup"><span data-stu-id="d97e2-122">None</span></span>|<span data-ttu-id="d97e2-123">の[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="d97e2-124">DeviceManagementScriptGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="d97e2-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d97e2-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="d97e2-126">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d97e2-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d97e2-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d97e2-127">Properties</span></span>
|<span data-ttu-id="d97e2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d97e2-128">Property</span></span>|<span data-ttu-id="d97e2-129">型</span><span class="sxs-lookup"><span data-stu-id="d97e2-129">Type</span></span>|<span data-ttu-id="d97e2-130">説明</span><span class="sxs-lookup"><span data-stu-id="d97e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d97e2-131">id</span><span class="sxs-lookup"><span data-stu-id="d97e2-131">id</span></span>|<span data-ttu-id="d97e2-132">String</span><span class="sxs-lookup"><span data-stu-id="d97e2-132">String</span></span>|<span data-ttu-id="d97e2-133">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="d97e2-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d97e2-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d97e2-134">targetGroupId</span></span>|<span data-ttu-id="d97e2-135">String</span><span class="sxs-lookup"><span data-stu-id="d97e2-135">String</span></span>|<span data-ttu-id="d97e2-136">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="d97e2-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d97e2-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d97e2-137">Relationships</span></span>
<span data-ttu-id="d97e2-138">なし</span><span class="sxs-lookup"><span data-stu-id="d97e2-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d97e2-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d97e2-139">JSON Representation</span></span>
<span data-ttu-id="d97e2-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d97e2-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




