---
title: deviceManagementScriptDeviceState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するデバイスのプロパティが含まれています。
ms.openlocfilehash: 11c9e574e880df371f45181dd02fdb2292d0cb15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074259"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="8d16b-103">deviceManagementScriptDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d16b-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="8d16b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d16b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d16b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d16b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d16b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d16b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d16b-107">状態のデバイスの管理スクリプトを実行するデバイスのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d16b-107">Contains properties for device run state of the device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="8d16b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8d16b-108">Methods</span></span>
|<span data-ttu-id="8d16b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8d16b-109">Method</span></span>|<span data-ttu-id="8d16b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8d16b-110">Return Type</span></span>|<span data-ttu-id="8d16b-111">説明</span><span class="sxs-lookup"><span data-stu-id="8d16b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8d16b-112">リスト deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="8d16b-112">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="8d16b-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8d16b-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="8d16b-114">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-114">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="8d16b-115">DeviceManagementScriptDeviceState を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-115">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="8d16b-116">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8d16b-116">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8d16b-117">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d16b-117">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="8d16b-118">DeviceManagementScriptDeviceState を作成します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-118">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="8d16b-119">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8d16b-119">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8d16b-120">新しい[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-120">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="8d16b-121">DeviceManagementScriptDeviceState を削除します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-121">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="8d16b-122">なし</span><span class="sxs-lookup"><span data-stu-id="8d16b-122">None</span></span>|<span data-ttu-id="8d16b-123">の[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-123">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="8d16b-124">DeviceManagementScriptDeviceState を更新します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-124">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="8d16b-125">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="8d16b-125">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="8d16b-126">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-126">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d16b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d16b-127">Properties</span></span>
|<span data-ttu-id="8d16b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d16b-128">Property</span></span>|<span data-ttu-id="8d16b-129">型</span><span class="sxs-lookup"><span data-stu-id="8d16b-129">Type</span></span>|<span data-ttu-id="8d16b-130">説明</span><span class="sxs-lookup"><span data-stu-id="8d16b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d16b-131">id</span><span class="sxs-lookup"><span data-stu-id="8d16b-131">id</span></span>|<span data-ttu-id="8d16b-132">String</span><span class="sxs-lookup"><span data-stu-id="8d16b-132">String</span></span>|<span data-ttu-id="8d16b-133">デバイス管理スクリプト デバイス状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="8d16b-133">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="8d16b-134">runState</span><span class="sxs-lookup"><span data-stu-id="8d16b-134">runState</span></span>|[<span data-ttu-id="8d16b-135">runState</span><span class="sxs-lookup"><span data-stu-id="8d16b-135">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8d16b-136">デバイス管理スクリプトの実行を最新の状態です。</span><span class="sxs-lookup"><span data-stu-id="8d16b-136">State of latest run of the device management script.</span></span> <span data-ttu-id="8d16b-137">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="8d16b-137">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="8d16b-138">resultMessage</span><span class="sxs-lookup"><span data-stu-id="8d16b-138">resultMessage</span></span>|<span data-ttu-id="8d16b-139">String</span><span class="sxs-lookup"><span data-stu-id="8d16b-139">String</span></span>|<span data-ttu-id="8d16b-140">実行結果の詳細です。</span><span class="sxs-lookup"><span data-stu-id="8d16b-140">Details of execution output.</span></span>|
|<span data-ttu-id="8d16b-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8d16b-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="8d16b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d16b-142">DateTimeOffset</span></span>|<span data-ttu-id="8d16b-143">最新の時間、デバイスの管理スクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="8d16b-143">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="8d16b-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="8d16b-144">errorCode</span></span>|<span data-ttu-id="8d16b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8d16b-145">Int32</span></span>|<span data-ttu-id="8d16b-146">デバイス管理スクリプトの実行がエラーに対応するエラー ・ コードです。</span><span class="sxs-lookup"><span data-stu-id="8d16b-146">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="8d16b-147">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8d16b-147">errorDescription</span></span>|<span data-ttu-id="8d16b-148">String</span><span class="sxs-lookup"><span data-stu-id="8d16b-148">String</span></span>|<span data-ttu-id="8d16b-149">デバイス管理スクリプトの実行がエラーに対応するエラーの説明です。</span><span class="sxs-lookup"><span data-stu-id="8d16b-149">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d16b-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d16b-150">Relationships</span></span>
|<span data-ttu-id="8d16b-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d16b-151">Relationship</span></span>|<span data-ttu-id="8d16b-152">型</span><span class="sxs-lookup"><span data-stu-id="8d16b-152">Type</span></span>|<span data-ttu-id="8d16b-153">説明</span><span class="sxs-lookup"><span data-stu-id="8d16b-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d16b-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="8d16b-154">managedDevice</span></span>|[<span data-ttu-id="8d16b-155">managedDevice</span><span class="sxs-lookup"><span data-stu-id="8d16b-155">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="8d16b-156">デバイスの管理スクリプトを実行する管理対象のデバイスです。</span><span class="sxs-lookup"><span data-stu-id="8d16b-156">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d16b-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d16b-157">JSON Representation</span></span>
<span data-ttu-id="8d16b-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d16b-158">Here is a JSON representation of the resource.</span></span>
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





