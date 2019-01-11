---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7243b337a53cca31054f99ae807e5c17cdd3e372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876270"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="28ad3-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28ad3-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="28ad3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28ad3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28ad3-105">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="28ad3-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="28ad3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28ad3-106">Properties</span></span>
|<span data-ttu-id="28ad3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28ad3-107">Property</span></span>|<span data-ttu-id="28ad3-108">種類</span><span class="sxs-lookup"><span data-stu-id="28ad3-108">Type</span></span>|<span data-ttu-id="28ad3-109">説明</span><span class="sxs-lookup"><span data-stu-id="28ad3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28ad3-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="28ad3-110">v8_0</span></span>|<span data-ttu-id="28ad3-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="28ad3-111">Boolean</span></span>|<span data-ttu-id="28ad3-112">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="28ad3-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="28ad3-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="28ad3-113">v9_0</span></span>|<span data-ttu-id="28ad3-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="28ad3-114">Boolean</span></span>|<span data-ttu-id="28ad3-115">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="28ad3-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="28ad3-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="28ad3-116">v10_0</span></span>|<span data-ttu-id="28ad3-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="28ad3-117">Boolean</span></span>|<span data-ttu-id="28ad3-118">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="28ad3-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="28ad3-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="28ad3-119">v11_0</span></span>|<span data-ttu-id="28ad3-120">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="28ad3-120">Boolean</span></span>|<span data-ttu-id="28ad3-121">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="28ad3-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="28ad3-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="28ad3-122">v12_0</span></span>|<span data-ttu-id="28ad3-123">ブール型</span><span class="sxs-lookup"><span data-stu-id="28ad3-123">Boolean</span></span>|<span data-ttu-id="28ad3-124">12.0 またはそれ以降のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="28ad3-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28ad3-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28ad3-125">Relationships</span></span>
<span data-ttu-id="28ad3-126">なし</span><span class="sxs-lookup"><span data-stu-id="28ad3-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28ad3-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28ad3-127">JSON Representation</span></span>
<span data-ttu-id="28ad3-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28ad3-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



