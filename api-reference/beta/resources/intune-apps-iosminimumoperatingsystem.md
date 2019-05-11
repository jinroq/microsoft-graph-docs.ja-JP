---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 998c7a1214fb05596d4f851f7883be514d368e88
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950439"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="eb04a-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb04a-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="eb04a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb04a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb04a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb04a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb04a-106">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="eb04a-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="eb04a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb04a-107">Properties</span></span>
|<span data-ttu-id="eb04a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb04a-108">Property</span></span>|<span data-ttu-id="eb04a-109">型</span><span class="sxs-lookup"><span data-stu-id="eb04a-109">Type</span></span>|<span data-ttu-id="eb04a-110">説明</span><span class="sxs-lookup"><span data-stu-id="eb04a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb04a-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="eb04a-111">v8_0</span></span>|<span data-ttu-id="eb04a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb04a-112">Boolean</span></span>|<span data-ttu-id="eb04a-113">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="eb04a-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="eb04a-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="eb04a-114">v9_0</span></span>|<span data-ttu-id="eb04a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb04a-115">Boolean</span></span>|<span data-ttu-id="eb04a-116">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="eb04a-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="eb04a-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="eb04a-117">v10_0</span></span>|<span data-ttu-id="eb04a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb04a-118">Boolean</span></span>|<span data-ttu-id="eb04a-119">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="eb04a-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="eb04a-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="eb04a-120">v11_0</span></span>|<span data-ttu-id="eb04a-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="eb04a-121">Boolean</span></span>|<span data-ttu-id="eb04a-122">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="eb04a-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="eb04a-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="eb04a-123">v12_0</span></span>|<span data-ttu-id="eb04a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb04a-124">Boolean</span></span>|<span data-ttu-id="eb04a-125">バージョン12.0 以降。</span><span class="sxs-lookup"><span data-stu-id="eb04a-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb04a-126">関係</span><span class="sxs-lookup"><span data-stu-id="eb04a-126">Relationships</span></span>
<span data-ttu-id="eb04a-127">なし</span><span class="sxs-lookup"><span data-stu-id="eb04a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb04a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb04a-128">JSON Representation</span></span>
<span data-ttu-id="eb04a-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb04a-129">Here is a JSON representation of the resource.</span></span>
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




