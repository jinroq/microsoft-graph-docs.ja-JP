---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395056"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="95535-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95535-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="95535-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95535-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95535-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95535-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95535-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95535-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95535-107">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="95535-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="95535-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95535-108">Properties</span></span>
|<span data-ttu-id="95535-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95535-109">Property</span></span>|<span data-ttu-id="95535-110">型</span><span class="sxs-lookup"><span data-stu-id="95535-110">Type</span></span>|<span data-ttu-id="95535-111">説明</span><span class="sxs-lookup"><span data-stu-id="95535-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95535-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="95535-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="95535-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95535-113">DateTimeOffset</span></span>|<span data-ttu-id="95535-114">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="95535-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="95535-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="95535-115">lastCollectedDateTime</span></span>|<span data-ttu-id="95535-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95535-116">DateTimeOffset</span></span>|<span data-ttu-id="95535-117">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="95535-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="95535-118">longitude</span><span class="sxs-lookup"><span data-stu-id="95535-118">longitude</span></span>|<span data-ttu-id="95535-119">Double</span><span class="sxs-lookup"><span data-stu-id="95535-119">Double</span></span>|<span data-ttu-id="95535-120">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="95535-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="95535-121">latitude</span><span class="sxs-lookup"><span data-stu-id="95535-121">latitude</span></span>|<span data-ttu-id="95535-122">Double</span><span class="sxs-lookup"><span data-stu-id="95535-122">Double</span></span>|<span data-ttu-id="95535-123">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="95535-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="95535-124">altitude</span><span class="sxs-lookup"><span data-stu-id="95535-124">altitude</span></span>|<span data-ttu-id="95535-125">Double</span><span class="sxs-lookup"><span data-stu-id="95535-125">Double</span></span>|<span data-ttu-id="95535-126">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="95535-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="95535-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="95535-127">horizontalAccuracy</span></span>|<span data-ttu-id="95535-128">Double</span><span class="sxs-lookup"><span data-stu-id="95535-128">Double</span></span>|<span data-ttu-id="95535-129">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="95535-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="95535-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="95535-130">verticalAccuracy</span></span>|<span data-ttu-id="95535-131">Double</span><span class="sxs-lookup"><span data-stu-id="95535-131">Double</span></span>|<span data-ttu-id="95535-132">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="95535-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="95535-133">heading</span><span class="sxs-lookup"><span data-stu-id="95535-133">heading</span></span>|<span data-ttu-id="95535-134">Double</span><span class="sxs-lookup"><span data-stu-id="95535-134">Double</span></span>|<span data-ttu-id="95535-135">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="95535-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="95535-136">speed</span><span class="sxs-lookup"><span data-stu-id="95535-136">speed</span></span>|<span data-ttu-id="95535-137">Double</span><span class="sxs-lookup"><span data-stu-id="95535-137">Double</span></span>|<span data-ttu-id="95535-138">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="95535-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="95535-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95535-139">Relationships</span></span>
<span data-ttu-id="95535-140">なし</span><span class="sxs-lookup"><span data-stu-id="95535-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95535-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95535-141">JSON Representation</span></span>
<span data-ttu-id="95535-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95535-142">Here is a JSON representation of the resource.</span></span>
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




