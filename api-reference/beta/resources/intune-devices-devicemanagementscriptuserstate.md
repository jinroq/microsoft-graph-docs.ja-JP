---
title: deviceManagementScriptUserState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1884967707be8e126724148afa5d04b07f80a48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407285"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="2d7d0-103">deviceManagementScriptUserState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d7d0-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="2d7d0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d7d0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d7d0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d7d0-107">状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-107">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="2d7d0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d7d0-108">Methods</span></span>
|<span data-ttu-id="2d7d0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d7d0-109">Method</span></span>|<span data-ttu-id="2d7d0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2d7d0-110">Return Type</span></span>|<span data-ttu-id="2d7d0-111">説明</span><span class="sxs-lookup"><span data-stu-id="2d7d0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d7d0-112">リスト deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="2d7d0-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="2d7d0-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2d7d0-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="2d7d0-114">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="2d7d0-115">DeviceManagementScriptUserState を取得します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="2d7d0-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="2d7d0-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="2d7d0-117">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="2d7d0-118">DeviceManagementScriptUserState を作成します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="2d7d0-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="2d7d0-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="2d7d0-120">新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="2d7d0-121">DeviceManagementScriptUserState を削除します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="2d7d0-122">なし</span><span class="sxs-lookup"><span data-stu-id="2d7d0-122">None</span></span>|<span data-ttu-id="2d7d0-123">の[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="2d7d0-124">DeviceManagementScriptUserState を更新します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="2d7d0-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="2d7d0-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="2d7d0-126">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d7d0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d7d0-127">Properties</span></span>
|<span data-ttu-id="2d7d0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d7d0-128">Property</span></span>|<span data-ttu-id="2d7d0-129">型</span><span class="sxs-lookup"><span data-stu-id="2d7d0-129">Type</span></span>|<span data-ttu-id="2d7d0-130">説明</span><span class="sxs-lookup"><span data-stu-id="2d7d0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d7d0-131">id</span><span class="sxs-lookup"><span data-stu-id="2d7d0-131">id</span></span>|<span data-ttu-id="2d7d0-132">String</span><span class="sxs-lookup"><span data-stu-id="2d7d0-132">String</span></span>|<span data-ttu-id="2d7d0-133">デバイス管理スクリプト ユーザー状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-133">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="2d7d0-134">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7d0-134">successDeviceCount</span></span>|<span data-ttu-id="2d7d0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7d0-135">Int32</span></span>|<span data-ttu-id="2d7d0-136">デバイスの数の特定のユーザーに成功します。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-136">Success device count for specific user.</span></span>|
|<span data-ttu-id="2d7d0-137">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7d0-137">errorDeviceCount</span></span>|<span data-ttu-id="2d7d0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7d0-138">Int32</span></span>|<span data-ttu-id="2d7d0-139">特定のユーザー エラー デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-139">Error device count for specific user.</span></span>|
|<span data-ttu-id="2d7d0-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d7d0-140">userPrincipalName</span></span>|<span data-ttu-id="2d7d0-141">String</span><span class="sxs-lookup"><span data-stu-id="2d7d0-141">String</span></span>|<span data-ttu-id="2d7d0-142">特定のユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-142">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d7d0-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d7d0-143">Relationships</span></span>
|<span data-ttu-id="2d7d0-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d7d0-144">Relationship</span></span>|<span data-ttu-id="2d7d0-145">型</span><span class="sxs-lookup"><span data-stu-id="2d7d0-145">Type</span></span>|<span data-ttu-id="2d7d0-146">説明</span><span class="sxs-lookup"><span data-stu-id="2d7d0-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d7d0-147">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="2d7d0-147">deviceRunStates</span></span>|<span data-ttu-id="2d7d0-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2d7d0-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="2d7d0-149">特定のユーザーのすべてのデバイスでは、このスクリプトの実行状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-149">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d7d0-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d7d0-150">JSON Representation</span></span>
<span data-ttu-id="2d7d0-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d7d0-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```




