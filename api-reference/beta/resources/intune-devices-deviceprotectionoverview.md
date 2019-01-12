---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7b7c28474692c1b1df3b1d6a703e3dd43d05a15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944321"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="e99a0-103">deviceProtectionOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e99a0-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="e99a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e99a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e99a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e99a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e99a0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e99a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e99a0-107">特定のデバイスのハードウェア情報です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e99a0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e99a0-108">Properties</span></span>
|<span data-ttu-id="e99a0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e99a0-109">Property</span></span>|<span data-ttu-id="e99a0-110">型</span><span class="sxs-lookup"><span data-stu-id="e99a0-110">Type</span></span>|<span data-ttu-id="e99a0-111">説明</span><span class="sxs-lookup"><span data-stu-id="e99a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e99a0-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="e99a0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-113">Int32</span></span>|<span data-ttu-id="e99a0-114">デバイスの合計数です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-114">Total device count.</span></span>|
|<span data-ttu-id="e99a0-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="e99a0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-116">Int32</span></span>|<span data-ttu-id="e99a0-117">使用頻度の低い脅威エージェントの数とデバイス</span><span class="sxs-lookup"><span data-stu-id="e99a0-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="e99a0-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="e99a0-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-119">Int32</span></span>|<span data-ttu-id="e99a0-120">不明な数として脅威エージェントの状態を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="e99a0-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="e99a0-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="e99a0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-122">Int32</span></span>|<span data-ttu-id="e99a0-123">古い署名の数を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="e99a0-123">Device with old signature count.</span></span>|
|<span data-ttu-id="e99a0-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-124">cleanDeviceCount</span></span>|<span data-ttu-id="e99a0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-125">Int32</span></span>|<span data-ttu-id="e99a0-126">デバイス数をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="e99a0-126">Clean device count.</span></span>|
|<span data-ttu-id="e99a0-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="e99a0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-128">Int32</span></span>|<span data-ttu-id="e99a0-129">全体を走査する保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e99a0-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="e99a0-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="e99a0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-131">Int32</span></span>|<span data-ttu-id="e99a0-132">再起動の保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e99a0-132">Pending restart device count.</span></span>|
|<span data-ttu-id="e99a0-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="e99a0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-134">Int32</span></span>|<span data-ttu-id="e99a0-135">手作業で保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e99a0-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="e99a0-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="e99a0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-137">Int32</span></span>|<span data-ttu-id="e99a0-138">オフライン保留中のデバイス数をスキャンします。</span><span class="sxs-lookup"><span data-stu-id="e99a0-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="e99a0-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e99a0-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="e99a0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e99a0-140">Int32</span></span>|<span data-ttu-id="e99a0-141">障害の重要なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e99a0-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e99a0-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e99a0-142">Relationships</span></span>
<span data-ttu-id="e99a0-143">なし</span><span class="sxs-lookup"><span data-stu-id="e99a0-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e99a0-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e99a0-144">JSON Representation</span></span>
<span data-ttu-id="e99a0-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-145">Here is a JSON representation of the resource.</span></span>
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





