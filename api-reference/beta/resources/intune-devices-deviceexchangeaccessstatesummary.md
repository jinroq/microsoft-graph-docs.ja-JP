---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8ca08b026b8e1cdbac4bd0dc73331a9d5df80fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889986"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="eaa22-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eaa22-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="eaa22-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eaa22-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa22-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaa22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaa22-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eaa22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaa22-107">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="eaa22-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="eaa22-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eaa22-108">Properties</span></span>
|<span data-ttu-id="eaa22-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eaa22-109">Property</span></span>|<span data-ttu-id="eaa22-110">種類</span><span class="sxs-lookup"><span data-stu-id="eaa22-110">Type</span></span>|<span data-ttu-id="eaa22-111">説明</span><span class="sxs-lookup"><span data-stu-id="eaa22-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaa22-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eaa22-112">allowedDeviceCount</span></span>|<span data-ttu-id="eaa22-113">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa22-113">Int32</span></span>|<span data-ttu-id="eaa22-114">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="eaa22-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eaa22-115">blockedDeviceCount</span></span>|<span data-ttu-id="eaa22-116">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa22-116">Int32</span></span>|<span data-ttu-id="eaa22-117">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="eaa22-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eaa22-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="eaa22-119">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa22-119">Int32</span></span>|<span data-ttu-id="eaa22-120">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="eaa22-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eaa22-121">unknownDeviceCount</span></span>|<span data-ttu-id="eaa22-122">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa22-122">Int32</span></span>|<span data-ttu-id="eaa22-123">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="eaa22-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eaa22-124">unavailableDeviceCount</span></span>|<span data-ttu-id="eaa22-125">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa22-125">Int32</span></span>|<span data-ttu-id="eaa22-126">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaa22-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eaa22-127">Relationships</span></span>
<span data-ttu-id="eaa22-128">なし</span><span class="sxs-lookup"><span data-stu-id="eaa22-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eaa22-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eaa22-129">JSON Representation</span></span>
<span data-ttu-id="eaa22-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eaa22-130">Here is a JSON representation of the resource.</span></span>
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





