---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553051"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="e57bb-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e57bb-103">excludedApps resource type</span></span>

> <span data-ttu-id="e57bb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e57bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e57bb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e57bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e57bb-106">除外された Office365 アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e57bb-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="e57bb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e57bb-107">Properties</span></span>
|<span data-ttu-id="e57bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e57bb-108">Property</span></span>|<span data-ttu-id="e57bb-109">型</span><span class="sxs-lookup"><span data-stu-id="e57bb-109">Type</span></span>|<span data-ttu-id="e57bb-110">説明</span><span class="sxs-lookup"><span data-stu-id="e57bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e57bb-111">接続</span><span class="sxs-lookup"><span data-stu-id="e57bb-111">access</span></span>|<span data-ttu-id="e57bb-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-112">Boolean</span></span>|<span data-ttu-id="e57bb-113">MS Office へのアクセスを除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-114">シート</span><span class="sxs-lookup"><span data-stu-id="e57bb-114">excel</span></span>|<span data-ttu-id="e57bb-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-115">Boolean</span></span>|<span data-ttu-id="e57bb-116">MS Office Excel を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e57bb-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-117">スペース</span><span class="sxs-lookup"><span data-stu-id="e57bb-117">groove</span></span>|<span data-ttu-id="e57bb-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-118">Boolean</span></span>|<span data-ttu-id="e57bb-119">MS Office OneDrive for business-Groove を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-120">もと</span><span class="sxs-lookup"><span data-stu-id="e57bb-120">infoPath</span></span>|<span data-ttu-id="e57bb-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-121">Boolean</span></span>|<span data-ttu-id="e57bb-122">MS Office InfoPath を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-123">lync</span><span class="sxs-lookup"><span data-stu-id="e57bb-123">lync</span></span>|<span data-ttu-id="e57bb-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-124">Boolean</span></span>|<span data-ttu-id="e57bb-125">MS Office Skype for business-Lync を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-126">スペース</span><span class="sxs-lookup"><span data-stu-id="e57bb-126">oneDrive</span></span>|<span data-ttu-id="e57bb-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-127">Boolean</span></span>|<span data-ttu-id="e57bb-128">MS Office OneDrive を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-129">ノート</span><span class="sxs-lookup"><span data-stu-id="e57bb-129">oneNote</span></span>|<span data-ttu-id="e57bb-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-130">Boolean</span></span>|<span data-ttu-id="e57bb-131">MS Office OneNote を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-132">outlook</span><span class="sxs-lookup"><span data-stu-id="e57bb-132">outlook</span></span>|<span data-ttu-id="e57bb-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-133">Boolean</span></span>|<span data-ttu-id="e57bb-134">MS Office Outlook を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-135">しまう</span><span class="sxs-lookup"><span data-stu-id="e57bb-135">powerPoint</span></span>|<span data-ttu-id="e57bb-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-136">Boolean</span></span>|<span data-ttu-id="e57bb-137">microsoft Office PowerPoint を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e57bb-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-138">publisher</span><span class="sxs-lookup"><span data-stu-id="e57bb-138">publisher</span></span>|<span data-ttu-id="e57bb-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-139">Boolean</span></span>|<span data-ttu-id="e57bb-140">MS Office Publisher を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-141">sharepointdesigner</span><span class="sxs-lookup"><span data-stu-id="e57bb-141">sharePointDesigner</span></span>|<span data-ttu-id="e57bb-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-142">Boolean</span></span>|<span data-ttu-id="e57bb-143">MS Office sharepointdesigner を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e57bb-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-144">teams</span><span class="sxs-lookup"><span data-stu-id="e57bb-144">teams</span></span>|<span data-ttu-id="e57bb-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-145">Boolean</span></span>|<span data-ttu-id="e57bb-146">MS Office Teams を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-147">visio</span><span class="sxs-lookup"><span data-stu-id="e57bb-147">visio</span></span>|<span data-ttu-id="e57bb-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-148">Boolean</span></span>|<span data-ttu-id="e57bb-149">MS Office Visio を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="e57bb-150">段落</span><span class="sxs-lookup"><span data-stu-id="e57bb-150">word</span></span>|<span data-ttu-id="e57bb-151">ブール値</span><span class="sxs-lookup"><span data-stu-id="e57bb-151">Boolean</span></span>|<span data-ttu-id="e57bb-152">MS Office Word を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e57bb-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e57bb-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e57bb-153">Relationships</span></span>
<span data-ttu-id="e57bb-154">なし</span><span class="sxs-lookup"><span data-stu-id="e57bb-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e57bb-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e57bb-155">JSON Representation</span></span>
<span data-ttu-id="e57bb-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e57bb-156">Here is a JSON representation of the resource.</span></span>
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





