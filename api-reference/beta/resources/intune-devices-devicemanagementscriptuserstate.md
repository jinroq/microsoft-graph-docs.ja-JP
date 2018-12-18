---
title: deviceManagementScriptUserState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: acce3d40d390c22d848b9ee3f8c94c997ae6da12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301212"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="0db9b-103">deviceManagementScriptUserState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0db9b-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="0db9b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0db9b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0db9b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0db9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0db9b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0db9b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0db9b-107">状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9b-107">Contains properties for user run state of the device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="0db9b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0db9b-108">Methods</span></span>
|<span data-ttu-id="0db9b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0db9b-109">Method</span></span>|<span data-ttu-id="0db9b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0db9b-110">Return Type</span></span>|<span data-ttu-id="0db9b-111">説明</span><span class="sxs-lookup"><span data-stu-id="0db9b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0db9b-112">リスト deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="0db9b-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="0db9b-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0db9b-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="0db9b-114">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="0db9b-115">DeviceManagementScriptUserState を取得します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="0db9b-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="0db9b-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="0db9b-117">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0db9b-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="0db9b-118">DeviceManagementScriptUserState を作成します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="0db9b-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="0db9b-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="0db9b-120">新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="0db9b-121">DeviceManagementScriptUserState を削除します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="0db9b-122">なし</span><span class="sxs-lookup"><span data-stu-id="0db9b-122">None</span></span>|<span data-ttu-id="0db9b-123">の[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="0db9b-124">DeviceManagementScriptUserState を更新します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="0db9b-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="0db9b-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="0db9b-126">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0db9b-127">Properties</span><span class="sxs-lookup"><span data-stu-id="0db9b-127">Properties</span></span>
|<span data-ttu-id="0db9b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0db9b-128">Property</span></span>|<span data-ttu-id="0db9b-129">種類</span><span class="sxs-lookup"><span data-stu-id="0db9b-129">Type</span></span>|<span data-ttu-id="0db9b-130">説明</span><span class="sxs-lookup"><span data-stu-id="0db9b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db9b-131">ID</span><span class="sxs-lookup"><span data-stu-id="0db9b-131">id</span></span>|<span data-ttu-id="0db9b-132">String</span><span class="sxs-lookup"><span data-stu-id="0db9b-132">String</span></span>|<span data-ttu-id="0db9b-133">デバイス管理スクリプト ユーザー状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="0db9b-133">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="0db9b-134">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0db9b-134">successDeviceCount</span></span>|<span data-ttu-id="0db9b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0db9b-135">Int32</span></span>|<span data-ttu-id="0db9b-136">デバイスの数の特定のユーザーに成功します。</span><span class="sxs-lookup"><span data-stu-id="0db9b-136">Success device count for specific user.</span></span>|
|<span data-ttu-id="0db9b-137">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0db9b-137">errorDeviceCount</span></span>|<span data-ttu-id="0db9b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0db9b-138">Int32</span></span>|<span data-ttu-id="0db9b-139">特定のユーザー エラー デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0db9b-139">Error device count for specific user.</span></span>|
|<span data-ttu-id="0db9b-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0db9b-140">userPrincipalName</span></span>|<span data-ttu-id="0db9b-141">String</span><span class="sxs-lookup"><span data-stu-id="0db9b-141">String</span></span>|<span data-ttu-id="0db9b-142">特定のユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="0db9b-142">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db9b-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0db9b-143">Relationships</span></span>
|<span data-ttu-id="0db9b-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0db9b-144">Relationship</span></span>|<span data-ttu-id="0db9b-145">型</span><span class="sxs-lookup"><span data-stu-id="0db9b-145">Type</span></span>|<span data-ttu-id="0db9b-146">説明</span><span class="sxs-lookup"><span data-stu-id="0db9b-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db9b-147">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="0db9b-147">deviceRunStates</span></span>|<span data-ttu-id="0db9b-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0db9b-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="0db9b-149">特定のユーザーのすべてのデバイスでは、このスクリプトの実行状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="0db9b-149">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0db9b-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0db9b-150">JSON Representation</span></span>
<span data-ttu-id="0db9b-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0db9b-151">Here is a JSON representation of the resource.</span></span>
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





