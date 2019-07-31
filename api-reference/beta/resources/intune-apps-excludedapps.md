---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6bd731107571e8959418466541e2947d40d16072
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006011"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="7e63c-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e63c-103">excludedApps resource type</span></span>

> <span data-ttu-id="7e63c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e63c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e63c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e63c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e63c-106">除外された Office365 アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e63c-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="7e63c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e63c-107">Properties</span></span>
|<span data-ttu-id="7e63c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e63c-108">Property</span></span>|<span data-ttu-id="7e63c-109">型</span><span class="sxs-lookup"><span data-stu-id="7e63c-109">Type</span></span>|<span data-ttu-id="7e63c-110">説明</span><span class="sxs-lookup"><span data-stu-id="7e63c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e63c-111">接続</span><span class="sxs-lookup"><span data-stu-id="7e63c-111">access</span></span>|<span data-ttu-id="7e63c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-112">Boolean</span></span>|<span data-ttu-id="7e63c-113">MS Office へのアクセスを除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-114">シート</span><span class="sxs-lookup"><span data-stu-id="7e63c-114">excel</span></span>|<span data-ttu-id="7e63c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-115">Boolean</span></span>|<span data-ttu-id="7e63c-116">MS Office Excel を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e63c-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-117">スペース</span><span class="sxs-lookup"><span data-stu-id="7e63c-117">groove</span></span>|<span data-ttu-id="7e63c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-118">Boolean</span></span>|<span data-ttu-id="7e63c-119">MS Office OneDrive for Business-Groove を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-120">もと</span><span class="sxs-lookup"><span data-stu-id="7e63c-120">infoPath</span></span>|<span data-ttu-id="7e63c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-121">Boolean</span></span>|<span data-ttu-id="7e63c-122">MS Office InfoPath を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-123">lync</span><span class="sxs-lookup"><span data-stu-id="7e63c-123">lync</span></span>|<span data-ttu-id="7e63c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-124">Boolean</span></span>|<span data-ttu-id="7e63c-125">MS Office Skype for Business-Lync を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-126">スペース</span><span class="sxs-lookup"><span data-stu-id="7e63c-126">oneDrive</span></span>|<span data-ttu-id="7e63c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-127">Boolean</span></span>|<span data-ttu-id="7e63c-128">MS Office OneDrive を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-129">ノート</span><span class="sxs-lookup"><span data-stu-id="7e63c-129">oneNote</span></span>|<span data-ttu-id="7e63c-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-130">Boolean</span></span>|<span data-ttu-id="7e63c-131">MS Office OneNote を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-132">outlook</span><span class="sxs-lookup"><span data-stu-id="7e63c-132">outlook</span></span>|<span data-ttu-id="7e63c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-133">Boolean</span></span>|<span data-ttu-id="7e63c-134">MS Office Outlook を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-135">しまう</span><span class="sxs-lookup"><span data-stu-id="7e63c-135">powerPoint</span></span>|<span data-ttu-id="7e63c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-136">Boolean</span></span>|<span data-ttu-id="7e63c-137">MICROSOFT Office PowerPoint を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e63c-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-138">publisher</span><span class="sxs-lookup"><span data-stu-id="7e63c-138">publisher</span></span>|<span data-ttu-id="7e63c-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-139">Boolean</span></span>|<span data-ttu-id="7e63c-140">MS Office Publisher を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="7e63c-141">sharePointDesigner</span></span>|<span data-ttu-id="7e63c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-142">Boolean</span></span>|<span data-ttu-id="7e63c-143">MS Office SharePointDesigner を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e63c-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-144">teams</span><span class="sxs-lookup"><span data-stu-id="7e63c-144">teams</span></span>|<span data-ttu-id="7e63c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-145">Boolean</span></span>|<span data-ttu-id="7e63c-146">MS Office Teams を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-147">visio</span><span class="sxs-lookup"><span data-stu-id="7e63c-147">visio</span></span>|<span data-ttu-id="7e63c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-148">Boolean</span></span>|<span data-ttu-id="7e63c-149">MS Office Visio を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="7e63c-150">段落</span><span class="sxs-lookup"><span data-stu-id="7e63c-150">word</span></span>|<span data-ttu-id="7e63c-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e63c-151">Boolean</span></span>|<span data-ttu-id="7e63c-152">MS Office Word を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7e63c-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e63c-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e63c-153">Relationships</span></span>
<span data-ttu-id="7e63c-154">なし</span><span class="sxs-lookup"><span data-stu-id="7e63c-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e63c-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e63c-155">JSON Representation</span></span>
<span data-ttu-id="7e63c-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e63c-156">Here is a JSON representation of the resource.</span></span>
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





