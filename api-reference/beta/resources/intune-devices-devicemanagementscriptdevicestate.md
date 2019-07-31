---
title: deviceManagementScriptDeviceState リソースの種類
description: デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a59754e92fc86cf635edaedb575ffa358875c64c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999844"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="8c905-103">deviceManagementScriptDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c905-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="8c905-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c905-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c905-106">デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8c905-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="8c905-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c905-107">Methods</span></span>
|<span data-ttu-id="8c905-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c905-108">Method</span></span>|<span data-ttu-id="8c905-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8c905-109">Return Type</span></span>|<span data-ttu-id="8c905-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c905-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c905-111">リスト deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="8c905-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="8c905-112">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c905-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="8c905-113">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8c905-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="8c905-114">DeviceManagementScriptDeviceState の取得</span><span class="sxs-lookup"><span data-stu-id="8c905-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="8c905-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8c905-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8c905-116">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8c905-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="8c905-117">DeviceManagementScriptDeviceState の作成</span><span class="sxs-lookup"><span data-stu-id="8c905-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="8c905-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8c905-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8c905-119">新しい[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c905-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="8c905-120">DeviceManagementScriptDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="8c905-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="8c905-121">None</span><span class="sxs-lookup"><span data-stu-id="8c905-121">None</span></span>|<span data-ttu-id="8c905-122">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8c905-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="8c905-123">DeviceManagementScriptDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="8c905-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="8c905-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8c905-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8c905-125">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c905-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c905-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c905-126">Properties</span></span>
|<span data-ttu-id="8c905-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c905-127">Property</span></span>|<span data-ttu-id="8c905-128">型</span><span class="sxs-lookup"><span data-stu-id="8c905-128">Type</span></span>|<span data-ttu-id="8c905-129">説明</span><span class="sxs-lookup"><span data-stu-id="8c905-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c905-130">id</span><span class="sxs-lookup"><span data-stu-id="8c905-130">id</span></span>|<span data-ttu-id="8c905-131">String</span><span class="sxs-lookup"><span data-stu-id="8c905-131">String</span></span>|<span data-ttu-id="8c905-132">デバイス管理スクリプトのデバイス状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8c905-132">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="8c905-133">runState</span><span class="sxs-lookup"><span data-stu-id="8c905-133">runState</span></span>|[<span data-ttu-id="8c905-134">runState</span><span class="sxs-lookup"><span data-stu-id="8c905-134">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8c905-135">デバイス管理スクリプトの最新の実行の状態。</span><span class="sxs-lookup"><span data-stu-id="8c905-135">State of latest run of the device management script.</span></span> <span data-ttu-id="8c905-136">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="8c905-136">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="8c905-137">resultMessage</span><span class="sxs-lookup"><span data-stu-id="8c905-137">resultMessage</span></span>|<span data-ttu-id="8c905-138">String</span><span class="sxs-lookup"><span data-stu-id="8c905-138">String</span></span>|<span data-ttu-id="8c905-139">実行出力の詳細。</span><span class="sxs-lookup"><span data-stu-id="8c905-139">Details of execution output.</span></span>|
|<span data-ttu-id="8c905-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8c905-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="8c905-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c905-141">DateTimeOffset</span></span>|<span data-ttu-id="8c905-142">デバイス管理スクリプトが最後に実行された時刻。</span><span class="sxs-lookup"><span data-stu-id="8c905-142">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="8c905-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="8c905-143">errorCode</span></span>|<span data-ttu-id="8c905-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8c905-144">Int32</span></span>|<span data-ttu-id="8c905-145">デバイス管理スクリプトの誤った実行に対応するエラーコード。</span><span class="sxs-lookup"><span data-stu-id="8c905-145">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="8c905-146">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8c905-146">errorDescription</span></span>|<span data-ttu-id="8c905-147">String</span><span class="sxs-lookup"><span data-stu-id="8c905-147">String</span></span>|<span data-ttu-id="8c905-148">デバイス管理スクリプトの誤った実行に対応するエラーの説明。</span><span class="sxs-lookup"><span data-stu-id="8c905-148">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c905-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c905-149">Relationships</span></span>
|<span data-ttu-id="8c905-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c905-150">Relationship</span></span>|<span data-ttu-id="8c905-151">型</span><span class="sxs-lookup"><span data-stu-id="8c905-151">Type</span></span>|<span data-ttu-id="8c905-152">説明</span><span class="sxs-lookup"><span data-stu-id="8c905-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c905-153">managedDevice</span><span class="sxs-lookup"><span data-stu-id="8c905-153">managedDevice</span></span>|[<span data-ttu-id="8c905-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="8c905-154">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="8c905-155">デバイス管理スクリプトを実行する管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="8c905-155">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c905-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c905-156">JSON Representation</span></span>
<span data-ttu-id="8c905-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c905-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```





