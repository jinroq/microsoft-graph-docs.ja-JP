---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541991"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="96b12-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96b12-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="96b12-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96b12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96b12-105">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="96b12-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="96b12-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b12-106">Properties</span></span>
|<span data-ttu-id="96b12-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b12-107">Property</span></span>|<span data-ttu-id="96b12-108">型</span><span class="sxs-lookup"><span data-stu-id="96b12-108">Type</span></span>|<span data-ttu-id="96b12-109">説明</span><span class="sxs-lookup"><span data-stu-id="96b12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96b12-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b12-110">allowedDeviceCount</span></span>|<span data-ttu-id="96b12-111">Int32</span><span class="sxs-lookup"><span data-stu-id="96b12-111">Int32</span></span>|<span data-ttu-id="96b12-112">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="96b12-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="96b12-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b12-113">blockedDeviceCount</span></span>|<span data-ttu-id="96b12-114">Int32</span><span class="sxs-lookup"><span data-stu-id="96b12-114">Int32</span></span>|<span data-ttu-id="96b12-115">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="96b12-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="96b12-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b12-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="96b12-117">Int32</span><span class="sxs-lookup"><span data-stu-id="96b12-117">Int32</span></span>|<span data-ttu-id="96b12-118">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="96b12-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="96b12-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b12-119">unknownDeviceCount</span></span>|<span data-ttu-id="96b12-120">Int32</span><span class="sxs-lookup"><span data-stu-id="96b12-120">Int32</span></span>|<span data-ttu-id="96b12-121">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="96b12-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="96b12-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b12-122">unavailableDeviceCount</span></span>|<span data-ttu-id="96b12-123">Int32</span><span class="sxs-lookup"><span data-stu-id="96b12-123">Int32</span></span>|<span data-ttu-id="96b12-124">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="96b12-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96b12-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96b12-125">Relationships</span></span>
<span data-ttu-id="96b12-126">なし</span><span class="sxs-lookup"><span data-stu-id="96b12-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96b12-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96b12-127">JSON Representation</span></span>
<span data-ttu-id="96b12-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96b12-128">Here is a JSON representation of the resource.</span></span>
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



