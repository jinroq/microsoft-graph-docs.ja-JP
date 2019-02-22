---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ba3e53a26ff71dde2d5a95fde811e42ba2ccb99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154027"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="92a9e-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92a9e-103">excludedApps resource type</span></span>

> <span data-ttu-id="92a9e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92a9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92a9e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92a9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a9e-106">除外された Office365 アプリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92a9e-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="92a9e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92a9e-107">Properties</span></span>
|<span data-ttu-id="92a9e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92a9e-108">Property</span></span>|<span data-ttu-id="92a9e-109">型</span><span class="sxs-lookup"><span data-stu-id="92a9e-109">Type</span></span>|<span data-ttu-id="92a9e-110">説明</span><span class="sxs-lookup"><span data-stu-id="92a9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a9e-111">接続</span><span class="sxs-lookup"><span data-stu-id="92a9e-111">access</span></span>|<span data-ttu-id="92a9e-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-112">Boolean</span></span>|<span data-ttu-id="92a9e-113">MS Office へのアクセスを除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-114">シート</span><span class="sxs-lookup"><span data-stu-id="92a9e-114">excel</span></span>|<span data-ttu-id="92a9e-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-115">Boolean</span></span>|<span data-ttu-id="92a9e-116">MS Office Excel を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="92a9e-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-117">スペース</span><span class="sxs-lookup"><span data-stu-id="92a9e-117">groove</span></span>|<span data-ttu-id="92a9e-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-118">Boolean</span></span>|<span data-ttu-id="92a9e-119">MS Office OneDrive for business-Groove を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-120">もと</span><span class="sxs-lookup"><span data-stu-id="92a9e-120">infoPath</span></span>|<span data-ttu-id="92a9e-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-121">Boolean</span></span>|<span data-ttu-id="92a9e-122">MS Office InfoPath を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-123">lync</span><span class="sxs-lookup"><span data-stu-id="92a9e-123">lync</span></span>|<span data-ttu-id="92a9e-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-124">Boolean</span></span>|<span data-ttu-id="92a9e-125">MS Office Skype for business-Lync を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-126">スペース</span><span class="sxs-lookup"><span data-stu-id="92a9e-126">oneDrive</span></span>|<span data-ttu-id="92a9e-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-127">Boolean</span></span>|<span data-ttu-id="92a9e-128">MS Office OneDrive を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-129">ノート</span><span class="sxs-lookup"><span data-stu-id="92a9e-129">oneNote</span></span>|<span data-ttu-id="92a9e-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-130">Boolean</span></span>|<span data-ttu-id="92a9e-131">MS Office OneNote を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-132">outlook</span><span class="sxs-lookup"><span data-stu-id="92a9e-132">outlook</span></span>|<span data-ttu-id="92a9e-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-133">Boolean</span></span>|<span data-ttu-id="92a9e-134">MS Office Outlook を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-135">しまう</span><span class="sxs-lookup"><span data-stu-id="92a9e-135">powerPoint</span></span>|<span data-ttu-id="92a9e-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-136">Boolean</span></span>|<span data-ttu-id="92a9e-137">microsoft Office PowerPoint を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="92a9e-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-138">publisher</span><span class="sxs-lookup"><span data-stu-id="92a9e-138">publisher</span></span>|<span data-ttu-id="92a9e-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-139">Boolean</span></span>|<span data-ttu-id="92a9e-140">MS Office Publisher を除外する必要があるかどうかの値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-141">sharepointdesigner</span><span class="sxs-lookup"><span data-stu-id="92a9e-141">sharePointDesigner</span></span>|<span data-ttu-id="92a9e-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-142">Boolean</span></span>|<span data-ttu-id="92a9e-143">MS Office sharepointdesigner を除外するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="92a9e-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-144">visio</span><span class="sxs-lookup"><span data-stu-id="92a9e-144">visio</span></span>|<span data-ttu-id="92a9e-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-145">Boolean</span></span>|<span data-ttu-id="92a9e-146">MS Office Visio を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-146">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="92a9e-147">段落</span><span class="sxs-lookup"><span data-stu-id="92a9e-147">word</span></span>|<span data-ttu-id="92a9e-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="92a9e-148">Boolean</span></span>|<span data-ttu-id="92a9e-149">MS Office Word を除外する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="92a9e-149">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92a9e-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92a9e-150">Relationships</span></span>
<span data-ttu-id="92a9e-151">なし</span><span class="sxs-lookup"><span data-stu-id="92a9e-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92a9e-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92a9e-152">JSON Representation</span></span>
<span data-ttu-id="92a9e-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92a9e-153">Here is a JSON representation of the resource.</span></span>
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




