---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c293e7490df1e7a6c53628b49440a050ee21a39
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395819"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="bee47-103">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bee47-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="bee47-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bee47-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bee47-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bee47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bee47-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bee47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee47-107">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="bee47-107">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="bee47-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bee47-108">Properties</span></span>
|<span data-ttu-id="bee47-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bee47-109">Property</span></span>|<span data-ttu-id="bee47-110">型</span><span class="sxs-lookup"><span data-stu-id="bee47-110">Type</span></span>|<span data-ttu-id="bee47-111">説明</span><span class="sxs-lookup"><span data-stu-id="bee47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee47-112">v8_0</span><span class="sxs-lookup"><span data-stu-id="bee47-112">v8_0</span></span>|<span data-ttu-id="bee47-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bee47-113">Boolean</span></span>|<span data-ttu-id="bee47-114">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="bee47-114">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="bee47-115">v8_1</span><span class="sxs-lookup"><span data-stu-id="bee47-115">v8_1</span></span>|<span data-ttu-id="bee47-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bee47-116">Boolean</span></span>|<span data-ttu-id="bee47-117">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="bee47-117">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="bee47-118">v10_0</span><span class="sxs-lookup"><span data-stu-id="bee47-118">v10_0</span></span>|<span data-ttu-id="bee47-119">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bee47-119">Boolean</span></span>|<span data-ttu-id="bee47-120">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="bee47-120">Windows version 10.0 or later.</span></span>|
|<span data-ttu-id="bee47-121">v10_1607</span><span class="sxs-lookup"><span data-stu-id="bee47-121">v10_1607</span></span>|<span data-ttu-id="bee47-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee47-122">Boolean</span></span>|<span data-ttu-id="bee47-123">Windows 10 1607 以降です。</span><span class="sxs-lookup"><span data-stu-id="bee47-123">Windows 10 1607 or later.</span></span>|
|<span data-ttu-id="bee47-124">v10_1703</span><span class="sxs-lookup"><span data-stu-id="bee47-124">v10_1703</span></span>|<span data-ttu-id="bee47-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee47-125">Boolean</span></span>|<span data-ttu-id="bee47-126">10 1703 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="bee47-126">Windows 10 1703 or later.</span></span>|
|<span data-ttu-id="bee47-127">v10_1709</span><span class="sxs-lookup"><span data-stu-id="bee47-127">v10_1709</span></span>|<span data-ttu-id="bee47-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee47-128">Boolean</span></span>|<span data-ttu-id="bee47-129">10 1709 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="bee47-129">Windows 10 1709 or later.</span></span>|
|<span data-ttu-id="bee47-130">v10_1803</span><span class="sxs-lookup"><span data-stu-id="bee47-130">v10_1803</span></span>|<span data-ttu-id="bee47-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="bee47-131">Boolean</span></span>|<span data-ttu-id="bee47-132">10 1803 の Windows またはそれ以降です。</span><span class="sxs-lookup"><span data-stu-id="bee47-132">Windows 10 1803 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bee47-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bee47-133">Relationships</span></span>
<span data-ttu-id="bee47-134">なし</span><span class="sxs-lookup"><span data-stu-id="bee47-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bee47-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bee47-135">JSON Representation</span></span>
<span data-ttu-id="bee47-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bee47-136">Here is a JSON representation of the resource.</span></span>
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




