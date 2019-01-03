---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報です。
author: tfitzmac
ms.openlocfilehash: e705324bfc611117657ec629f8770e76c69be28d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317053"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="54f26-103">deviceProtectionOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54f26-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="54f26-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54f26-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54f26-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54f26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54f26-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="54f26-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54f26-107">特定のデバイスのハードウェア情報です。</span><span class="sxs-lookup"><span data-stu-id="54f26-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="54f26-108">Properties</span><span class="sxs-lookup"><span data-stu-id="54f26-108">Properties</span></span>
|<span data-ttu-id="54f26-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54f26-109">Property</span></span>|<span data-ttu-id="54f26-110">種類</span><span class="sxs-lookup"><span data-stu-id="54f26-110">Type</span></span>|<span data-ttu-id="54f26-111">説明</span><span class="sxs-lookup"><span data-stu-id="54f26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54f26-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="54f26-113">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-113">Int32</span></span>|<span data-ttu-id="54f26-114">デバイスの合計数です。</span><span class="sxs-lookup"><span data-stu-id="54f26-114">Total device count.</span></span>|
|<span data-ttu-id="54f26-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="54f26-116">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-116">Int32</span></span>|<span data-ttu-id="54f26-117">使用頻度の低い脅威エージェントの数とデバイス</span><span class="sxs-lookup"><span data-stu-id="54f26-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="54f26-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="54f26-119">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-119">Int32</span></span>|<span data-ttu-id="54f26-120">不明な数として脅威エージェントの状態を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="54f26-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="54f26-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="54f26-122">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-122">Int32</span></span>|<span data-ttu-id="54f26-123">古い署名の数を持つデバイス。</span><span class="sxs-lookup"><span data-stu-id="54f26-123">Device with old signature count.</span></span>|
|<span data-ttu-id="54f26-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-124">cleanDeviceCount</span></span>|<span data-ttu-id="54f26-125">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-125">Int32</span></span>|<span data-ttu-id="54f26-126">デバイス数をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="54f26-126">Clean device count.</span></span>|
|<span data-ttu-id="54f26-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="54f26-128">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-128">Int32</span></span>|<span data-ttu-id="54f26-129">全体を走査する保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="54f26-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="54f26-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="54f26-131">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-131">Int32</span></span>|<span data-ttu-id="54f26-132">再起動の保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="54f26-132">Pending restart device count.</span></span>|
|<span data-ttu-id="54f26-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="54f26-134">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-134">Int32</span></span>|<span data-ttu-id="54f26-135">手作業で保留中のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="54f26-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="54f26-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="54f26-137">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-137">Int32</span></span>|<span data-ttu-id="54f26-138">オフライン保留中のデバイス数をスキャンします。</span><span class="sxs-lookup"><span data-stu-id="54f26-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="54f26-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54f26-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="54f26-140">Int32</span><span class="sxs-lookup"><span data-stu-id="54f26-140">Int32</span></span>|<span data-ttu-id="54f26-141">障害の重要なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="54f26-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54f26-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54f26-142">Relationships</span></span>
<span data-ttu-id="54f26-143">なし</span><span class="sxs-lookup"><span data-stu-id="54f26-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54f26-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54f26-144">JSON Representation</span></span>
<span data-ttu-id="54f26-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54f26-145">Here is a JSON representation of the resource.</span></span>
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




