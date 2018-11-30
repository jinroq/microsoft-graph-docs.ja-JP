---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
ms.openlocfilehash: fec7290ec559f411bed04e03166b31678d43036f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073164"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ab7d1-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab7d1-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="ab7d1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab7d1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab7d1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab7d1-107">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="ab7d1-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="ab7d1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7d1-108">Properties</span></span>
|<span data-ttu-id="ab7d1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7d1-109">Property</span></span>|<span data-ttu-id="ab7d1-110">型</span><span class="sxs-lookup"><span data-stu-id="ab7d1-110">Type</span></span>|<span data-ttu-id="ab7d1-111">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7d1-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab7d1-112">allowedDeviceCount</span></span>|<span data-ttu-id="ab7d1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7d1-113">Int32</span></span>|<span data-ttu-id="ab7d1-114">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ab7d1-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab7d1-115">blockedDeviceCount</span></span>|<span data-ttu-id="ab7d1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7d1-116">Int32</span></span>|<span data-ttu-id="ab7d1-117">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ab7d1-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab7d1-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="ab7d1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7d1-119">Int32</span></span>|<span data-ttu-id="ab7d1-120">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ab7d1-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab7d1-121">unknownDeviceCount</span></span>|<span data-ttu-id="ab7d1-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7d1-122">Int32</span></span>|<span data-ttu-id="ab7d1-123">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ab7d1-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab7d1-124">unavailableDeviceCount</span></span>|<span data-ttu-id="ab7d1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7d1-125">Int32</span></span>|<span data-ttu-id="ab7d1-126">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab7d1-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab7d1-127">Relationships</span></span>
<span data-ttu-id="ab7d1-128">なし</span><span class="sxs-lookup"><span data-stu-id="ab7d1-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab7d1-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab7d1-129">JSON Representation</span></span>
<span data-ttu-id="ab7d1-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab7d1-130">Here is a JSON representation of the resource.</span></span>
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





