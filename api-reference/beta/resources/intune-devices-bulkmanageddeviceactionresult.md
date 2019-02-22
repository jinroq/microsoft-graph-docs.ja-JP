---
title: bulkmanageddeviceactionresult リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199fe08b4eaf339f17fdb67bb6dbcc0243fd90f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168335"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="df749-103">bulkmanageddeviceactionresult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df749-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="df749-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df749-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df749-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df749-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df749-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="df749-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="df749-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df749-107">Properties</span></span>
|<span data-ttu-id="df749-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df749-108">Property</span></span>|<span data-ttu-id="df749-109">型</span><span class="sxs-lookup"><span data-stu-id="df749-109">Type</span></span>|<span data-ttu-id="df749-110">説明</span><span class="sxs-lookup"><span data-stu-id="df749-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df749-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="df749-111">successfulDeviceIds</span></span>|<span data-ttu-id="df749-112">String collection</span><span class="sxs-lookup"><span data-stu-id="df749-112">String collection</span></span>|<span data-ttu-id="df749-113">成功したデバイス</span><span class="sxs-lookup"><span data-stu-id="df749-113">Successful devices</span></span>|
|<span data-ttu-id="df749-114">失敗 deviceid</span><span class="sxs-lookup"><span data-stu-id="df749-114">failedDeviceIds</span></span>|<span data-ttu-id="df749-115">String collection</span><span class="sxs-lookup"><span data-stu-id="df749-115">String collection</span></span>|<span data-ttu-id="df749-116">失敗したデバイス</span><span class="sxs-lookup"><span data-stu-id="df749-116">Failed devices</span></span>|
|<span data-ttu-id="df749-117">not見つかり deviceid</span><span class="sxs-lookup"><span data-stu-id="df749-117">notFoundDeviceIds</span></span>|<span data-ttu-id="df749-118">String collection</span><span class="sxs-lookup"><span data-stu-id="df749-118">String collection</span></span>|<span data-ttu-id="df749-119">見つからないデバイス</span><span class="sxs-lookup"><span data-stu-id="df749-119">Not found devices</span></span>|
|<span data-ttu-id="df749-120">notsupporteddeviceids</span><span class="sxs-lookup"><span data-stu-id="df749-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="df749-121">String collection</span><span class="sxs-lookup"><span data-stu-id="df749-121">String collection</span></span>|<span data-ttu-id="df749-122">サポートされていないデバイス</span><span class="sxs-lookup"><span data-stu-id="df749-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="df749-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df749-123">Relationships</span></span>
<span data-ttu-id="df749-124">なし</span><span class="sxs-lookup"><span data-stu-id="df749-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df749-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df749-125">JSON Representation</span></span>
<span data-ttu-id="df749-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df749-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```




