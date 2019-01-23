---
title: deviceManagementScriptAssignment リソースの種類
description: デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6e153842e0b820a845260bc125154df7cef0cb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413851"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="14cbd-103">deviceManagementScriptAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14cbd-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="14cbd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14cbd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14cbd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14cbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14cbd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14cbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14cbd-107">デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="14cbd-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="14cbd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14cbd-108">Methods</span></span>
|<span data-ttu-id="14cbd-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="14cbd-109">Method</span></span>|<span data-ttu-id="14cbd-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14cbd-110">Return Type</span></span>|<span data-ttu-id="14cbd-111">説明</span><span class="sxs-lookup"><span data-stu-id="14cbd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14cbd-112">リスト deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="14cbd-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="14cbd-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14cbd-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="14cbd-114">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="14cbd-115">DeviceManagementScriptAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="14cbd-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="14cbd-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="14cbd-117">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14cbd-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="14cbd-118">DeviceManagementScriptAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="14cbd-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="14cbd-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="14cbd-120">新しい[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="14cbd-121">DeviceManagementScriptAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="14cbd-122">なし</span><span class="sxs-lookup"><span data-stu-id="14cbd-122">None</span></span>|<span data-ttu-id="14cbd-123">の[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="14cbd-124">DeviceManagementScriptAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="14cbd-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="14cbd-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="14cbd-126">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="14cbd-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14cbd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14cbd-127">Properties</span></span>
|<span data-ttu-id="14cbd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14cbd-128">Property</span></span>|<span data-ttu-id="14cbd-129">型</span><span class="sxs-lookup"><span data-stu-id="14cbd-129">Type</span></span>|<span data-ttu-id="14cbd-130">説明</span><span class="sxs-lookup"><span data-stu-id="14cbd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cbd-131">id</span><span class="sxs-lookup"><span data-stu-id="14cbd-131">id</span></span>|<span data-ttu-id="14cbd-132">String</span><span class="sxs-lookup"><span data-stu-id="14cbd-132">String</span></span>|<span data-ttu-id="14cbd-133">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="14cbd-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="14cbd-134">target</span><span class="sxs-lookup"><span data-stu-id="14cbd-134">target</span></span>|[<span data-ttu-id="14cbd-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="14cbd-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="14cbd-136">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="14cbd-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cbd-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14cbd-137">Relationships</span></span>
<span data-ttu-id="14cbd-138">なし</span><span class="sxs-lookup"><span data-stu-id="14cbd-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14cbd-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14cbd-139">JSON Representation</span></span>
<span data-ttu-id="14cbd-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14cbd-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




