---
title: deliveryOptimizationBandwidthHoursWithPercentage リソースの種類
description: 営業時間に対する割合としての帯域幅制限。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecb024d15ee5d4e748d57e1b895c9418feadd52a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562728"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="51cbb-103">deliveryOptimizationBandwidthHoursWithPercentage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51cbb-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="51cbb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51cbb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51cbb-106">営業時間に対する割合としての帯域幅制限。</span><span class="sxs-lookup"><span data-stu-id="51cbb-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="51cbb-107">[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="51cbb-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51cbb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51cbb-108">Properties</span></span>
|<span data-ttu-id="51cbb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51cbb-109">Property</span></span>|<span data-ttu-id="51cbb-110">型</span><span class="sxs-lookup"><span data-stu-id="51cbb-110">Type</span></span>|<span data-ttu-id="51cbb-111">説明</span><span class="sxs-lookup"><span data-stu-id="51cbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51cbb-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="51cbb-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="51cbb-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="51cbb-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="51cbb-114">バックグラウンドダウンロードの割合 (時間)。</span><span class="sxs-lookup"><span data-stu-id="51cbb-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="51cbb-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="51cbb-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="51cbb-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="51cbb-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="51cbb-117">フォアグラウンドダウンロードの割合 (時間)。</span><span class="sxs-lookup"><span data-stu-id="51cbb-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51cbb-118">関係</span><span class="sxs-lookup"><span data-stu-id="51cbb-118">Relationships</span></span>
<span data-ttu-id="51cbb-119">なし</span><span class="sxs-lookup"><span data-stu-id="51cbb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51cbb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51cbb-120">JSON Representation</span></span>
<span data-ttu-id="51cbb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51cbb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```





