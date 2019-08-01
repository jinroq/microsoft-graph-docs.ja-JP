---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da56780e66e88baaa074c3106997e3b4a3cc3b64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032348"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="0e264-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e264-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="0e264-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e264-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e264-105">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0e264-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="0e264-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e264-106">Properties</span></span>
|<span data-ttu-id="0e264-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e264-107">Property</span></span>|<span data-ttu-id="0e264-108">型</span><span class="sxs-lookup"><span data-stu-id="0e264-108">Type</span></span>|<span data-ttu-id="0e264-109">説明</span><span class="sxs-lookup"><span data-stu-id="0e264-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e264-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="0e264-110">v8_0</span></span>|<span data-ttu-id="0e264-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e264-111">Boolean</span></span>|<span data-ttu-id="0e264-112">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="0e264-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="0e264-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="0e264-113">v9_0</span></span>|<span data-ttu-id="0e264-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e264-114">Boolean</span></span>|<span data-ttu-id="0e264-115">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="0e264-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="0e264-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="0e264-116">v10_0</span></span>|<span data-ttu-id="0e264-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e264-117">Boolean</span></span>|<span data-ttu-id="0e264-118">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="0e264-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="0e264-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="0e264-119">v11_0</span></span>|<span data-ttu-id="0e264-120">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0e264-120">Boolean</span></span>|<span data-ttu-id="0e264-121">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="0e264-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="0e264-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="0e264-122">v12_0</span></span>|<span data-ttu-id="0e264-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e264-123">Boolean</span></span>|<span data-ttu-id="0e264-124">バージョン12.0 以降。</span><span class="sxs-lookup"><span data-stu-id="0e264-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e264-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e264-125">Relationships</span></span>
<span data-ttu-id="0e264-126">なし</span><span class="sxs-lookup"><span data-stu-id="0e264-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e264-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e264-127">JSON Representation</span></span>
<span data-ttu-id="0e264-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e264-128">Here is a JSON representation of the resource.</span></span>
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



