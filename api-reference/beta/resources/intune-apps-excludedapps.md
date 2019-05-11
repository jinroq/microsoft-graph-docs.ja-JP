---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37abd83b34fde565aa78e62454c4ce7d47ea192a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950411"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="bc48e-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc48e-103">excludedApps resource type</span></span>

> <span data-ttu-id="bc48e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc48e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc48e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc48e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc48e-106">除外された Office365 アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc48e-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="bc48e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc48e-107">Properties</span></span>
|<span data-ttu-id="bc48e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc48e-108">Property</span></span>|<span data-ttu-id="bc48e-109">型</span><span class="sxs-lookup"><span data-stu-id="bc48e-109">Type</span></span>|<span data-ttu-id="bc48e-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc48e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc48e-111">接続</span><span class="sxs-lookup"><span data-stu-id="bc48e-111">access</span></span>|<span data-ttu-id="bc48e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-112">Boolean</span></span>|<span data-ttu-id="bc48e-113">MS Office へのアクセスを除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-114">シート</span><span class="sxs-lookup"><span data-stu-id="bc48e-114">excel</span></span>|<span data-ttu-id="bc48e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-115">Boolean</span></span>|<span data-ttu-id="bc48e-116">MS Office Excel を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc48e-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-117">スペース</span><span class="sxs-lookup"><span data-stu-id="bc48e-117">groove</span></span>|<span data-ttu-id="bc48e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-118">Boolean</span></span>|<span data-ttu-id="bc48e-119">MS Office OneDrive for Business-Groove を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-120">もと</span><span class="sxs-lookup"><span data-stu-id="bc48e-120">infoPath</span></span>|<span data-ttu-id="bc48e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-121">Boolean</span></span>|<span data-ttu-id="bc48e-122">MS Office InfoPath を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-123">lync</span><span class="sxs-lookup"><span data-stu-id="bc48e-123">lync</span></span>|<span data-ttu-id="bc48e-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-124">Boolean</span></span>|<span data-ttu-id="bc48e-125">MS Office Skype for Business-Lync を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-126">スペース</span><span class="sxs-lookup"><span data-stu-id="bc48e-126">oneDrive</span></span>|<span data-ttu-id="bc48e-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-127">Boolean</span></span>|<span data-ttu-id="bc48e-128">MS Office OneDrive を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-129">ノート</span><span class="sxs-lookup"><span data-stu-id="bc48e-129">oneNote</span></span>|<span data-ttu-id="bc48e-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-130">Boolean</span></span>|<span data-ttu-id="bc48e-131">MS Office OneNote を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-132">outlook</span><span class="sxs-lookup"><span data-stu-id="bc48e-132">outlook</span></span>|<span data-ttu-id="bc48e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-133">Boolean</span></span>|<span data-ttu-id="bc48e-134">MS Office Outlook を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-135">しまう</span><span class="sxs-lookup"><span data-stu-id="bc48e-135">powerPoint</span></span>|<span data-ttu-id="bc48e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-136">Boolean</span></span>|<span data-ttu-id="bc48e-137">MICROSOFT Office PowerPoint を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc48e-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-138">publisher</span><span class="sxs-lookup"><span data-stu-id="bc48e-138">publisher</span></span>|<span data-ttu-id="bc48e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-139">Boolean</span></span>|<span data-ttu-id="bc48e-140">MS Office Publisher を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="bc48e-141">sharePointDesigner</span></span>|<span data-ttu-id="bc48e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-142">Boolean</span></span>|<span data-ttu-id="bc48e-143">MS Office SharePointDesigner を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc48e-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-144">teams</span><span class="sxs-lookup"><span data-stu-id="bc48e-144">teams</span></span>|<span data-ttu-id="bc48e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-145">Boolean</span></span>|<span data-ttu-id="bc48e-146">MS Office Teams を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-147">visio</span><span class="sxs-lookup"><span data-stu-id="bc48e-147">visio</span></span>|<span data-ttu-id="bc48e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-148">Boolean</span></span>|<span data-ttu-id="bc48e-149">MS Office Visio を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="bc48e-150">段落</span><span class="sxs-lookup"><span data-stu-id="bc48e-150">word</span></span>|<span data-ttu-id="bc48e-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc48e-151">Boolean</span></span>|<span data-ttu-id="bc48e-152">MS Office Word を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bc48e-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc48e-153">関係</span><span class="sxs-lookup"><span data-stu-id="bc48e-153">Relationships</span></span>
<span data-ttu-id="bc48e-154">なし</span><span class="sxs-lookup"><span data-stu-id="bc48e-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc48e-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc48e-155">JSON Representation</span></span>
<span data-ttu-id="bc48e-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc48e-156">Here is a JSON representation of the resource.</span></span>
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
  "teams": true,
  "visio": true,
  "word": true
}
```




