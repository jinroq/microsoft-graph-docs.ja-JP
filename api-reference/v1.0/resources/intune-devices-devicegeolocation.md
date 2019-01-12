---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 248af3f66a78e3197a3f966225e864f5583f8597
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940954"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="76c13-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76c13-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="76c13-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76c13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76c13-105">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="76c13-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="76c13-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76c13-106">Properties</span></span>
|<span data-ttu-id="76c13-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76c13-107">Property</span></span>|<span data-ttu-id="76c13-108">型</span><span class="sxs-lookup"><span data-stu-id="76c13-108">Type</span></span>|<span data-ttu-id="76c13-109">説明</span><span class="sxs-lookup"><span data-stu-id="76c13-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c13-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="76c13-110">lastCollectedDateTime</span></span>|<span data-ttu-id="76c13-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76c13-111">DateTimeOffset</span></span>|<span data-ttu-id="76c13-112">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="76c13-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="76c13-113">longitude</span><span class="sxs-lookup"><span data-stu-id="76c13-113">longitude</span></span>|<span data-ttu-id="76c13-114">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-114">Double</span></span>|<span data-ttu-id="76c13-115">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="76c13-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="76c13-116">latitude</span><span class="sxs-lookup"><span data-stu-id="76c13-116">latitude</span></span>|<span data-ttu-id="76c13-117">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-117">Double</span></span>|<span data-ttu-id="76c13-118">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="76c13-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="76c13-119">altitude</span><span class="sxs-lookup"><span data-stu-id="76c13-119">altitude</span></span>|<span data-ttu-id="76c13-120">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-120">Double</span></span>|<span data-ttu-id="76c13-121">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="76c13-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="76c13-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="76c13-122">horizontalAccuracy</span></span>|<span data-ttu-id="76c13-123">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-123">Double</span></span>|<span data-ttu-id="76c13-124">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="76c13-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="76c13-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="76c13-125">verticalAccuracy</span></span>|<span data-ttu-id="76c13-126">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-126">Double</span></span>|<span data-ttu-id="76c13-127">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="76c13-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="76c13-128">heading</span><span class="sxs-lookup"><span data-stu-id="76c13-128">heading</span></span>|<span data-ttu-id="76c13-129">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-129">Double</span></span>|<span data-ttu-id="76c13-130">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="76c13-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="76c13-131">speed</span><span class="sxs-lookup"><span data-stu-id="76c13-131">speed</span></span>|<span data-ttu-id="76c13-132">Double</span><span class="sxs-lookup"><span data-stu-id="76c13-132">Double</span></span>|<span data-ttu-id="76c13-133">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="76c13-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="76c13-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76c13-134">Relationships</span></span>
<span data-ttu-id="76c13-135">なし</span><span class="sxs-lookup"><span data-stu-id="76c13-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76c13-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76c13-136">JSON Representation</span></span>
<span data-ttu-id="76c13-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76c13-137">Here is a JSON representation of the resource.</span></span>
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



