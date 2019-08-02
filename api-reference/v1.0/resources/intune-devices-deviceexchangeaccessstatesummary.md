---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b975dbe09a5c1b277b55bfb7f13405d9871bd1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030843"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="5a9f5-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a9f5-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="5a9f5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a9f5-105">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="5a9f5-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="5a9f5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a9f5-106">Properties</span></span>
|<span data-ttu-id="5a9f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a9f5-107">Property</span></span>|<span data-ttu-id="5a9f5-108">型</span><span class="sxs-lookup"><span data-stu-id="5a9f5-108">Type</span></span>|<span data-ttu-id="5a9f5-109">説明</span><span class="sxs-lookup"><span data-stu-id="5a9f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a9f5-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a9f5-110">allowedDeviceCount</span></span>|<span data-ttu-id="5a9f5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9f5-111">Int32</span></span>|<span data-ttu-id="5a9f5-112">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="5a9f5-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a9f5-113">blockedDeviceCount</span></span>|<span data-ttu-id="5a9f5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9f5-114">Int32</span></span>|<span data-ttu-id="5a9f5-115">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="5a9f5-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a9f5-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="5a9f5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9f5-117">Int32</span></span>|<span data-ttu-id="5a9f5-118">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="5a9f5-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a9f5-119">unknownDeviceCount</span></span>|<span data-ttu-id="5a9f5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9f5-120">Int32</span></span>|<span data-ttu-id="5a9f5-121">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="5a9f5-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a9f5-122">unavailableDeviceCount</span></span>|<span data-ttu-id="5a9f5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9f5-123">Int32</span></span>|<span data-ttu-id="5a9f5-124">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a9f5-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a9f5-125">Relationships</span></span>
<span data-ttu-id="5a9f5-126">なし</span><span class="sxs-lookup"><span data-stu-id="5a9f5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a9f5-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a9f5-127">JSON Representation</span></span>
<span data-ttu-id="5a9f5-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a9f5-128">Here is a JSON representation of the resource.</span></span>
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



