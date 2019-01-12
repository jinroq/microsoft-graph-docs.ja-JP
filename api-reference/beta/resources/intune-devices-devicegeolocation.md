---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef73925c31b58327f0e0b89d5682035d14d38afc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943101"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="9494b-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9494b-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="9494b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9494b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9494b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9494b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9494b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9494b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9494b-107">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="9494b-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="9494b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9494b-108">Properties</span></span>
|<span data-ttu-id="9494b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9494b-109">Property</span></span>|<span data-ttu-id="9494b-110">型</span><span class="sxs-lookup"><span data-stu-id="9494b-110">Type</span></span>|<span data-ttu-id="9494b-111">説明</span><span class="sxs-lookup"><span data-stu-id="9494b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9494b-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="9494b-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="9494b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9494b-113">DateTimeOffset</span></span>|<span data-ttu-id="9494b-114">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="9494b-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="9494b-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="9494b-115">lastCollectedDateTime</span></span>|<span data-ttu-id="9494b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9494b-116">DateTimeOffset</span></span>|<span data-ttu-id="9494b-117">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="9494b-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="9494b-118">longitude</span><span class="sxs-lookup"><span data-stu-id="9494b-118">longitude</span></span>|<span data-ttu-id="9494b-119">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-119">Double</span></span>|<span data-ttu-id="9494b-120">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="9494b-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="9494b-121">latitude</span><span class="sxs-lookup"><span data-stu-id="9494b-121">latitude</span></span>|<span data-ttu-id="9494b-122">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-122">Double</span></span>|<span data-ttu-id="9494b-123">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="9494b-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="9494b-124">altitude</span><span class="sxs-lookup"><span data-stu-id="9494b-124">altitude</span></span>|<span data-ttu-id="9494b-125">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-125">Double</span></span>|<span data-ttu-id="9494b-126">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="9494b-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="9494b-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="9494b-127">horizontalAccuracy</span></span>|<span data-ttu-id="9494b-128">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-128">Double</span></span>|<span data-ttu-id="9494b-129">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="9494b-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="9494b-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="9494b-130">verticalAccuracy</span></span>|<span data-ttu-id="9494b-131">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-131">Double</span></span>|<span data-ttu-id="9494b-132">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="9494b-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="9494b-133">heading</span><span class="sxs-lookup"><span data-stu-id="9494b-133">heading</span></span>|<span data-ttu-id="9494b-134">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-134">Double</span></span>|<span data-ttu-id="9494b-135">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="9494b-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="9494b-136">speed</span><span class="sxs-lookup"><span data-stu-id="9494b-136">speed</span></span>|<span data-ttu-id="9494b-137">Double</span><span class="sxs-lookup"><span data-stu-id="9494b-137">Double</span></span>|<span data-ttu-id="9494b-138">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="9494b-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="9494b-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9494b-139">Relationships</span></span>
<span data-ttu-id="9494b-140">なし</span><span class="sxs-lookup"><span data-stu-id="9494b-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9494b-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9494b-141">JSON Representation</span></span>
<span data-ttu-id="9494b-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9494b-142">Here is a JSON representation of the resource.</span></span>
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





