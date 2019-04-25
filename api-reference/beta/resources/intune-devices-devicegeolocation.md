---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acf2987e7c022754ff0659d82027b4d0d26901bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524443"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="a2356-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2356-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="a2356-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2356-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2356-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2356-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2356-106">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="a2356-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="a2356-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2356-107">Properties</span></span>
|<span data-ttu-id="a2356-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2356-108">Property</span></span>|<span data-ttu-id="a2356-109">型</span><span class="sxs-lookup"><span data-stu-id="a2356-109">Type</span></span>|<span data-ttu-id="a2356-110">説明</span><span class="sxs-lookup"><span data-stu-id="a2356-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2356-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="a2356-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="a2356-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2356-112">DateTimeOffset</span></span>|<span data-ttu-id="a2356-113">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="a2356-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="a2356-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2356-114">lastCollectedDateTime</span></span>|<span data-ttu-id="a2356-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2356-115">DateTimeOffset</span></span>|<span data-ttu-id="a2356-116">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="a2356-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="a2356-117">longitude</span><span class="sxs-lookup"><span data-stu-id="a2356-117">longitude</span></span>|<span data-ttu-id="a2356-118">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-118">Double</span></span>|<span data-ttu-id="a2356-119">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="a2356-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a2356-120">latitude</span><span class="sxs-lookup"><span data-stu-id="a2356-120">latitude</span></span>|<span data-ttu-id="a2356-121">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-121">Double</span></span>|<span data-ttu-id="a2356-122">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="a2356-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a2356-123">altitude</span><span class="sxs-lookup"><span data-stu-id="a2356-123">altitude</span></span>|<span data-ttu-id="a2356-124">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-124">Double</span></span>|<span data-ttu-id="a2356-125">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="a2356-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="a2356-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a2356-126">horizontalAccuracy</span></span>|<span data-ttu-id="a2356-127">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-127">Double</span></span>|<span data-ttu-id="a2356-128">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="a2356-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="a2356-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a2356-129">verticalAccuracy</span></span>|<span data-ttu-id="a2356-130">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-130">Double</span></span>|<span data-ttu-id="a2356-131">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="a2356-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="a2356-132">heading</span><span class="sxs-lookup"><span data-stu-id="a2356-132">heading</span></span>|<span data-ttu-id="a2356-133">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a2356-133">Double</span></span>|<span data-ttu-id="a2356-134">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="a2356-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="a2356-135">speed</span><span class="sxs-lookup"><span data-stu-id="a2356-135">speed</span></span>|<span data-ttu-id="a2356-136">Double</span><span class="sxs-lookup"><span data-stu-id="a2356-136">Double</span></span>|<span data-ttu-id="a2356-137">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="a2356-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2356-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2356-138">Relationships</span></span>
<span data-ttu-id="a2356-139">なし</span><span class="sxs-lookup"><span data-stu-id="a2356-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2356-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2356-140">JSON Representation</span></span>
<span data-ttu-id="a2356-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2356-141">Here is a JSON representation of the resource.</span></span>
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





