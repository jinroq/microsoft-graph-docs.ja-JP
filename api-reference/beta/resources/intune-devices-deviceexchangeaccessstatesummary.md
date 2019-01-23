---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a01a1207801063285d7b59f0fa51c474ae78fb6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418555"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="4188f-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4188f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="4188f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4188f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4188f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4188f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4188f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4188f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4188f-107">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="4188f-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="4188f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4188f-108">Properties</span></span>
|<span data-ttu-id="4188f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4188f-109">Property</span></span>|<span data-ttu-id="4188f-110">型</span><span class="sxs-lookup"><span data-stu-id="4188f-110">Type</span></span>|<span data-ttu-id="4188f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4188f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4188f-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4188f-112">allowedDeviceCount</span></span>|<span data-ttu-id="4188f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4188f-113">Int32</span></span>|<span data-ttu-id="4188f-114">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="4188f-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="4188f-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4188f-115">blockedDeviceCount</span></span>|<span data-ttu-id="4188f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4188f-116">Int32</span></span>|<span data-ttu-id="4188f-117">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="4188f-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="4188f-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4188f-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="4188f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4188f-119">Int32</span></span>|<span data-ttu-id="4188f-120">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="4188f-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="4188f-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4188f-121">unknownDeviceCount</span></span>|<span data-ttu-id="4188f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4188f-122">Int32</span></span>|<span data-ttu-id="4188f-123">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="4188f-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="4188f-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4188f-124">unavailableDeviceCount</span></span>|<span data-ttu-id="4188f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4188f-125">Int32</span></span>|<span data-ttu-id="4188f-126">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="4188f-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4188f-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4188f-127">Relationships</span></span>
<span data-ttu-id="4188f-128">なし</span><span class="sxs-lookup"><span data-stu-id="4188f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4188f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4188f-129">JSON Representation</span></span>
<span data-ttu-id="4188f-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4188f-130">Here is a JSON representation of the resource.</span></span>
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




