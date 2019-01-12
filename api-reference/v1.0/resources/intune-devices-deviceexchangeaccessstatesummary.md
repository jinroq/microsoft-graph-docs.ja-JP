---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 389bba96adc477e90244f6f9800da09ff3e87992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990538"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="13b10-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13b10-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="13b10-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13b10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13b10-105">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="13b10-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="13b10-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13b10-106">Properties</span></span>
|<span data-ttu-id="13b10-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13b10-107">Property</span></span>|<span data-ttu-id="13b10-108">型</span><span class="sxs-lookup"><span data-stu-id="13b10-108">Type</span></span>|<span data-ttu-id="13b10-109">説明</span><span class="sxs-lookup"><span data-stu-id="13b10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b10-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13b10-110">allowedDeviceCount</span></span>|<span data-ttu-id="13b10-111">Int32</span><span class="sxs-lookup"><span data-stu-id="13b10-111">Int32</span></span>|<span data-ttu-id="13b10-112">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="13b10-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="13b10-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13b10-113">blockedDeviceCount</span></span>|<span data-ttu-id="13b10-114">Int32</span><span class="sxs-lookup"><span data-stu-id="13b10-114">Int32</span></span>|<span data-ttu-id="13b10-115">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="13b10-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="13b10-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13b10-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="13b10-117">Int32</span><span class="sxs-lookup"><span data-stu-id="13b10-117">Int32</span></span>|<span data-ttu-id="13b10-118">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="13b10-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="13b10-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13b10-119">unknownDeviceCount</span></span>|<span data-ttu-id="13b10-120">Int32</span><span class="sxs-lookup"><span data-stu-id="13b10-120">Int32</span></span>|<span data-ttu-id="13b10-121">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="13b10-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="13b10-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13b10-122">unavailableDeviceCount</span></span>|<span data-ttu-id="13b10-123">Int32</span><span class="sxs-lookup"><span data-stu-id="13b10-123">Int32</span></span>|<span data-ttu-id="13b10-124">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="13b10-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b10-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13b10-125">Relationships</span></span>
<span data-ttu-id="13b10-126">なし</span><span class="sxs-lookup"><span data-stu-id="13b10-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13b10-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13b10-127">JSON Representation</span></span>
<span data-ttu-id="13b10-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13b10-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



