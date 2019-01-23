---
title: excludedApps リソースの種類
description: Office365 アプリケーションの除外プロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395679"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c0a5a-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0a5a-103">excludedApps resource type</span></span>

> <span data-ttu-id="c0a5a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0a5a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0a5a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0a5a-107">Office365 アプリケーションの除外プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="c0a5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0a5a-108">Properties</span></span>
|<span data-ttu-id="c0a5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0a5a-109">Property</span></span>|<span data-ttu-id="c0a5a-110">型</span><span class="sxs-lookup"><span data-stu-id="c0a5a-110">Type</span></span>|<span data-ttu-id="c0a5a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c0a5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0a5a-112">アクセス</span><span class="sxs-lookup"><span data-stu-id="c0a5a-112">access</span></span>|<span data-ttu-id="c0a5a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-113">Boolean</span></span>|<span data-ttu-id="c0a5a-114">値かの MS Office のアクセスを除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-115">excel</span><span class="sxs-lookup"><span data-stu-id="c0a5a-115">excel</span></span>|<span data-ttu-id="c0a5a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-116">Boolean</span></span>|<span data-ttu-id="c0a5a-117">値かの MS Office Excel を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-118">溝</span><span class="sxs-lookup"><span data-stu-id="c0a5a-118">groove</span></span>|<span data-ttu-id="c0a5a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-119">Boolean</span></span>|<span data-ttu-id="c0a5a-120">値か、ビジネスの Groove の MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="c0a5a-121">infoPath</span></span>|<span data-ttu-id="c0a5a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-122">Boolean</span></span>|<span data-ttu-id="c0a5a-123">値かの MS Office InfoPath を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-124">lync</span><span class="sxs-lookup"><span data-stu-id="c0a5a-124">lync</span></span>|<span data-ttu-id="c0a5a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-125">Boolean</span></span>|<span data-ttu-id="c0a5a-126">値か、ビジネス - Lync の MS Office の Skype を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c0a5a-127">oneDrive</span></span>|<span data-ttu-id="c0a5a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-128">Boolean</span></span>|<span data-ttu-id="c0a5a-129">値かの MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="c0a5a-130">oneNote</span></span>|<span data-ttu-id="c0a5a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-131">Boolean</span></span>|<span data-ttu-id="c0a5a-132">値かの MS Office OneNote を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-133">outlook</span><span class="sxs-lookup"><span data-stu-id="c0a5a-133">outlook</span></span>|<span data-ttu-id="c0a5a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-134">Boolean</span></span>|<span data-ttu-id="c0a5a-135">値かの MS Office Outlook を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c0a5a-136">powerPoint</span></span>|<span data-ttu-id="c0a5a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-137">Boolean</span></span>|<span data-ttu-id="c0a5a-138">値かの MS Office PowerPoint を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-139">publisher</span><span class="sxs-lookup"><span data-stu-id="c0a5a-139">publisher</span></span>|<span data-ttu-id="c0a5a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-140">Boolean</span></span>|<span data-ttu-id="c0a5a-141">値かの MS Office の発行元を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="c0a5a-142">sharePointDesigner</span></span>|<span data-ttu-id="c0a5a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-143">Boolean</span></span>|<span data-ttu-id="c0a5a-144">値かの MS Office の SharePointDesigner を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-145">visio</span><span class="sxs-lookup"><span data-stu-id="c0a5a-145">visio</span></span>|<span data-ttu-id="c0a5a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-146">Boolean</span></span>|<span data-ttu-id="c0a5a-147">値かの MS Office Visio を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c0a5a-148">単語</span><span class="sxs-lookup"><span data-stu-id="c0a5a-148">word</span></span>|<span data-ttu-id="c0a5a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a5a-149">Boolean</span></span>|<span data-ttu-id="c0a5a-150">値かの MS Office の Word を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0a5a-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0a5a-151">Relationships</span></span>
<span data-ttu-id="c0a5a-152">なし</span><span class="sxs-lookup"><span data-stu-id="c0a5a-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0a5a-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0a5a-153">JSON Representation</span></span>
<span data-ttu-id="c0a5a-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0a5a-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```




