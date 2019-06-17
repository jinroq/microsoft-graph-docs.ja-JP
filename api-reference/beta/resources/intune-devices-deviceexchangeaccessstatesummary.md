---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81f9768deaaeebfaebf02beff35a70e795244050
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983142"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="b4c7f-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4c7f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="b4c7f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4c7f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c7f-106">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="b4c7f-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="b4c7f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4c7f-107">Properties</span></span>
|<span data-ttu-id="b4c7f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4c7f-108">Property</span></span>|<span data-ttu-id="b4c7f-109">型</span><span class="sxs-lookup"><span data-stu-id="b4c7f-109">Type</span></span>|<span data-ttu-id="b4c7f-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4c7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c7f-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4c7f-111">allowedDeviceCount</span></span>|<span data-ttu-id="b4c7f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c7f-112">Int32</span></span>|<span data-ttu-id="b4c7f-113">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="b4c7f-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4c7f-114">blockedDeviceCount</span></span>|<span data-ttu-id="b4c7f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c7f-115">Int32</span></span>|<span data-ttu-id="b4c7f-116">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="b4c7f-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4c7f-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="b4c7f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c7f-118">Int32</span></span>|<span data-ttu-id="b4c7f-119">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="b4c7f-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4c7f-120">unknownDeviceCount</span></span>|<span data-ttu-id="b4c7f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c7f-121">Int32</span></span>|<span data-ttu-id="b4c7f-122">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="b4c7f-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4c7f-123">unavailableDeviceCount</span></span>|<span data-ttu-id="b4c7f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c7f-124">Int32</span></span>|<span data-ttu-id="b4c7f-125">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4c7f-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4c7f-126">Relationships</span></span>
<span data-ttu-id="b4c7f-127">なし</span><span class="sxs-lookup"><span data-stu-id="b4c7f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4c7f-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4c7f-128">JSON Representation</span></span>
<span data-ttu-id="b4c7f-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4c7f-129">Here is a JSON representation of the resource.</span></span>
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





