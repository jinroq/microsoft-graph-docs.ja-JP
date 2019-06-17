---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91418a1a60a87f381dc15c63a60d69e8c264a5c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991248"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c5a80-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5a80-103">excludedApps resource type</span></span>

> <span data-ttu-id="c5a80-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5a80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a80-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5a80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a80-106">除外された Office365 アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5a80-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="c5a80-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a80-107">Properties</span></span>
|<span data-ttu-id="c5a80-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a80-108">Property</span></span>|<span data-ttu-id="c5a80-109">型</span><span class="sxs-lookup"><span data-stu-id="c5a80-109">Type</span></span>|<span data-ttu-id="c5a80-110">説明</span><span class="sxs-lookup"><span data-stu-id="c5a80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a80-111">接続</span><span class="sxs-lookup"><span data-stu-id="c5a80-111">access</span></span>|<span data-ttu-id="c5a80-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-112">Boolean</span></span>|<span data-ttu-id="c5a80-113">MS Office へのアクセスを除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-114">シート</span><span class="sxs-lookup"><span data-stu-id="c5a80-114">excel</span></span>|<span data-ttu-id="c5a80-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-115">Boolean</span></span>|<span data-ttu-id="c5a80-116">MS Office Excel を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5a80-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-117">スペース</span><span class="sxs-lookup"><span data-stu-id="c5a80-117">groove</span></span>|<span data-ttu-id="c5a80-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-118">Boolean</span></span>|<span data-ttu-id="c5a80-119">MS Office OneDrive for Business-Groove を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-120">もと</span><span class="sxs-lookup"><span data-stu-id="c5a80-120">infoPath</span></span>|<span data-ttu-id="c5a80-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-121">Boolean</span></span>|<span data-ttu-id="c5a80-122">MS Office InfoPath を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-123">lync</span><span class="sxs-lookup"><span data-stu-id="c5a80-123">lync</span></span>|<span data-ttu-id="c5a80-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-124">Boolean</span></span>|<span data-ttu-id="c5a80-125">MS Office Skype for Business-Lync を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-126">スペース</span><span class="sxs-lookup"><span data-stu-id="c5a80-126">oneDrive</span></span>|<span data-ttu-id="c5a80-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-127">Boolean</span></span>|<span data-ttu-id="c5a80-128">MS Office OneDrive を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-129">ノート</span><span class="sxs-lookup"><span data-stu-id="c5a80-129">oneNote</span></span>|<span data-ttu-id="c5a80-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-130">Boolean</span></span>|<span data-ttu-id="c5a80-131">MS Office OneNote を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-132">outlook</span><span class="sxs-lookup"><span data-stu-id="c5a80-132">outlook</span></span>|<span data-ttu-id="c5a80-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-133">Boolean</span></span>|<span data-ttu-id="c5a80-134">MS Office Outlook を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-135">しまう</span><span class="sxs-lookup"><span data-stu-id="c5a80-135">powerPoint</span></span>|<span data-ttu-id="c5a80-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-136">Boolean</span></span>|<span data-ttu-id="c5a80-137">MICROSOFT Office PowerPoint を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5a80-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-138">publisher</span><span class="sxs-lookup"><span data-stu-id="c5a80-138">publisher</span></span>|<span data-ttu-id="c5a80-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-139">Boolean</span></span>|<span data-ttu-id="c5a80-140">MS Office Publisher を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="c5a80-141">sharePointDesigner</span></span>|<span data-ttu-id="c5a80-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-142">Boolean</span></span>|<span data-ttu-id="c5a80-143">MS Office SharePointDesigner を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5a80-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-144">teams</span><span class="sxs-lookup"><span data-stu-id="c5a80-144">teams</span></span>|<span data-ttu-id="c5a80-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-145">Boolean</span></span>|<span data-ttu-id="c5a80-146">MS Office Teams を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-147">visio</span><span class="sxs-lookup"><span data-stu-id="c5a80-147">visio</span></span>|<span data-ttu-id="c5a80-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-148">Boolean</span></span>|<span data-ttu-id="c5a80-149">MS Office Visio を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c5a80-150">段落</span><span class="sxs-lookup"><span data-stu-id="c5a80-150">word</span></span>|<span data-ttu-id="c5a80-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a80-151">Boolean</span></span>|<span data-ttu-id="c5a80-152">MS Office Word を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c5a80-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5a80-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5a80-153">Relationships</span></span>
<span data-ttu-id="c5a80-154">なし</span><span class="sxs-lookup"><span data-stu-id="c5a80-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5a80-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5a80-155">JSON Representation</span></span>
<span data-ttu-id="c5a80-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5a80-156">Here is a JSON representation of the resource.</span></span>
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





