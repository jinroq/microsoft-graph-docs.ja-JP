---
title: deliveryOptimizationBandwidthAbsolute リソースの種類
description: 帯域幅制限 (キロバイト/秒)。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178270"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="0475c-103">deliveryOptimizationBandwidthAbsolute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0475c-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="0475c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0475c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0475c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0475c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0475c-106">帯域幅制限 (キロバイト/秒)。</span><span class="sxs-lookup"><span data-stu-id="0475c-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="0475c-107">[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0475c-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0475c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0475c-108">Properties</span></span>
|<span data-ttu-id="0475c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0475c-109">Property</span></span>|<span data-ttu-id="0475c-110">型</span><span class="sxs-lookup"><span data-stu-id="0475c-110">Type</span></span>|<span data-ttu-id="0475c-111">説明</span><span class="sxs-lookup"><span data-stu-id="0475c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0475c-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="0475c-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="0475c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0475c-113">Int64</span></span>|<span data-ttu-id="0475c-114">配信の最適化を使用して、すべての同時ダウンロードアクティビティでデバイスが使用できる最大ダウンロード帯域幅をキロバイト/秒で指定します。</span><span class="sxs-lookup"><span data-stu-id="0475c-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="0475c-115">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="0475c-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="0475c-116">値 0 (ゼロ) は、配信の最適化が、ダウンロードに使用可能な帯域幅を使用するように動的に調整されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="0475c-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="0475c-117">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="0475c-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="0475c-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="0475c-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="0475c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0475c-119">Int64</span></span>|<span data-ttu-id="0475c-120">配信の最適化 (0-4000000) を使用して、デバイスがすべての同時アップロードアクティビティで使用する最大アップロード帯域幅 (キロバイト/秒) を指定します。</span><span class="sxs-lookup"><span data-stu-id="0475c-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="0475c-121">有効な値は 0 ~ 400万</span><span class="sxs-lookup"><span data-stu-id="0475c-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="0475c-122">既定値は0で、無制限に可能な帯域幅を許可します (アップロード帯域幅の使用を最小限にするために最適化されています)。</span><span class="sxs-lookup"><span data-stu-id="0475c-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="0475c-123">有効な値は 0 ~ 400万</span><span class="sxs-lookup"><span data-stu-id="0475c-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="0475c-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0475c-124">Relationships</span></span>
<span data-ttu-id="0475c-125">なし</span><span class="sxs-lookup"><span data-stu-id="0475c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0475c-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0475c-126">JSON Representation</span></span>
<span data-ttu-id="0475c-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0475c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```




