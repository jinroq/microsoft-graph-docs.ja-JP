---
title: deliveryOptimizationBandwidthAbsolute リソースの種類
description: 帯域幅制限 (キロバイト/秒)。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14e277258f4e8bbad75c3457b6c3da6dd604ff01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970822"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="57947-103">deliveryOptimizationBandwidthAbsolute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57947-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="57947-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57947-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57947-106">帯域幅制限 (キロバイト/秒)。</span><span class="sxs-lookup"><span data-stu-id="57947-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="57947-107">[DeliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57947-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57947-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57947-108">Properties</span></span>
|<span data-ttu-id="57947-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57947-109">Property</span></span>|<span data-ttu-id="57947-110">型</span><span class="sxs-lookup"><span data-stu-id="57947-110">Type</span></span>|<span data-ttu-id="57947-111">説明</span><span class="sxs-lookup"><span data-stu-id="57947-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57947-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="57947-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="57947-113">Int64</span><span class="sxs-lookup"><span data-stu-id="57947-113">Int64</span></span>|<span data-ttu-id="57947-114">配信の最適化を使用して、すべての同時ダウンロードアクティビティでデバイスが使用できる最大ダウンロード帯域幅をキロバイト/秒で指定します。</span><span class="sxs-lookup"><span data-stu-id="57947-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="57947-115">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="57947-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="57947-116">値 0 (ゼロ) は、配信の最適化が、ダウンロードに使用可能な帯域幅を使用するように動的に調整されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="57947-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="57947-117">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="57947-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="57947-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="57947-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="57947-119">Int64</span><span class="sxs-lookup"><span data-stu-id="57947-119">Int64</span></span>|<span data-ttu-id="57947-120">配信の最適化 (0-4000000) を使用して、デバイスがすべての同時アップロードアクティビティで使用する最大アップロード帯域幅 (キロバイト/秒) を指定します。</span><span class="sxs-lookup"><span data-stu-id="57947-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="57947-121">有効な値は 0 ~ 400万</span><span class="sxs-lookup"><span data-stu-id="57947-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="57947-122">既定値は0で、無制限に可能な帯域幅を許可します (アップロード帯域幅の使用を最小限にするために最適化されています)。</span><span class="sxs-lookup"><span data-stu-id="57947-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="57947-123">有効な値は 0 ~ 400万</span><span class="sxs-lookup"><span data-stu-id="57947-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="57947-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="57947-124">Relationships</span></span>
<span data-ttu-id="57947-125">なし</span><span class="sxs-lookup"><span data-stu-id="57947-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57947-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57947-126">JSON Representation</span></span>
<span data-ttu-id="57947-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57947-127">Here is a JSON representation of the resource.</span></span>
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





