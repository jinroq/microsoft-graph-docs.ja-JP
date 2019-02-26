---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260215"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="092d2-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="092d2-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="092d2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="092d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="092d2-105">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="092d2-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="092d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="092d2-106">Properties</span></span>
|<span data-ttu-id="092d2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="092d2-107">Property</span></span>|<span data-ttu-id="092d2-108">型</span><span class="sxs-lookup"><span data-stu-id="092d2-108">Type</span></span>|<span data-ttu-id="092d2-109">説明</span><span class="sxs-lookup"><span data-stu-id="092d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="092d2-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="092d2-110">lastCollectedDateTime</span></span>|<span data-ttu-id="092d2-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="092d2-111">DateTimeOffset</span></span>|<span data-ttu-id="092d2-112">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="092d2-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="092d2-113">longitude</span><span class="sxs-lookup"><span data-stu-id="092d2-113">longitude</span></span>|<span data-ttu-id="092d2-114">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-114">Double</span></span>|<span data-ttu-id="092d2-115">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="092d2-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="092d2-116">latitude</span><span class="sxs-lookup"><span data-stu-id="092d2-116">latitude</span></span>|<span data-ttu-id="092d2-117">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-117">Double</span></span>|<span data-ttu-id="092d2-118">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="092d2-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="092d2-119">altitude</span><span class="sxs-lookup"><span data-stu-id="092d2-119">altitude</span></span>|<span data-ttu-id="092d2-120">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-120">Double</span></span>|<span data-ttu-id="092d2-121">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="092d2-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="092d2-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="092d2-122">horizontalAccuracy</span></span>|<span data-ttu-id="092d2-123">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-123">Double</span></span>|<span data-ttu-id="092d2-124">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="092d2-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="092d2-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="092d2-125">verticalAccuracy</span></span>|<span data-ttu-id="092d2-126">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-126">Double</span></span>|<span data-ttu-id="092d2-127">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="092d2-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="092d2-128">heading</span><span class="sxs-lookup"><span data-stu-id="092d2-128">heading</span></span>|<span data-ttu-id="092d2-129">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="092d2-129">Double</span></span>|<span data-ttu-id="092d2-130">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="092d2-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="092d2-131">speed</span><span class="sxs-lookup"><span data-stu-id="092d2-131">speed</span></span>|<span data-ttu-id="092d2-132">Double</span><span class="sxs-lookup"><span data-stu-id="092d2-132">Double</span></span>|<span data-ttu-id="092d2-133">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="092d2-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="092d2-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="092d2-134">Relationships</span></span>
<span data-ttu-id="092d2-135">なし</span><span class="sxs-lookup"><span data-stu-id="092d2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="092d2-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="092d2-136">JSON Representation</span></span>
<span data-ttu-id="092d2-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="092d2-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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



