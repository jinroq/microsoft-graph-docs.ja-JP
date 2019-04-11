---
title: devicemanagementscriptdevicestate リソースの種類
description: デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b985b7641d66c806acc544174fffff4a2216421a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784958"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="3a42e-103">devicemanagementscriptdevicestate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a42e-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="3a42e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a42e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a42e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a42e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a42e-106">デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3a42e-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="3a42e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3a42e-107">Methods</span></span>
|<span data-ttu-id="3a42e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3a42e-108">Method</span></span>|<span data-ttu-id="3a42e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3a42e-109">Return Type</span></span>|<span data-ttu-id="3a42e-110">説明</span><span class="sxs-lookup"><span data-stu-id="3a42e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a42e-111">リスト deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="3a42e-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="3a42e-112">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3a42e-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="3a42e-113">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3a42e-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="3a42e-114">devicemanagementscriptdevicestate の取得</span><span class="sxs-lookup"><span data-stu-id="3a42e-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="3a42e-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3a42e-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="3a42e-116">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3a42e-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="3a42e-117">devicemanagementscriptdevicestate の作成</span><span class="sxs-lookup"><span data-stu-id="3a42e-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="3a42e-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3a42e-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="3a42e-119">新しい[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3a42e-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="3a42e-120">devicemanagementscriptdevicestate の削除</span><span class="sxs-lookup"><span data-stu-id="3a42e-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="3a42e-121">なし</span><span class="sxs-lookup"><span data-stu-id="3a42e-121">None</span></span>|<span data-ttu-id="3a42e-122">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3a42e-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="3a42e-123">devicemanagementscriptdevicestate の更新</span><span class="sxs-lookup"><span data-stu-id="3a42e-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="3a42e-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3a42e-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="3a42e-125">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3a42e-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a42e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a42e-126">Properties</span></span>
|<span data-ttu-id="3a42e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a42e-127">Property</span></span>|<span data-ttu-id="3a42e-128">型</span><span class="sxs-lookup"><span data-stu-id="3a42e-128">Type</span></span>|<span data-ttu-id="3a42e-129">説明</span><span class="sxs-lookup"><span data-stu-id="3a42e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a42e-130">id</span><span class="sxs-lookup"><span data-stu-id="3a42e-130">id</span></span>|<span data-ttu-id="3a42e-131">String</span><span class="sxs-lookup"><span data-stu-id="3a42e-131">String</span></span>|<span data-ttu-id="3a42e-132">デバイス管理スクリプトのデバイス状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3a42e-132">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="3a42e-133">runstate</span><span class="sxs-lookup"><span data-stu-id="3a42e-133">runState</span></span>|[<span data-ttu-id="3a42e-134">runstate</span><span class="sxs-lookup"><span data-stu-id="3a42e-134">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3a42e-135">デバイス管理スクリプトの最新の実行の状態。</span><span class="sxs-lookup"><span data-stu-id="3a42e-135">State of latest run of the device management script.</span></span> <span data-ttu-id="3a42e-136">使用可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="3a42e-136">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="3a42e-137">resultmessage</span><span class="sxs-lookup"><span data-stu-id="3a42e-137">resultMessage</span></span>|<span data-ttu-id="3a42e-138">文字列</span><span class="sxs-lookup"><span data-stu-id="3a42e-138">String</span></span>|<span data-ttu-id="3a42e-139">実行出力の詳細。</span><span class="sxs-lookup"><span data-stu-id="3a42e-139">Details of execution output.</span></span>|
|<span data-ttu-id="3a42e-140">laststateupdatedatetime</span><span class="sxs-lookup"><span data-stu-id="3a42e-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="3a42e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a42e-141">DateTimeOffset</span></span>|<span data-ttu-id="3a42e-142">デバイス管理スクリプトが最後に実行された時刻。</span><span class="sxs-lookup"><span data-stu-id="3a42e-142">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="3a42e-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="3a42e-143">errorCode</span></span>|<span data-ttu-id="3a42e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3a42e-144">Int32</span></span>|<span data-ttu-id="3a42e-145">デバイス管理スクリプトの誤った実行に対応するエラーコード。</span><span class="sxs-lookup"><span data-stu-id="3a42e-145">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="3a42e-146">errorDescription</span><span class="sxs-lookup"><span data-stu-id="3a42e-146">errorDescription</span></span>|<span data-ttu-id="3a42e-147">String</span><span class="sxs-lookup"><span data-stu-id="3a42e-147">String</span></span>|<span data-ttu-id="3a42e-148">デバイス管理スクリプトの誤った実行に対応するエラーの説明。</span><span class="sxs-lookup"><span data-stu-id="3a42e-148">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a42e-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a42e-149">Relationships</span></span>
|<span data-ttu-id="3a42e-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a42e-150">Relationship</span></span>|<span data-ttu-id="3a42e-151">型</span><span class="sxs-lookup"><span data-stu-id="3a42e-151">Type</span></span>|<span data-ttu-id="3a42e-152">説明</span><span class="sxs-lookup"><span data-stu-id="3a42e-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a42e-153">managedDevice</span><span class="sxs-lookup"><span data-stu-id="3a42e-153">managedDevice</span></span>|[<span data-ttu-id="3a42e-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="3a42e-154">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="3a42e-155">デバイス管理スクリプトを実行する管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="3a42e-155">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a42e-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a42e-156">JSON Representation</span></span>
<span data-ttu-id="3a42e-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a42e-157">Here is a JSON representation of the resource.</span></span>
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





