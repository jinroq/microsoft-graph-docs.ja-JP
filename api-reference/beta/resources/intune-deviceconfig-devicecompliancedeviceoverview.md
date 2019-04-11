---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe7216986a4a64c242dd041cd4325f321d0c5956
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800372"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="c60f5-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c60f5-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="c60f5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c60f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c60f5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c60f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c60f5-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c60f5-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c60f5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c60f5-107">Methods</span></span>
|<span data-ttu-id="c60f5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c60f5-108">Method</span></span>|<span data-ttu-id="c60f5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c60f5-109">Return Type</span></span>|<span data-ttu-id="c60f5-110">説明</span><span class="sxs-lookup"><span data-stu-id="c60f5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c60f5-111">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c60f5-111">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="c60f5-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c60f5-112">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c60f5-113">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c60f5-113">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="c60f5-114">deviceComplianceDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="c60f5-114">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="c60f5-115">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c60f5-115">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c60f5-116">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c60f5-116">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c60f5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c60f5-117">Properties</span></span>
|<span data-ttu-id="c60f5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c60f5-118">Property</span></span>|<span data-ttu-id="c60f5-119">型</span><span class="sxs-lookup"><span data-stu-id="c60f5-119">Type</span></span>|<span data-ttu-id="c60f5-120">説明</span><span class="sxs-lookup"><span data-stu-id="c60f5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c60f5-121">id</span><span class="sxs-lookup"><span data-stu-id="c60f5-121">id</span></span>|<span data-ttu-id="c60f5-122">String</span><span class="sxs-lookup"><span data-stu-id="c60f5-122">String</span></span>|<span data-ttu-id="c60f5-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c60f5-123">Key of the entity.</span></span>|
|<span data-ttu-id="c60f5-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-124">pendingCount</span></span>|<span data-ttu-id="c60f5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-125">Int32</span></span>|<span data-ttu-id="c60f5-126">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-126">Number of pending devices</span></span>|
|<span data-ttu-id="c60f5-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-127">notApplicableCount</span></span>|<span data-ttu-id="c60f5-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-128">Int32</span></span>|<span data-ttu-id="c60f5-129">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="c60f5-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="c60f5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-131">Int32</span></span>|<span data-ttu-id="c60f5-132">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="c60f5-133">successCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-133">successCount</span></span>|<span data-ttu-id="c60f5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-134">Int32</span></span>|<span data-ttu-id="c60f5-135">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="c60f5-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-136">errorCount</span></span>|<span data-ttu-id="c60f5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-137">Int32</span></span>|<span data-ttu-id="c60f5-138">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-138">Number of error devices</span></span>|
|<span data-ttu-id="c60f5-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-139">failedCount</span></span>|<span data-ttu-id="c60f5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-140">Int32</span></span>|<span data-ttu-id="c60f5-141">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-141">Number of failed devices</span></span>|
|<span data-ttu-id="c60f5-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c60f5-142">conflictCount</span></span>|<span data-ttu-id="c60f5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-143">Int32</span></span>|<span data-ttu-id="c60f5-144">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c60f5-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="c60f5-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c60f5-145">lastUpdateDateTime</span></span>|<span data-ttu-id="c60f5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c60f5-146">DateTimeOffset</span></span>|<span data-ttu-id="c60f5-147">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="c60f5-147">Last update time</span></span>|
|<span data-ttu-id="c60f5-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c60f5-148">configurationVersion</span></span>|<span data-ttu-id="c60f5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c60f5-149">Int32</span></span>|<span data-ttu-id="c60f5-150">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="c60f5-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c60f5-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c60f5-151">Relationships</span></span>
<span data-ttu-id="c60f5-152">なし</span><span class="sxs-lookup"><span data-stu-id="c60f5-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c60f5-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c60f5-153">JSON Representation</span></span>
<span data-ttu-id="c60f5-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c60f5-154">Here is a JSON representation of the resource.</span></span>
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





