---
title: devicemanagementscriptuserstate リソースの種類
description: デバイス管理スクリプトのユーザー実行状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2476329a402e0d6a50594ab110e88da4b5f5ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522406"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="c0b72-103">devicemanagementscriptuserstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0b72-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="c0b72-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0b72-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0b72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0b72-106">デバイス管理スクリプトのユーザー実行状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0b72-106">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="c0b72-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0b72-107">Methods</span></span>
|<span data-ttu-id="c0b72-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0b72-108">Method</span></span>|<span data-ttu-id="c0b72-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c0b72-109">Return Type</span></span>|<span data-ttu-id="c0b72-110">説明</span><span class="sxs-lookup"><span data-stu-id="c0b72-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0b72-111">devicemanagementscriptuserstates のリスト</span><span class="sxs-lookup"><span data-stu-id="c0b72-111">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="c0b72-112">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b72-112">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="c0b72-113">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c0b72-113">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="c0b72-114">devicemanagementscriptuserstate の取得</span><span class="sxs-lookup"><span data-stu-id="c0b72-114">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="c0b72-115">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c0b72-115">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c0b72-116">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c0b72-116">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="c0b72-117">devicemanagementscriptuserstate の作成</span><span class="sxs-lookup"><span data-stu-id="c0b72-117">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="c0b72-118">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c0b72-118">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c0b72-119">新しい[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c0b72-119">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="c0b72-120">devicemanagementscriptuserstate の削除</span><span class="sxs-lookup"><span data-stu-id="c0b72-120">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="c0b72-121">なし</span><span class="sxs-lookup"><span data-stu-id="c0b72-121">None</span></span>|<span data-ttu-id="c0b72-122">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c0b72-122">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="c0b72-123">devicemanagementscriptuserstate の更新</span><span class="sxs-lookup"><span data-stu-id="c0b72-123">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="c0b72-124">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c0b72-124">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c0b72-125">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0b72-125">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0b72-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b72-126">Properties</span></span>
|<span data-ttu-id="c0b72-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b72-127">Property</span></span>|<span data-ttu-id="c0b72-128">型</span><span class="sxs-lookup"><span data-stu-id="c0b72-128">Type</span></span>|<span data-ttu-id="c0b72-129">説明</span><span class="sxs-lookup"><span data-stu-id="c0b72-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b72-130">id</span><span class="sxs-lookup"><span data-stu-id="c0b72-130">id</span></span>|<span data-ttu-id="c0b72-131">String</span><span class="sxs-lookup"><span data-stu-id="c0b72-131">String</span></span>|<span data-ttu-id="c0b72-132">デバイス管理スクリプトのユーザー状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0b72-132">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="c0b72-133">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c0b72-133">successDeviceCount</span></span>|<span data-ttu-id="c0b72-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b72-134">Int32</span></span>|<span data-ttu-id="c0b72-135">特定のユーザーの成功デバイス数。</span><span class="sxs-lookup"><span data-stu-id="c0b72-135">Success device count for specific user.</span></span>|
|<span data-ttu-id="c0b72-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c0b72-136">errorDeviceCount</span></span>|<span data-ttu-id="c0b72-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b72-137">Int32</span></span>|<span data-ttu-id="c0b72-138">特定のユーザーのエラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="c0b72-138">Error device count for specific user.</span></span>|
|<span data-ttu-id="c0b72-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0b72-139">userPrincipalName</span></span>|<span data-ttu-id="c0b72-140">String</span><span class="sxs-lookup"><span data-stu-id="c0b72-140">String</span></span>|<span data-ttu-id="c0b72-141">特定のユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="c0b72-141">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0b72-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0b72-142">Relationships</span></span>
|<span data-ttu-id="c0b72-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0b72-143">Relationship</span></span>|<span data-ttu-id="c0b72-144">型</span><span class="sxs-lookup"><span data-stu-id="c0b72-144">Type</span></span>|<span data-ttu-id="c0b72-145">説明</span><span class="sxs-lookup"><span data-stu-id="c0b72-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b72-146">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="c0b72-146">deviceRunStates</span></span>|<span data-ttu-id="c0b72-147">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b72-147">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="c0b72-148">特定のユーザーのすべてのデバイスでこのスクリプトの実行状態を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c0b72-148">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0b72-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0b72-149">JSON Representation</span></span>
<span data-ttu-id="c0b72-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0b72-150">Here is a JSON representation of the resource.</span></span>
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





