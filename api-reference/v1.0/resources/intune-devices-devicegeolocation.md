---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
ms.openlocfilehash: fe8ffe7684132c9871225747a28905da1983672d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336996"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="f0324-103">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0324-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="f0324-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0324-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0324-105">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="f0324-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="f0324-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0324-106">Properties</span></span>
|<span data-ttu-id="f0324-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0324-107">Property</span></span>|<span data-ttu-id="f0324-108">種類</span><span class="sxs-lookup"><span data-stu-id="f0324-108">Type</span></span>|<span data-ttu-id="f0324-109">説明</span><span class="sxs-lookup"><span data-stu-id="f0324-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0324-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0324-110">lastCollectedDateTime</span></span>|<span data-ttu-id="f0324-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0324-111">DateTimeOffset</span></span>|<span data-ttu-id="f0324-112">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="f0324-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="f0324-113">longitude</span><span class="sxs-lookup"><span data-stu-id="f0324-113">longitude</span></span>|<span data-ttu-id="f0324-114">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-114">Double</span></span>|<span data-ttu-id="f0324-115">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="f0324-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f0324-116">latitude</span><span class="sxs-lookup"><span data-stu-id="f0324-116">latitude</span></span>|<span data-ttu-id="f0324-117">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-117">Double</span></span>|<span data-ttu-id="f0324-118">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="f0324-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f0324-119">altitude</span><span class="sxs-lookup"><span data-stu-id="f0324-119">altitude</span></span>|<span data-ttu-id="f0324-120">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-120">Double</span></span>|<span data-ttu-id="f0324-121">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="f0324-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="f0324-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f0324-122">horizontalAccuracy</span></span>|<span data-ttu-id="f0324-123">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-123">Double</span></span>|<span data-ttu-id="f0324-124">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="f0324-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="f0324-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f0324-125">verticalAccuracy</span></span>|<span data-ttu-id="f0324-126">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-126">Double</span></span>|<span data-ttu-id="f0324-127">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="f0324-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="f0324-128">heading</span><span class="sxs-lookup"><span data-stu-id="f0324-128">heading</span></span>|<span data-ttu-id="f0324-129">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-129">Double</span></span>|<span data-ttu-id="f0324-130">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="f0324-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="f0324-131">speed</span><span class="sxs-lookup"><span data-stu-id="f0324-131">speed</span></span>|<span data-ttu-id="f0324-132">Double</span><span class="sxs-lookup"><span data-stu-id="f0324-132">Double</span></span>|<span data-ttu-id="f0324-133">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="f0324-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0324-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0324-134">Relationships</span></span>
<span data-ttu-id="f0324-135">なし</span><span class="sxs-lookup"><span data-stu-id="f0324-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0324-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0324-136">JSON Representation</span></span>
<span data-ttu-id="f0324-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0324-137">Here is a JSON representation of the resource.</span></span>
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



