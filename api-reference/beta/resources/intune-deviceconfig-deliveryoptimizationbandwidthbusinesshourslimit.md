---
title: deliveryOptimizationBandwidthBusinessHoursLimit リソースの種類
description: 帯域幅の営業時間とパーセンテージの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f1a9f5e3074372605352e1ff6e1bc9a04b97174
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979712"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="03a4a-103">deliveryOptimizationBandwidthBusinessHoursLimit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03a4a-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="03a4a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03a4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03a4a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03a4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03a4a-106">帯域幅の営業時間とパーセンテージの種類</span><span class="sxs-lookup"><span data-stu-id="03a4a-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="03a4a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a4a-107">Properties</span></span>
|<span data-ttu-id="03a4a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a4a-108">Property</span></span>|<span data-ttu-id="03a4a-109">型</span><span class="sxs-lookup"><span data-stu-id="03a4a-109">Type</span></span>|<span data-ttu-id="03a4a-110">説明</span><span class="sxs-lookup"><span data-stu-id="03a4a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a4a-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="03a4a-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="03a4a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="03a4a-112">Int32</span></span>|<span data-ttu-id="03a4a-113">24時間形式 (0-23) を使用して営業時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="03a4a-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="03a4a-114">有効な値は0から23までです</span><span class="sxs-lookup"><span data-stu-id="03a4a-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="03a4a-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="03a4a-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="03a4a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="03a4a-116">Int32</span></span>|<span data-ttu-id="03a4a-117">24時間形式 (0-23) を使用して営業時間の終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="03a4a-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="03a4a-118">有効な値は0から23までです</span><span class="sxs-lookup"><span data-stu-id="03a4a-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="03a4a-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="03a4a-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="03a4a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="03a4a-120">Int32</span></span>|<span data-ttu-id="03a4a-121">営業時間内に制限する帯域幅の割合 (0-100) を指定します。</span><span class="sxs-lookup"><span data-stu-id="03a4a-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="03a4a-122">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="03a4a-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="03a4a-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="03a4a-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="03a4a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="03a4a-124">Int32</span></span>|<span data-ttu-id="03a4a-125">勤務時間を制限する帯域幅の割合 (0-100) を指定します。</span><span class="sxs-lookup"><span data-stu-id="03a4a-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="03a4a-126">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="03a4a-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="03a4a-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03a4a-127">Relationships</span></span>
<span data-ttu-id="03a4a-128">なし</span><span class="sxs-lookup"><span data-stu-id="03a4a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03a4a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03a4a-129">JSON Representation</span></span>
<span data-ttu-id="03a4a-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03a4a-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```





