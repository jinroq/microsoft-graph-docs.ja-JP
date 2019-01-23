---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b581b94e7933e39c012d47c499b0119b61fd41ce
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395763"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="47a75-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47a75-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="47a75-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47a75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47a75-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47a75-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47a75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47a75-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="47a75-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="47a75-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="47a75-108">Methods</span></span>
|<span data-ttu-id="47a75-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="47a75-109">Method</span></span>|<span data-ttu-id="47a75-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="47a75-110">Return Type</span></span>|<span data-ttu-id="47a75-111">説明</span><span class="sxs-lookup"><span data-stu-id="47a75-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47a75-112">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47a75-112">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="47a75-113">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47a75-113">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="47a75-114">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="47a75-114">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="47a75-115">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47a75-115">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="47a75-116">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47a75-116">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="47a75-117">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47a75-117">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47a75-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47a75-118">Properties</span></span>
|<span data-ttu-id="47a75-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47a75-119">Property</span></span>|<span data-ttu-id="47a75-120">型</span><span class="sxs-lookup"><span data-stu-id="47a75-120">Type</span></span>|<span data-ttu-id="47a75-121">説明</span><span class="sxs-lookup"><span data-stu-id="47a75-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a75-122">id</span><span class="sxs-lookup"><span data-stu-id="47a75-122">id</span></span>|<span data-ttu-id="47a75-123">String</span><span class="sxs-lookup"><span data-stu-id="47a75-123">String</span></span>|<span data-ttu-id="47a75-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47a75-124">Key of the entity.</span></span>|
|<span data-ttu-id="47a75-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="47a75-125">pendingCount</span></span>|<span data-ttu-id="47a75-126">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-126">Int32</span></span>|<span data-ttu-id="47a75-127">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-127">Number of pending devices</span></span>|
|<span data-ttu-id="47a75-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="47a75-128">notApplicableCount</span></span>|<span data-ttu-id="47a75-129">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-129">Int32</span></span>|<span data-ttu-id="47a75-130">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="47a75-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="47a75-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="47a75-132">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-132">Int32</span></span>|<span data-ttu-id="47a75-133">一致していないプラットフォームとポリシーが適用されないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="47a75-134">successCount</span><span class="sxs-lookup"><span data-stu-id="47a75-134">successCount</span></span>|<span data-ttu-id="47a75-135">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-135">Int32</span></span>|<span data-ttu-id="47a75-136">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="47a75-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="47a75-137">errorCount</span></span>|<span data-ttu-id="47a75-138">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-138">Int32</span></span>|<span data-ttu-id="47a75-139">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-139">Number of error devices</span></span>|
|<span data-ttu-id="47a75-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="47a75-140">failedCount</span></span>|<span data-ttu-id="47a75-141">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-141">Int32</span></span>|<span data-ttu-id="47a75-142">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-142">Number of failed devices</span></span>|
|<span data-ttu-id="47a75-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="47a75-143">conflictCount</span></span>|<span data-ttu-id="47a75-144">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-144">Int32</span></span>|<span data-ttu-id="47a75-145">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="47a75-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="47a75-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="47a75-146">lastUpdateDateTime</span></span>|<span data-ttu-id="47a75-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47a75-147">DateTimeOffset</span></span>|<span data-ttu-id="47a75-148">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="47a75-148">Last update time</span></span>|
|<span data-ttu-id="47a75-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="47a75-149">configurationVersion</span></span>|<span data-ttu-id="47a75-150">Int32</span><span class="sxs-lookup"><span data-stu-id="47a75-150">Int32</span></span>|<span data-ttu-id="47a75-151">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="47a75-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a75-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47a75-152">Relationships</span></span>
<span data-ttu-id="47a75-153">なし</span><span class="sxs-lookup"><span data-stu-id="47a75-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47a75-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47a75-154">JSON Representation</span></span>
<span data-ttu-id="47a75-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47a75-155">Here is a JSON representation of the resource.</span></span>
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




