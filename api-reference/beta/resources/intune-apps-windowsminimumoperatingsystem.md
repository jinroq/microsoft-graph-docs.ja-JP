---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbee999b213d6c4b76a1203ac48b84c8dbeda3c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914648"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="6706e-103">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6706e-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="6706e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6706e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6706e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6706e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6706e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6706e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6706e-107">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="6706e-107">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="6706e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6706e-108">Properties</span></span>
|<span data-ttu-id="6706e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6706e-109">Property</span></span>|<span data-ttu-id="6706e-110">型</span><span class="sxs-lookup"><span data-stu-id="6706e-110">Type</span></span>|<span data-ttu-id="6706e-111">説明</span><span class="sxs-lookup"><span data-stu-id="6706e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6706e-112">v8_0</span><span class="sxs-lookup"><span data-stu-id="6706e-112">v8_0</span></span>|<span data-ttu-id="6706e-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6706e-113">Boolean</span></span>|<span data-ttu-id="6706e-114">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="6706e-114">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="6706e-115">v8_1</span><span class="sxs-lookup"><span data-stu-id="6706e-115">v8_1</span></span>|<span data-ttu-id="6706e-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6706e-116">Boolean</span></span>|<span data-ttu-id="6706e-117">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="6706e-117">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="6706e-118">v10_0</span><span class="sxs-lookup"><span data-stu-id="6706e-118">v10_0</span></span>|<span data-ttu-id="6706e-119">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6706e-119">Boolean</span></span>|<span data-ttu-id="6706e-120">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="6706e-120">Windows version 10.0 or later.</span></span>|
|<span data-ttu-id="6706e-121">v10_1607</span><span class="sxs-lookup"><span data-stu-id="6706e-121">v10_1607</span></span>|<span data-ttu-id="6706e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6706e-122">Boolean</span></span>|<span data-ttu-id="6706e-123">Windows 10 1607 以降です。</span><span class="sxs-lookup"><span data-stu-id="6706e-123">Windows 10 1607 or later.</span></span>|
|<span data-ttu-id="6706e-124">v10_1703</span><span class="sxs-lookup"><span data-stu-id="6706e-124">v10_1703</span></span>|<span data-ttu-id="6706e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6706e-125">Boolean</span></span>|<span data-ttu-id="6706e-126">10 1703 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="6706e-126">Windows 10 1703 or later.</span></span>|
|<span data-ttu-id="6706e-127">v10_1709</span><span class="sxs-lookup"><span data-stu-id="6706e-127">v10_1709</span></span>|<span data-ttu-id="6706e-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="6706e-128">Boolean</span></span>|<span data-ttu-id="6706e-129">10 1709 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="6706e-129">Windows 10 1709 or later.</span></span>|
|<span data-ttu-id="6706e-130">v10_1803</span><span class="sxs-lookup"><span data-stu-id="6706e-130">v10_1803</span></span>|<span data-ttu-id="6706e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6706e-131">Boolean</span></span>|<span data-ttu-id="6706e-132">10 1803 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="6706e-132">Windows 10 1803 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6706e-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6706e-133">Relationships</span></span>
<span data-ttu-id="6706e-134">なし</span><span class="sxs-lookup"><span data-stu-id="6706e-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6706e-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6706e-135">JSON Representation</span></span>
<span data-ttu-id="6706e-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6706e-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true
}
```





