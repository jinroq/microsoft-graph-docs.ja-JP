---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
ms.openlocfilehash: cb04de02e44f16534e9a57383e48d989a16f8582
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326601"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="d2832-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2832-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="d2832-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2832-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2832-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2832-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2832-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2832-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2832-107">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="d2832-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="d2832-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2832-108">Properties</span></span>
|<span data-ttu-id="d2832-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2832-109">Property</span></span>|<span data-ttu-id="d2832-110">種類</span><span class="sxs-lookup"><span data-stu-id="d2832-110">Type</span></span>|<span data-ttu-id="d2832-111">説明</span><span class="sxs-lookup"><span data-stu-id="d2832-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2832-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2832-112">allowedDeviceCount</span></span>|<span data-ttu-id="d2832-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d2832-113">Int32</span></span>|<span data-ttu-id="d2832-114">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="d2832-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="d2832-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2832-115">blockedDeviceCount</span></span>|<span data-ttu-id="d2832-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d2832-116">Int32</span></span>|<span data-ttu-id="d2832-117">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="d2832-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="d2832-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2832-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="d2832-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d2832-119">Int32</span></span>|<span data-ttu-id="d2832-120">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="d2832-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="d2832-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2832-121">unknownDeviceCount</span></span>|<span data-ttu-id="d2832-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d2832-122">Int32</span></span>|<span data-ttu-id="d2832-123">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="d2832-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="d2832-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2832-124">unavailableDeviceCount</span></span>|<span data-ttu-id="d2832-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d2832-125">Int32</span></span>|<span data-ttu-id="d2832-126">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="d2832-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2832-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2832-127">Relationships</span></span>
<span data-ttu-id="d2832-128">なし</span><span class="sxs-lookup"><span data-stu-id="d2832-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2832-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2832-129">JSON Representation</span></span>
<span data-ttu-id="d2832-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2832-130">Here is a JSON representation of the resource.</span></span>
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





