---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e74342f8567c9b1fb8901b07a7a231ba196bfd44
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947058"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="13675-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13675-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="13675-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13675-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13675-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13675-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="13675-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="13675-107">Methods</span></span>
|<span data-ttu-id="13675-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="13675-108">Method</span></span>|<span data-ttu-id="13675-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="13675-109">Return Type</span></span>|<span data-ttu-id="13675-110">説明</span><span class="sxs-lookup"><span data-stu-id="13675-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13675-111">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="13675-111">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="13675-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="13675-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="13675-113">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="13675-113">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="13675-114">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="13675-114">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="13675-115">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="13675-115">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="13675-116">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="13675-116">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13675-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13675-117">Properties</span></span>
|<span data-ttu-id="13675-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13675-118">Property</span></span>|<span data-ttu-id="13675-119">型</span><span class="sxs-lookup"><span data-stu-id="13675-119">Type</span></span>|<span data-ttu-id="13675-120">説明</span><span class="sxs-lookup"><span data-stu-id="13675-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13675-121">id</span><span class="sxs-lookup"><span data-stu-id="13675-121">id</span></span>|<span data-ttu-id="13675-122">String</span><span class="sxs-lookup"><span data-stu-id="13675-122">String</span></span>|<span data-ttu-id="13675-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="13675-123">Key of the entity.</span></span>|
|<span data-ttu-id="13675-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="13675-124">pendingCount</span></span>|<span data-ttu-id="13675-125">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-125">Int32</span></span>|<span data-ttu-id="13675-126">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-126">Number of pending devices</span></span>|
|<span data-ttu-id="13675-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="13675-127">notApplicableCount</span></span>|<span data-ttu-id="13675-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-128">Int32</span></span>|<span data-ttu-id="13675-129">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="13675-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="13675-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="13675-131">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-131">Int32</span></span>|<span data-ttu-id="13675-132">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="13675-133">successCount</span><span class="sxs-lookup"><span data-stu-id="13675-133">successCount</span></span>|<span data-ttu-id="13675-134">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-134">Int32</span></span>|<span data-ttu-id="13675-135">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="13675-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="13675-136">errorCount</span></span>|<span data-ttu-id="13675-137">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-137">Int32</span></span>|<span data-ttu-id="13675-138">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-138">Number of error devices</span></span>|
|<span data-ttu-id="13675-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="13675-139">failedCount</span></span>|<span data-ttu-id="13675-140">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-140">Int32</span></span>|<span data-ttu-id="13675-141">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-141">Number of failed devices</span></span>|
|<span data-ttu-id="13675-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="13675-142">conflictCount</span></span>|<span data-ttu-id="13675-143">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-143">Int32</span></span>|<span data-ttu-id="13675-144">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="13675-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="13675-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="13675-145">lastUpdateDateTime</span></span>|<span data-ttu-id="13675-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13675-146">DateTimeOffset</span></span>|<span data-ttu-id="13675-147">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="13675-147">Last update time</span></span>|
|<span data-ttu-id="13675-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="13675-148">configurationVersion</span></span>|<span data-ttu-id="13675-149">Int32</span><span class="sxs-lookup"><span data-stu-id="13675-149">Int32</span></span>|<span data-ttu-id="13675-150">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="13675-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="13675-151">関係</span><span class="sxs-lookup"><span data-stu-id="13675-151">Relationships</span></span>
<span data-ttu-id="13675-152">なし</span><span class="sxs-lookup"><span data-stu-id="13675-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13675-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13675-153">JSON Representation</span></span>
<span data-ttu-id="13675-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13675-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```




