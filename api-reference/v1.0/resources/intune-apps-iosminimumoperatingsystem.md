---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254570"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="1af5f-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1af5f-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="1af5f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1af5f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af5f-105">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1af5f-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="1af5f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1af5f-106">Properties</span></span>
|<span data-ttu-id="1af5f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1af5f-107">Property</span></span>|<span data-ttu-id="1af5f-108">型</span><span class="sxs-lookup"><span data-stu-id="1af5f-108">Type</span></span>|<span data-ttu-id="1af5f-109">説明</span><span class="sxs-lookup"><span data-stu-id="1af5f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af5f-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="1af5f-110">v8_0</span></span>|<span data-ttu-id="1af5f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af5f-111">Boolean</span></span>|<span data-ttu-id="1af5f-112">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1af5f-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="1af5f-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="1af5f-113">v9_0</span></span>|<span data-ttu-id="1af5f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af5f-114">Boolean</span></span>|<span data-ttu-id="1af5f-115">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1af5f-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="1af5f-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="1af5f-116">v10_0</span></span>|<span data-ttu-id="1af5f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af5f-117">Boolean</span></span>|<span data-ttu-id="1af5f-118">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1af5f-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="1af5f-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="1af5f-119">v11_0</span></span>|<span data-ttu-id="1af5f-120">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1af5f-120">Boolean</span></span>|<span data-ttu-id="1af5f-121">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1af5f-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="1af5f-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="1af5f-122">v12_0</span></span>|<span data-ttu-id="1af5f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af5f-123">Boolean</span></span>|<span data-ttu-id="1af5f-124">バージョン12.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1af5f-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af5f-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1af5f-125">Relationships</span></span>
<span data-ttu-id="1af5f-126">なし</span><span class="sxs-lookup"><span data-stu-id="1af5f-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af5f-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1af5f-127">JSON Representation</span></span>
<span data-ttu-id="1af5f-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1af5f-128">Here is a JSON representation of the resource.</span></span>
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



