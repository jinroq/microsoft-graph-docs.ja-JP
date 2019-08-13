---
title: deliveryOptimizationBandwidthPercentage リソースの種類
description: 割合として指定された帯域幅制限。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 782ed9a68ee3e759e719b14c2241cc1a02e30138
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333353"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="8d4fc-103">deliveryOptimizationBandwidthPercentage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d4fc-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="8d4fc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d4fc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d4fc-106">割合として指定された帯域幅制限。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="8d4fc-107">[DeliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d4fc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d4fc-108">Properties</span></span>
|<span data-ttu-id="8d4fc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d4fc-109">Property</span></span>|<span data-ttu-id="8d4fc-110">型</span><span class="sxs-lookup"><span data-stu-id="8d4fc-110">Type</span></span>|<span data-ttu-id="8d4fc-111">説明</span><span class="sxs-lookup"><span data-stu-id="8d4fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d4fc-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="8d4fc-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="8d4fc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8d4fc-113">Int32</span></span>|<span data-ttu-id="8d4fc-114">利用可能なダウンロード帯域幅 (0-100) の割合として、配信の最適化で使用される最大バックグラウンドダウンロード帯域幅を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="8d4fc-115">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d4fc-115">Valid values 0 to 100</span></span>
<span data-ttu-id="8d4fc-116">既定値の 0 (ゼロ) は、配信の最適化が、バックグラウンドダウンロードに使用可能な帯域幅を使用するように動的に調整されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="8d4fc-117">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d4fc-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8d4fc-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="8d4fc-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="8d4fc-119">Int32</span><span class="sxs-lookup"><span data-stu-id="8d4fc-119">Int32</span></span>|<span data-ttu-id="8d4fc-120">利用可能なダウンロード帯域幅 (0-100) の割合として、すべての同時ダウンロードアクティビティにおいて配信の最適化で使用されるフォアグラウンドの最大ダウンロード帯域幅を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="8d4fc-121">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d4fc-121">Valid values 0 to 100</span></span>
<span data-ttu-id="8d4fc-122">既定値の 0 (ゼロ) は、配信の最適化が、フォアグラウンドダウンロードに使用可能な帯域幅を使用するように動的に調整されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="8d4fc-123">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d4fc-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d4fc-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d4fc-124">Relationships</span></span>
<span data-ttu-id="8d4fc-125">なし</span><span class="sxs-lookup"><span data-stu-id="8d4fc-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d4fc-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d4fc-126">JSON Representation</span></span>
<span data-ttu-id="8d4fc-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d4fc-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



