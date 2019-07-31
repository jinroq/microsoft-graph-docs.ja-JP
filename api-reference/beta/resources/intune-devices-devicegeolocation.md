---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70d2f943adee1710c56900191111b3c724bf5e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968492"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="3ef30-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ef30-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="3ef30-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ef30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ef30-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ef30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ef30-106">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="3ef30-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="3ef30-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ef30-107">Properties</span></span>
|<span data-ttu-id="3ef30-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ef30-108">Property</span></span>|<span data-ttu-id="3ef30-109">型</span><span class="sxs-lookup"><span data-stu-id="3ef30-109">Type</span></span>|<span data-ttu-id="3ef30-110">説明</span><span class="sxs-lookup"><span data-stu-id="3ef30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef30-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="3ef30-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="3ef30-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ef30-112">DateTimeOffset</span></span>|<span data-ttu-id="3ef30-113">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="3ef30-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3ef30-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ef30-114">lastCollectedDateTime</span></span>|<span data-ttu-id="3ef30-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ef30-115">DateTimeOffset</span></span>|<span data-ttu-id="3ef30-116">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="3ef30-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3ef30-117">longitude</span><span class="sxs-lookup"><span data-stu-id="3ef30-117">longitude</span></span>|<span data-ttu-id="3ef30-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="3ef30-118">Double</span></span>|<span data-ttu-id="3ef30-119">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="3ef30-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3ef30-120">latitude</span><span class="sxs-lookup"><span data-stu-id="3ef30-120">latitude</span></span>|<span data-ttu-id="3ef30-121">2 行分</span><span class="sxs-lookup"><span data-stu-id="3ef30-121">Double</span></span>|<span data-ttu-id="3ef30-122">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="3ef30-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3ef30-123">altitude</span><span class="sxs-lookup"><span data-stu-id="3ef30-123">altitude</span></span>|<span data-ttu-id="3ef30-124">2 行分</span><span class="sxs-lookup"><span data-stu-id="3ef30-124">Double</span></span>|<span data-ttu-id="3ef30-125">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="3ef30-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="3ef30-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3ef30-126">horizontalAccuracy</span></span>|<span data-ttu-id="3ef30-127">2 行分</span><span class="sxs-lookup"><span data-stu-id="3ef30-127">Double</span></span>|<span data-ttu-id="3ef30-128">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="3ef30-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="3ef30-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3ef30-129">verticalAccuracy</span></span>|<span data-ttu-id="3ef30-130">2 行分</span><span class="sxs-lookup"><span data-stu-id="3ef30-130">Double</span></span>|<span data-ttu-id="3ef30-131">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="3ef30-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="3ef30-132">heading</span><span class="sxs-lookup"><span data-stu-id="3ef30-132">heading</span></span>|<span data-ttu-id="3ef30-133">2 行分</span><span class="sxs-lookup"><span data-stu-id="3ef30-133">Double</span></span>|<span data-ttu-id="3ef30-134">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="3ef30-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="3ef30-135">speed</span><span class="sxs-lookup"><span data-stu-id="3ef30-135">speed</span></span>|<span data-ttu-id="3ef30-136">Double</span><span class="sxs-lookup"><span data-stu-id="3ef30-136">Double</span></span>|<span data-ttu-id="3ef30-137">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="3ef30-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ef30-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ef30-138">Relationships</span></span>
<span data-ttu-id="3ef30-139">なし</span><span class="sxs-lookup"><span data-stu-id="3ef30-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ef30-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ef30-140">JSON Representation</span></span>
<span data-ttu-id="3ef30-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ef30-141">Here is a JSON representation of the resource.</span></span>
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





