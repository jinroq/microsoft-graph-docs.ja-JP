---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 831fe9241b23758ee868053e59e93b427fbfc2dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950754"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="15051-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15051-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="15051-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15051-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15051-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15051-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15051-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15051-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15051-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15051-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="15051-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="15051-108">Methods</span></span>
|<span data-ttu-id="15051-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="15051-109">Method</span></span>|<span data-ttu-id="15051-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15051-110">Return Type</span></span>|<span data-ttu-id="15051-111">説明</span><span class="sxs-lookup"><span data-stu-id="15051-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15051-112">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15051-112">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="15051-113">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15051-113">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="15051-114">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="15051-114">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="15051-115">Update deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15051-115">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="15051-116">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="15051-116">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="15051-117">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15051-117">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15051-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15051-118">Properties</span></span>
|<span data-ttu-id="15051-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15051-119">Property</span></span>|<span data-ttu-id="15051-120">種類</span><span class="sxs-lookup"><span data-stu-id="15051-120">Type</span></span>|<span data-ttu-id="15051-121">説明</span><span class="sxs-lookup"><span data-stu-id="15051-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15051-122">ID</span><span class="sxs-lookup"><span data-stu-id="15051-122">id</span></span>|<span data-ttu-id="15051-123">String</span><span class="sxs-lookup"><span data-stu-id="15051-123">String</span></span>|<span data-ttu-id="15051-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="15051-124">Key of the entity.</span></span>|
|<span data-ttu-id="15051-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="15051-125">pendingCount</span></span>|<span data-ttu-id="15051-126">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-126">Int32</span></span>|<span data-ttu-id="15051-127">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-127">Number of pending devices</span></span>|
|<span data-ttu-id="15051-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="15051-128">notApplicableCount</span></span>|<span data-ttu-id="15051-129">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-129">Int32</span></span>|<span data-ttu-id="15051-130">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="15051-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="15051-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="15051-132">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-132">Int32</span></span>|<span data-ttu-id="15051-133">一致していないプラットフォームとポリシーが適用されないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="15051-134">successCount</span><span class="sxs-lookup"><span data-stu-id="15051-134">successCount</span></span>|<span data-ttu-id="15051-135">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-135">Int32</span></span>|<span data-ttu-id="15051-136">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="15051-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="15051-137">errorCount</span></span>|<span data-ttu-id="15051-138">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-138">Int32</span></span>|<span data-ttu-id="15051-139">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-139">Number of error devices</span></span>|
|<span data-ttu-id="15051-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="15051-140">failedCount</span></span>|<span data-ttu-id="15051-141">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-141">Int32</span></span>|<span data-ttu-id="15051-142">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-142">Number of failed devices</span></span>|
|<span data-ttu-id="15051-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="15051-143">conflictCount</span></span>|<span data-ttu-id="15051-144">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-144">Int32</span></span>|<span data-ttu-id="15051-145">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="15051-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="15051-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="15051-146">lastUpdateDateTime</span></span>|<span data-ttu-id="15051-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15051-147">DateTimeOffset</span></span>|<span data-ttu-id="15051-148">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="15051-148">Last update time</span></span>|
|<span data-ttu-id="15051-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="15051-149">configurationVersion</span></span>|<span data-ttu-id="15051-150">Int32</span><span class="sxs-lookup"><span data-stu-id="15051-150">Int32</span></span>|<span data-ttu-id="15051-151">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="15051-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="15051-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15051-152">Relationships</span></span>
<span data-ttu-id="15051-153">なし</span><span class="sxs-lookup"><span data-stu-id="15051-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15051-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15051-154">JSON Representation</span></span>
<span data-ttu-id="15051-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15051-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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





