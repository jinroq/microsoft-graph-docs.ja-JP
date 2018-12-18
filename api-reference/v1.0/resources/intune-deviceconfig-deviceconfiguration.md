---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
author: tfitzmac
ms.openlocfilehash: 5624b52c4c92f49b5ce5300cd3e1abc45afe2e9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311670"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="67bd5-103">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67bd5-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="67bd5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67bd5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67bd5-105">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="67bd5-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="67bd5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="67bd5-106">Methods</span></span>
|<span data-ttu-id="67bd5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="67bd5-107">Method</span></span>|<span data-ttu-id="67bd5-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67bd5-108">Return Type</span></span>|<span data-ttu-id="67bd5-109">説明</span><span class="sxs-lookup"><span data-stu-id="67bd5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67bd5-110">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="67bd5-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="67bd5-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="67bd5-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="67bd5-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="67bd5-113">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="67bd5-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="67bd5-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="67bd5-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="67bd5-115">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="67bd5-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="67bd5-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="67bd5-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="67bd5-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="67bd5-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bd5-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="67bd5-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67bd5-119">Properties</span></span>
|<span data-ttu-id="67bd5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67bd5-120">Property</span></span>|<span data-ttu-id="67bd5-121">種類</span><span class="sxs-lookup"><span data-stu-id="67bd5-121">Type</span></span>|<span data-ttu-id="67bd5-122">説明</span><span class="sxs-lookup"><span data-stu-id="67bd5-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bd5-123">ID</span><span class="sxs-lookup"><span data-stu-id="67bd5-123">id</span></span>|<span data-ttu-id="67bd5-124">String</span><span class="sxs-lookup"><span data-stu-id="67bd5-124">String</span></span>|<span data-ttu-id="67bd5-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67bd5-125">Key of the entity.</span></span>|
|<span data-ttu-id="67bd5-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67bd5-126">lastModifiedDateTime</span></span>|<span data-ttu-id="67bd5-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bd5-127">DateTimeOffset</span></span>|<span data-ttu-id="67bd5-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="67bd5-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="67bd5-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67bd5-129">createdDateTime</span></span>|<span data-ttu-id="67bd5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bd5-130">DateTimeOffset</span></span>|<span data-ttu-id="67bd5-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="67bd5-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="67bd5-132">説明</span><span class="sxs-lookup"><span data-stu-id="67bd5-132">description</span></span>|<span data-ttu-id="67bd5-133">String</span><span class="sxs-lookup"><span data-stu-id="67bd5-133">String</span></span>|<span data-ttu-id="67bd5-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="67bd5-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="67bd5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="67bd5-135">displayName</span></span>|<span data-ttu-id="67bd5-136">String</span><span class="sxs-lookup"><span data-stu-id="67bd5-136">String</span></span>|<span data-ttu-id="67bd5-137">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="67bd5-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="67bd5-138">version</span><span class="sxs-lookup"><span data-stu-id="67bd5-138">version</span></span>|<span data-ttu-id="67bd5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="67bd5-139">Int32</span></span>|<span data-ttu-id="67bd5-140">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="67bd5-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67bd5-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67bd5-141">Relationships</span></span>
|<span data-ttu-id="67bd5-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67bd5-142">Relationship</span></span>|<span data-ttu-id="67bd5-143">型</span><span class="sxs-lookup"><span data-stu-id="67bd5-143">Type</span></span>|<span data-ttu-id="67bd5-144">説明</span><span class="sxs-lookup"><span data-stu-id="67bd5-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bd5-145">assignments</span><span class="sxs-lookup"><span data-stu-id="67bd5-145">assignments</span></span>|<span data-ttu-id="67bd5-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="67bd5-147">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="67bd5-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="67bd5-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="67bd5-148">deviceStatuses</span></span>|<span data-ttu-id="67bd5-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="67bd5-150">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="67bd5-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="67bd5-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="67bd5-151">userStatuses</span></span>|<span data-ttu-id="67bd5-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="67bd5-153">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="67bd5-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="67bd5-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="67bd5-154">deviceStatusOverview</span></span>|[<span data-ttu-id="67bd5-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="67bd5-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="67bd5-156">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="67bd5-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="67bd5-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="67bd5-157">userStatusOverview</span></span>|[<span data-ttu-id="67bd5-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="67bd5-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="67bd5-159">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="67bd5-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="67bd5-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="67bd5-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="67bd5-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="67bd5-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="67bd5-162">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="67bd5-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67bd5-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67bd5-163">JSON Representation</span></span>
<span data-ttu-id="67bd5-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67bd5-164">Here is a JSON representation of the resource.</span></span>
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



