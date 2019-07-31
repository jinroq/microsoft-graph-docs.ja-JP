---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1efe63f87057952444e17b9c5684cd3ecc20d4c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999802"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="c7f81-103">deviceProtectionOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7f81-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="c7f81-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7f81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7f81-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7f81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f81-106">特定のデバイスのハードウェア情報。</span><span class="sxs-lookup"><span data-stu-id="c7f81-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="c7f81-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7f81-107">Properties</span></span>
|<span data-ttu-id="c7f81-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7f81-108">Property</span></span>|<span data-ttu-id="c7f81-109">型</span><span class="sxs-lookup"><span data-stu-id="c7f81-109">Type</span></span>|<span data-ttu-id="c7f81-110">説明</span><span class="sxs-lookup"><span data-stu-id="c7f81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f81-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="c7f81-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-112">Int32</span></span>|<span data-ttu-id="c7f81-113">デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-113">Total device count.</span></span>|
|<span data-ttu-id="c7f81-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="c7f81-115">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-115">Int32</span></span>|<span data-ttu-id="c7f81-116">脅威エージェント数が非アクティブなデバイス</span><span class="sxs-lookup"><span data-stu-id="c7f81-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="c7f81-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="c7f81-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-118">Int32</span></span>|<span data-ttu-id="c7f81-119">不明な数の脅威エージェントの状態を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="c7f81-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="c7f81-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="c7f81-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-121">Int32</span></span>|<span data-ttu-id="c7f81-122">署名数が古いデバイス。</span><span class="sxs-lookup"><span data-stu-id="c7f81-122">Device with old signature count.</span></span>|
|<span data-ttu-id="c7f81-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-123">cleanDeviceCount</span></span>|<span data-ttu-id="c7f81-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-124">Int32</span></span>|<span data-ttu-id="c7f81-125">デバイス数をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="c7f81-125">Clean device count.</span></span>|
|<span data-ttu-id="c7f81-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="c7f81-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-127">Int32</span></span>|<span data-ttu-id="c7f81-128">保留中のフルスキャンデバイス数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="c7f81-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="c7f81-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-130">Int32</span></span>|<span data-ttu-id="c7f81-131">保留中の再起動デバイス数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-131">Pending restart device count.</span></span>|
|<span data-ttu-id="c7f81-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="c7f81-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-133">Int32</span></span>|<span data-ttu-id="c7f81-134">保留中の手動手順デバイス数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="c7f81-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="c7f81-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-136">Int32</span></span>|<span data-ttu-id="c7f81-137">保留中のオフラインスキャンデバイス数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="c7f81-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7f81-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="c7f81-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f81-139">Int32</span></span>|<span data-ttu-id="c7f81-140">重大なエラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="c7f81-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7f81-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7f81-141">Relationships</span></span>
<span data-ttu-id="c7f81-142">なし</span><span class="sxs-lookup"><span data-stu-id="c7f81-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7f81-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7f81-143">JSON Representation</span></span>
<span data-ttu-id="c7f81-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7f81-144">Here is a JSON representation of the resource.</span></span>
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





