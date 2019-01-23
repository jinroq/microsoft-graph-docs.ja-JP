---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418989"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="b507d-103">deviceProtectionOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b507d-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="b507d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b507d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b507d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b507d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b507d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b507d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b507d-107">特定のデバイスのハードウェア情報です。</span><span class="sxs-lookup"><span data-stu-id="b507d-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b507d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b507d-108">Properties</span></span>
|<span data-ttu-id="b507d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b507d-109">Property</span></span>|<span data-ttu-id="b507d-110">型</span><span class="sxs-lookup"><span data-stu-id="b507d-110">Type</span></span>|<span data-ttu-id="b507d-111">説明</span><span class="sxs-lookup"><span data-stu-id="b507d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b507d-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="b507d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-113">Int32</span></span>|<span data-ttu-id="b507d-114">デバイスの合計数です。</span><span class="sxs-lookup"><span data-stu-id="b507d-114">Total device count.</span></span>|
|<span data-ttu-id="b507d-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="b507d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-116">Int32</span></span>|<span data-ttu-id="b507d-117">使用頻度の低い脅威エージェントの数とデバイス</span><span class="sxs-lookup"><span data-stu-id="b507d-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="b507d-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="b507d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-119">Int32</span></span>|<span data-ttu-id="b507d-120">不明な数として脅威エージェントの状態を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="b507d-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="b507d-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="b507d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-122">Int32</span></span>|<span data-ttu-id="b507d-123">古い署名の数を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="b507d-123">Device with old signature count.</span></span>|
|<span data-ttu-id="b507d-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-124">cleanDeviceCount</span></span>|<span data-ttu-id="b507d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-125">Int32</span></span>|<span data-ttu-id="b507d-126">デバイス数をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="b507d-126">Clean device count.</span></span>|
|<span data-ttu-id="b507d-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="b507d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-128">Int32</span></span>|<span data-ttu-id="b507d-129">全体を走査する保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b507d-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="b507d-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="b507d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-131">Int32</span></span>|<span data-ttu-id="b507d-132">再起動の保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b507d-132">Pending restart device count.</span></span>|
|<span data-ttu-id="b507d-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="b507d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-134">Int32</span></span>|<span data-ttu-id="b507d-135">手作業で保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b507d-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="b507d-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="b507d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-137">Int32</span></span>|<span data-ttu-id="b507d-138">オフライン保留中のデバイス数をスキャンします。</span><span class="sxs-lookup"><span data-stu-id="b507d-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="b507d-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b507d-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="b507d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b507d-140">Int32</span></span>|<span data-ttu-id="b507d-141">障害の重要なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b507d-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b507d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b507d-142">Relationships</span></span>
<span data-ttu-id="b507d-143">なし</span><span class="sxs-lookup"><span data-stu-id="b507d-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b507d-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b507d-144">JSON Representation</span></span>
<span data-ttu-id="b507d-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b507d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




