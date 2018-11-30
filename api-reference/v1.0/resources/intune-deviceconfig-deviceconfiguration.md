---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
ms.openlocfilehash: 7cde579aa9d2e096380286d628a9964d4522f402
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024330"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="aa59e-103">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa59e-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="aa59e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa59e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa59e-105">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="aa59e-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="aa59e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa59e-106">Methods</span></span>
|<span data-ttu-id="aa59e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa59e-107">Method</span></span>|<span data-ttu-id="aa59e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aa59e-108">Return Type</span></span>|<span data-ttu-id="aa59e-109">説明</span><span class="sxs-lookup"><span data-stu-id="aa59e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa59e-110">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="aa59e-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="aa59e-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="aa59e-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aa59e-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="aa59e-113">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="aa59e-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="aa59e-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa59e-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="aa59e-115">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aa59e-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="aa59e-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="aa59e-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="aa59e-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aa59e-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aa59e-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aa59e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa59e-119">Properties</span></span>
|<span data-ttu-id="aa59e-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa59e-120">Property</span></span>|<span data-ttu-id="aa59e-121">型</span><span class="sxs-lookup"><span data-stu-id="aa59e-121">Type</span></span>|<span data-ttu-id="aa59e-122">説明</span><span class="sxs-lookup"><span data-stu-id="aa59e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa59e-123">id</span><span class="sxs-lookup"><span data-stu-id="aa59e-123">id</span></span>|<span data-ttu-id="aa59e-124">String</span><span class="sxs-lookup"><span data-stu-id="aa59e-124">String</span></span>|<span data-ttu-id="aa59e-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aa59e-125">Key of the entity.</span></span>|
|<span data-ttu-id="aa59e-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa59e-126">lastModifiedDateTime</span></span>|<span data-ttu-id="aa59e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa59e-127">DateTimeOffset</span></span>|<span data-ttu-id="aa59e-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="aa59e-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="aa59e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa59e-129">createdDateTime</span></span>|<span data-ttu-id="aa59e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa59e-130">DateTimeOffset</span></span>|<span data-ttu-id="aa59e-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aa59e-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="aa59e-132">説明</span><span class="sxs-lookup"><span data-stu-id="aa59e-132">description</span></span>|<span data-ttu-id="aa59e-133">String</span><span class="sxs-lookup"><span data-stu-id="aa59e-133">String</span></span>|<span data-ttu-id="aa59e-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="aa59e-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="aa59e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aa59e-135">displayName</span></span>|<span data-ttu-id="aa59e-136">String</span><span class="sxs-lookup"><span data-stu-id="aa59e-136">String</span></span>|<span data-ttu-id="aa59e-137">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="aa59e-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="aa59e-138">version</span><span class="sxs-lookup"><span data-stu-id="aa59e-138">version</span></span>|<span data-ttu-id="aa59e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aa59e-139">Int32</span></span>|<span data-ttu-id="aa59e-140">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="aa59e-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa59e-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa59e-141">Relationships</span></span>
|<span data-ttu-id="aa59e-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa59e-142">Relationship</span></span>|<span data-ttu-id="aa59e-143">型</span><span class="sxs-lookup"><span data-stu-id="aa59e-143">Type</span></span>|<span data-ttu-id="aa59e-144">説明</span><span class="sxs-lookup"><span data-stu-id="aa59e-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa59e-145">assignments</span><span class="sxs-lookup"><span data-stu-id="aa59e-145">assignments</span></span>|<span data-ttu-id="aa59e-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aa59e-147">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="aa59e-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="aa59e-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="aa59e-148">deviceStatuses</span></span>|<span data-ttu-id="aa59e-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="aa59e-150">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="aa59e-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="aa59e-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="aa59e-151">userStatuses</span></span>|<span data-ttu-id="aa59e-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="aa59e-153">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="aa59e-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="aa59e-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aa59e-154">deviceStatusOverview</span></span>|[<span data-ttu-id="aa59e-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aa59e-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="aa59e-156">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="aa59e-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="aa59e-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aa59e-157">userStatusOverview</span></span>|[<span data-ttu-id="aa59e-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="aa59e-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="aa59e-159">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="aa59e-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="aa59e-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="aa59e-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="aa59e-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa59e-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="aa59e-162">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="aa59e-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa59e-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa59e-163">JSON Representation</span></span>
<span data-ttu-id="aa59e-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa59e-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



