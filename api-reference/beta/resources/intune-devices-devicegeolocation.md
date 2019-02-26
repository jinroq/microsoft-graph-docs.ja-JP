---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eaa46929ae627dbf6cdee8d300b7910b4817ffc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149603"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="7d2d8-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d2d8-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="7d2d8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d2d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d2d8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d2d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d2d8-106">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="7d2d8-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="7d2d8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d2d8-107">Properties</span></span>
|<span data-ttu-id="7d2d8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d2d8-108">Property</span></span>|<span data-ttu-id="7d2d8-109">型</span><span class="sxs-lookup"><span data-stu-id="7d2d8-109">Type</span></span>|<span data-ttu-id="7d2d8-110">説明</span><span class="sxs-lookup"><span data-stu-id="7d2d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d2d8-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="7d2d8-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="7d2d8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d2d8-112">DateTimeOffset</span></span>|<span data-ttu-id="7d2d8-113">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="7d2d8-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="7d2d8-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d2d8-114">lastCollectedDateTime</span></span>|<span data-ttu-id="7d2d8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d2d8-115">DateTimeOffset</span></span>|<span data-ttu-id="7d2d8-116">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="7d2d8-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="7d2d8-117">longitude</span><span class="sxs-lookup"><span data-stu-id="7d2d8-117">longitude</span></span>|<span data-ttu-id="7d2d8-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-118">Double</span></span>|<span data-ttu-id="7d2d8-119">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="7d2d8-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="7d2d8-120">latitude</span><span class="sxs-lookup"><span data-stu-id="7d2d8-120">latitude</span></span>|<span data-ttu-id="7d2d8-121">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-121">Double</span></span>|<span data-ttu-id="7d2d8-122">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="7d2d8-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="7d2d8-123">altitude</span><span class="sxs-lookup"><span data-stu-id="7d2d8-123">altitude</span></span>|<span data-ttu-id="7d2d8-124">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-124">Double</span></span>|<span data-ttu-id="7d2d8-125">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="7d2d8-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="7d2d8-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="7d2d8-126">horizontalAccuracy</span></span>|<span data-ttu-id="7d2d8-127">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-127">Double</span></span>|<span data-ttu-id="7d2d8-128">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="7d2d8-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="7d2d8-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="7d2d8-129">verticalAccuracy</span></span>|<span data-ttu-id="7d2d8-130">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-130">Double</span></span>|<span data-ttu-id="7d2d8-131">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="7d2d8-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="7d2d8-132">heading</span><span class="sxs-lookup"><span data-stu-id="7d2d8-132">heading</span></span>|<span data-ttu-id="7d2d8-133">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="7d2d8-133">Double</span></span>|<span data-ttu-id="7d2d8-134">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="7d2d8-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="7d2d8-135">speed</span><span class="sxs-lookup"><span data-stu-id="7d2d8-135">speed</span></span>|<span data-ttu-id="7d2d8-136">Double</span><span class="sxs-lookup"><span data-stu-id="7d2d8-136">Double</span></span>|<span data-ttu-id="7d2d8-137">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="7d2d8-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d2d8-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d2d8-138">Relationships</span></span>
<span data-ttu-id="7d2d8-139">なし</span><span class="sxs-lookup"><span data-stu-id="7d2d8-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d2d8-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d2d8-140">JSON Representation</span></span>
<span data-ttu-id="7d2d8-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d2d8-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```




