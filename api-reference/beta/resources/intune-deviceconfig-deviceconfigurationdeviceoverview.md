---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 754fc4ffe7fd92ae2630b9c4a6a2686cdb9f3e0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973217"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="40ace-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40ace-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="40ace-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40ace-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40ace-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40ace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40ace-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40ace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40ace-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="40ace-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="40ace-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="40ace-108">Methods</span></span>
|<span data-ttu-id="40ace-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="40ace-109">Method</span></span>|<span data-ttu-id="40ace-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="40ace-110">Return Type</span></span>|<span data-ttu-id="40ace-111">説明</span><span class="sxs-lookup"><span data-stu-id="40ace-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="40ace-112">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="40ace-112">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="40ace-113">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="40ace-113">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="40ace-114">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="40ace-114">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="40ace-115">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="40ace-115">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="40ace-116">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="40ace-116">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="40ace-117">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40ace-117">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="40ace-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40ace-118">Properties</span></span>
|<span data-ttu-id="40ace-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40ace-119">Property</span></span>|<span data-ttu-id="40ace-120">型</span><span class="sxs-lookup"><span data-stu-id="40ace-120">Type</span></span>|<span data-ttu-id="40ace-121">説明</span><span class="sxs-lookup"><span data-stu-id="40ace-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40ace-122">ID</span><span class="sxs-lookup"><span data-stu-id="40ace-122">id</span></span>|<span data-ttu-id="40ace-123">String</span><span class="sxs-lookup"><span data-stu-id="40ace-123">String</span></span>|<span data-ttu-id="40ace-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40ace-124">Key of the entity.</span></span>|
|<span data-ttu-id="40ace-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="40ace-125">pendingCount</span></span>|<span data-ttu-id="40ace-126">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-126">Int32</span></span>|<span data-ttu-id="40ace-127">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-127">Number of pending devices</span></span>|
|<span data-ttu-id="40ace-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="40ace-128">notApplicableCount</span></span>|<span data-ttu-id="40ace-129">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-129">Int32</span></span>|<span data-ttu-id="40ace-130">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="40ace-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="40ace-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="40ace-132">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-132">Int32</span></span>|<span data-ttu-id="40ace-133">一致していないプラットフォームとポリシーが適用されないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="40ace-134">successCount</span><span class="sxs-lookup"><span data-stu-id="40ace-134">successCount</span></span>|<span data-ttu-id="40ace-135">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-135">Int32</span></span>|<span data-ttu-id="40ace-136">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="40ace-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="40ace-137">errorCount</span></span>|<span data-ttu-id="40ace-138">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-138">Int32</span></span>|<span data-ttu-id="40ace-139">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-139">Number of error devices</span></span>|
|<span data-ttu-id="40ace-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="40ace-140">failedCount</span></span>|<span data-ttu-id="40ace-141">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-141">Int32</span></span>|<span data-ttu-id="40ace-142">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-142">Number of failed devices</span></span>|
|<span data-ttu-id="40ace-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="40ace-143">conflictCount</span></span>|<span data-ttu-id="40ace-144">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-144">Int32</span></span>|<span data-ttu-id="40ace-145">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="40ace-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="40ace-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="40ace-146">lastUpdateDateTime</span></span>|<span data-ttu-id="40ace-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40ace-147">DateTimeOffset</span></span>|<span data-ttu-id="40ace-148">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="40ace-148">Last update time</span></span>|
|<span data-ttu-id="40ace-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="40ace-149">configurationVersion</span></span>|<span data-ttu-id="40ace-150">Int32</span><span class="sxs-lookup"><span data-stu-id="40ace-150">Int32</span></span>|<span data-ttu-id="40ace-151">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="40ace-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="40ace-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40ace-152">Relationships</span></span>
<span data-ttu-id="40ace-153">なし</span><span class="sxs-lookup"><span data-stu-id="40ace-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40ace-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40ace-154">JSON Representation</span></span>
<span data-ttu-id="40ace-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40ace-155">Here is a JSON representation of the resource.</span></span>
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





