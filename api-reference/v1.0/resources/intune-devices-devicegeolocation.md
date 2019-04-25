---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542033"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="c2091-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c2091-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="c2091-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2091-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2091-105">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="c2091-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="c2091-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2091-106">Properties</span></span>
|<span data-ttu-id="c2091-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2091-107">Property</span></span>|<span data-ttu-id="c2091-108">型</span><span class="sxs-lookup"><span data-stu-id="c2091-108">Type</span></span>|<span data-ttu-id="c2091-109">説明</span><span class="sxs-lookup"><span data-stu-id="c2091-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2091-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2091-110">lastCollectedDateTime</span></span>|<span data-ttu-id="c2091-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2091-111">DateTimeOffset</span></span>|<span data-ttu-id="c2091-112">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="c2091-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="c2091-113">longitude</span><span class="sxs-lookup"><span data-stu-id="c2091-113">longitude</span></span>|<span data-ttu-id="c2091-114">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-114">Double</span></span>|<span data-ttu-id="c2091-115">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="c2091-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="c2091-116">latitude</span><span class="sxs-lookup"><span data-stu-id="c2091-116">latitude</span></span>|<span data-ttu-id="c2091-117">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-117">Double</span></span>|<span data-ttu-id="c2091-118">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="c2091-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="c2091-119">altitude</span><span class="sxs-lookup"><span data-stu-id="c2091-119">altitude</span></span>|<span data-ttu-id="c2091-120">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-120">Double</span></span>|<span data-ttu-id="c2091-121">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="c2091-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="c2091-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="c2091-122">horizontalAccuracy</span></span>|<span data-ttu-id="c2091-123">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-123">Double</span></span>|<span data-ttu-id="c2091-124">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="c2091-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="c2091-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="c2091-125">verticalAccuracy</span></span>|<span data-ttu-id="c2091-126">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-126">Double</span></span>|<span data-ttu-id="c2091-127">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="c2091-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="c2091-128">heading</span><span class="sxs-lookup"><span data-stu-id="c2091-128">heading</span></span>|<span data-ttu-id="c2091-129">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c2091-129">Double</span></span>|<span data-ttu-id="c2091-130">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="c2091-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="c2091-131">speed</span><span class="sxs-lookup"><span data-stu-id="c2091-131">speed</span></span>|<span data-ttu-id="c2091-132">Double</span><span class="sxs-lookup"><span data-stu-id="c2091-132">Double</span></span>|<span data-ttu-id="c2091-133">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="c2091-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2091-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2091-134">Relationships</span></span>
<span data-ttu-id="c2091-135">なし</span><span class="sxs-lookup"><span data-stu-id="c2091-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2091-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2091-136">JSON Representation</span></span>
<span data-ttu-id="c2091-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c2091-137">Here is a JSON representation of the resource.</span></span>
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



