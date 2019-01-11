---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 10eb3738e14e8239f92f8578d01b9d4888b06b24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829821"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="17266-103">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17266-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="17266-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17266-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17266-105">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="17266-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="17266-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17266-106">Properties</span></span>
|<span data-ttu-id="17266-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17266-107">Property</span></span>|<span data-ttu-id="17266-108">種類</span><span class="sxs-lookup"><span data-stu-id="17266-108">Type</span></span>|<span data-ttu-id="17266-109">説明</span><span class="sxs-lookup"><span data-stu-id="17266-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17266-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17266-110">allowedDeviceCount</span></span>|<span data-ttu-id="17266-111">Int32</span><span class="sxs-lookup"><span data-stu-id="17266-111">Int32</span></span>|<span data-ttu-id="17266-112">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="17266-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="17266-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17266-113">blockedDeviceCount</span></span>|<span data-ttu-id="17266-114">Int32</span><span class="sxs-lookup"><span data-stu-id="17266-114">Int32</span></span>|<span data-ttu-id="17266-115">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="17266-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="17266-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17266-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="17266-117">Int32</span><span class="sxs-lookup"><span data-stu-id="17266-117">Int32</span></span>|<span data-ttu-id="17266-118">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="17266-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="17266-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17266-119">unknownDeviceCount</span></span>|<span data-ttu-id="17266-120">Int32</span><span class="sxs-lookup"><span data-stu-id="17266-120">Int32</span></span>|<span data-ttu-id="17266-121">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="17266-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="17266-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17266-122">unavailableDeviceCount</span></span>|<span data-ttu-id="17266-123">Int32</span><span class="sxs-lookup"><span data-stu-id="17266-123">Int32</span></span>|<span data-ttu-id="17266-124">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="17266-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17266-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17266-125">Relationships</span></span>
<span data-ttu-id="17266-126">なし</span><span class="sxs-lookup"><span data-stu-id="17266-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17266-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17266-127">JSON Representation</span></span>
<span data-ttu-id="17266-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17266-128">Here is a JSON representation of the resource.</span></span>
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



