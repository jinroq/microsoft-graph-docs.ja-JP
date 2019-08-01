---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b054e2472965f59d8350a52fe22134ab98e00fdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028435"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="148a7-103">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="148a7-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="148a7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="148a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148a7-105">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="148a7-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="148a7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="148a7-106">Methods</span></span>
|<span data-ttu-id="148a7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="148a7-107">Method</span></span>|<span data-ttu-id="148a7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="148a7-108">Return Type</span></span>|<span data-ttu-id="148a7-109">説明</span><span class="sxs-lookup"><span data-stu-id="148a7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="148a7-110">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="148a7-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="148a7-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="148a7-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="148a7-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="148a7-113">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="148a7-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="148a7-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="148a7-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="148a7-115">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="148a7-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="148a7-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="148a7-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="148a7-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="148a7-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="148a7-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="148a7-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="148a7-119">Properties</span></span>
|<span data-ttu-id="148a7-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="148a7-120">Property</span></span>|<span data-ttu-id="148a7-121">型</span><span class="sxs-lookup"><span data-stu-id="148a7-121">Type</span></span>|<span data-ttu-id="148a7-122">説明</span><span class="sxs-lookup"><span data-stu-id="148a7-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148a7-123">id</span><span class="sxs-lookup"><span data-stu-id="148a7-123">id</span></span>|<span data-ttu-id="148a7-124">文字列</span><span class="sxs-lookup"><span data-stu-id="148a7-124">String</span></span>|<span data-ttu-id="148a7-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="148a7-125">Key of the entity.</span></span>|
|<span data-ttu-id="148a7-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="148a7-126">lastModifiedDateTime</span></span>|<span data-ttu-id="148a7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148a7-127">DateTimeOffset</span></span>|<span data-ttu-id="148a7-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="148a7-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="148a7-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="148a7-129">createdDateTime</span></span>|<span data-ttu-id="148a7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148a7-130">DateTimeOffset</span></span>|<span data-ttu-id="148a7-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="148a7-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="148a7-132">description</span><span class="sxs-lookup"><span data-stu-id="148a7-132">description</span></span>|<span data-ttu-id="148a7-133">String</span><span class="sxs-lookup"><span data-stu-id="148a7-133">String</span></span>|<span data-ttu-id="148a7-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="148a7-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="148a7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="148a7-135">displayName</span></span>|<span data-ttu-id="148a7-136">String</span><span class="sxs-lookup"><span data-stu-id="148a7-136">String</span></span>|<span data-ttu-id="148a7-137">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="148a7-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="148a7-138">version</span><span class="sxs-lookup"><span data-stu-id="148a7-138">version</span></span>|<span data-ttu-id="148a7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="148a7-139">Int32</span></span>|<span data-ttu-id="148a7-140">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="148a7-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="148a7-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="148a7-141">Relationships</span></span>
|<span data-ttu-id="148a7-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="148a7-142">Relationship</span></span>|<span data-ttu-id="148a7-143">型</span><span class="sxs-lookup"><span data-stu-id="148a7-143">Type</span></span>|<span data-ttu-id="148a7-144">説明</span><span class="sxs-lookup"><span data-stu-id="148a7-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148a7-145">assignments</span><span class="sxs-lookup"><span data-stu-id="148a7-145">assignments</span></span>|<span data-ttu-id="148a7-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="148a7-147">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="148a7-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="148a7-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="148a7-148">deviceStatuses</span></span>|<span data-ttu-id="148a7-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="148a7-150">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="148a7-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="148a7-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="148a7-151">userStatuses</span></span>|<span data-ttu-id="148a7-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="148a7-153">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="148a7-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="148a7-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="148a7-154">deviceStatusOverview</span></span>|[<span data-ttu-id="148a7-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="148a7-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="148a7-156">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="148a7-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="148a7-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="148a7-157">userStatusOverview</span></span>|[<span data-ttu-id="148a7-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="148a7-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="148a7-159">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="148a7-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="148a7-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="148a7-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="148a7-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a7-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="148a7-162">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="148a7-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="148a7-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="148a7-163">JSON Representation</span></span>
<span data-ttu-id="148a7-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="148a7-164">Here is a JSON representation of the resource.</span></span>
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



