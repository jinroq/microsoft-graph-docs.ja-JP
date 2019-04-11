---
title: deliveryOptimizationBandwidthHoursWithPercentage リソースの種類
description: 営業時間に対する割合としての帯域幅制限。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecb024d15ee5d4e748d57e1b895c9418feadd52a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802738"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="bdd16-103">deliveryOptimizationBandwidthHoursWithPercentage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdd16-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="bdd16-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdd16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdd16-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdd16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdd16-106">営業時間に対する割合としての帯域幅制限。</span><span class="sxs-lookup"><span data-stu-id="bdd16-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="bdd16-107">[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bdd16-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bdd16-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdd16-108">Properties</span></span>
|<span data-ttu-id="bdd16-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdd16-109">Property</span></span>|<span data-ttu-id="bdd16-110">型</span><span class="sxs-lookup"><span data-stu-id="bdd16-110">Type</span></span>|<span data-ttu-id="bdd16-111">説明</span><span class="sxs-lookup"><span data-stu-id="bdd16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd16-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="bdd16-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="bdd16-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="bdd16-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="bdd16-114">バックグラウンドダウンロードの割合 (時間)。</span><span class="sxs-lookup"><span data-stu-id="bdd16-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="bdd16-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="bdd16-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="bdd16-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="bdd16-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="bdd16-117">フォアグラウンドダウンロードの割合 (時間)。</span><span class="sxs-lookup"><span data-stu-id="bdd16-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdd16-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bdd16-118">Relationships</span></span>
<span data-ttu-id="bdd16-119">なし</span><span class="sxs-lookup"><span data-stu-id="bdd16-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdd16-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdd16-120">JSON Representation</span></span>
<span data-ttu-id="bdd16-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bdd16-121">Here is a JSON representation of the resource.</span></span>
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





