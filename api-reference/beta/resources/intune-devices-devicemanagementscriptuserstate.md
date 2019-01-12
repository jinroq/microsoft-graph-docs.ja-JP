---
title: deviceManagementScriptUserState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d74e8276603355af58ccff50401f742c56147d7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942249"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="86e21-103">deviceManagementScriptUserState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86e21-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="86e21-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86e21-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86e21-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86e21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86e21-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86e21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86e21-107">状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="86e21-107">Contains properties for user run state of the device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="86e21-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="86e21-108">Methods</span></span>
|<span data-ttu-id="86e21-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="86e21-109">Method</span></span>|<span data-ttu-id="86e21-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86e21-110">Return Type</span></span>|<span data-ttu-id="86e21-111">説明</span><span class="sxs-lookup"><span data-stu-id="86e21-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86e21-112">リスト deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="86e21-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="86e21-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86e21-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="86e21-114">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="86e21-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="86e21-115">DeviceManagementScriptUserState を取得します。</span><span class="sxs-lookup"><span data-stu-id="86e21-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="86e21-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="86e21-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="86e21-117">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86e21-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="86e21-118">DeviceManagementScriptUserState を作成します。</span><span class="sxs-lookup"><span data-stu-id="86e21-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="86e21-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="86e21-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="86e21-120">新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="86e21-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="86e21-121">DeviceManagementScriptUserState を削除します。</span><span class="sxs-lookup"><span data-stu-id="86e21-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="86e21-122">なし</span><span class="sxs-lookup"><span data-stu-id="86e21-122">None</span></span>|<span data-ttu-id="86e21-123">の[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="86e21-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="86e21-124">DeviceManagementScriptUserState を更新します。</span><span class="sxs-lookup"><span data-stu-id="86e21-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="86e21-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="86e21-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="86e21-126">[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="86e21-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86e21-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86e21-127">Properties</span></span>
|<span data-ttu-id="86e21-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86e21-128">Property</span></span>|<span data-ttu-id="86e21-129">種類</span><span class="sxs-lookup"><span data-stu-id="86e21-129">Type</span></span>|<span data-ttu-id="86e21-130">説明</span><span class="sxs-lookup"><span data-stu-id="86e21-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86e21-131">ID</span><span class="sxs-lookup"><span data-stu-id="86e21-131">id</span></span>|<span data-ttu-id="86e21-132">String</span><span class="sxs-lookup"><span data-stu-id="86e21-132">String</span></span>|<span data-ttu-id="86e21-133">デバイス管理スクリプト ユーザー状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="86e21-133">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="86e21-134">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86e21-134">successDeviceCount</span></span>|<span data-ttu-id="86e21-135">Int32</span><span class="sxs-lookup"><span data-stu-id="86e21-135">Int32</span></span>|<span data-ttu-id="86e21-136">デバイスの数の特定のユーザーに成功します。</span><span class="sxs-lookup"><span data-stu-id="86e21-136">Success device count for specific user.</span></span>|
|<span data-ttu-id="86e21-137">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86e21-137">errorDeviceCount</span></span>|<span data-ttu-id="86e21-138">Int32</span><span class="sxs-lookup"><span data-stu-id="86e21-138">Int32</span></span>|<span data-ttu-id="86e21-139">特定のユーザー エラー デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="86e21-139">Error device count for specific user.</span></span>|
|<span data-ttu-id="86e21-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86e21-140">userPrincipalName</span></span>|<span data-ttu-id="86e21-141">String</span><span class="sxs-lookup"><span data-stu-id="86e21-141">String</span></span>|<span data-ttu-id="86e21-142">特定のユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="86e21-142">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86e21-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86e21-143">Relationships</span></span>
|<span data-ttu-id="86e21-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86e21-144">Relationship</span></span>|<span data-ttu-id="86e21-145">型</span><span class="sxs-lookup"><span data-stu-id="86e21-145">Type</span></span>|<span data-ttu-id="86e21-146">説明</span><span class="sxs-lookup"><span data-stu-id="86e21-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86e21-147">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="86e21-147">deviceRunStates</span></span>|<span data-ttu-id="86e21-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86e21-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="86e21-149">特定のユーザーのすべてのデバイスでは、このスクリプトの実行状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="86e21-149">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86e21-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86e21-150">JSON Representation</span></span>
<span data-ttu-id="86e21-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86e21-151">Here is a JSON representation of the resource.</span></span>
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





