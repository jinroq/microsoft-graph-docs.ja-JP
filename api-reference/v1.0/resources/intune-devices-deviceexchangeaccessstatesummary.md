---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
ms.openlocfilehash: dd2784078e8b44b1a02cb5a0013c1e38804912c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301744"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="b16f5-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b16f5-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="b16f5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b16f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b16f5-105">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="b16f5-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="b16f5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b16f5-106">Properties</span></span>
|<span data-ttu-id="b16f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b16f5-107">Property</span></span>|<span data-ttu-id="b16f5-108">種類</span><span class="sxs-lookup"><span data-stu-id="b16f5-108">Type</span></span>|<span data-ttu-id="b16f5-109">説明</span><span class="sxs-lookup"><span data-stu-id="b16f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b16f5-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b16f5-110">allowedDeviceCount</span></span>|<span data-ttu-id="b16f5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b16f5-111">Int32</span></span>|<span data-ttu-id="b16f5-112">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="b16f5-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b16f5-113">blockedDeviceCount</span></span>|<span data-ttu-id="b16f5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b16f5-114">Int32</span></span>|<span data-ttu-id="b16f5-115">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="b16f5-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b16f5-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="b16f5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b16f5-117">Int32</span></span>|<span data-ttu-id="b16f5-118">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="b16f5-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b16f5-119">unknownDeviceCount</span></span>|<span data-ttu-id="b16f5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b16f5-120">Int32</span></span>|<span data-ttu-id="b16f5-121">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="b16f5-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b16f5-122">unavailableDeviceCount</span></span>|<span data-ttu-id="b16f5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b16f5-123">Int32</span></span>|<span data-ttu-id="b16f5-124">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b16f5-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b16f5-125">Relationships</span></span>
<span data-ttu-id="b16f5-126">なし</span><span class="sxs-lookup"><span data-stu-id="b16f5-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b16f5-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b16f5-127">JSON Representation</span></span>
<span data-ttu-id="b16f5-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b16f5-128">Here is a JSON representation of the resource.</span></span>
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



