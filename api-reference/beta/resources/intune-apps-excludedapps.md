---
title: excludedApps リソースの種類
description: Office365 アプリケーションの除外プロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2ec66c83c13088fb289e271e604154195902ca5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821883"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="b7455-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7455-103">excludedApps resource type</span></span>

> <span data-ttu-id="b7455-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7455-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7455-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7455-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7455-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7455-107">Office365 アプリケーションの除外プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7455-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="b7455-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7455-108">Properties</span></span>
|<span data-ttu-id="b7455-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7455-109">Property</span></span>|<span data-ttu-id="b7455-110">種類</span><span class="sxs-lookup"><span data-stu-id="b7455-110">Type</span></span>|<span data-ttu-id="b7455-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7455-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7455-112">アクセス</span><span class="sxs-lookup"><span data-stu-id="b7455-112">access</span></span>|<span data-ttu-id="b7455-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-113">Boolean</span></span>|<span data-ttu-id="b7455-114">値かの MS Office のアクセスを除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-115">excel</span><span class="sxs-lookup"><span data-stu-id="b7455-115">excel</span></span>|<span data-ttu-id="b7455-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-116">Boolean</span></span>|<span data-ttu-id="b7455-117">値かの MS Office Excel を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-118">溝</span><span class="sxs-lookup"><span data-stu-id="b7455-118">groove</span></span>|<span data-ttu-id="b7455-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-119">Boolean</span></span>|<span data-ttu-id="b7455-120">値か、ビジネスの Groove の MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="b7455-121">infoPath</span></span>|<span data-ttu-id="b7455-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-122">Boolean</span></span>|<span data-ttu-id="b7455-123">値かの MS Office InfoPath を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-124">lync</span><span class="sxs-lookup"><span data-stu-id="b7455-124">lync</span></span>|<span data-ttu-id="b7455-125">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-125">Boolean</span></span>|<span data-ttu-id="b7455-126">値か、ビジネス - Lync の MS Office の Skype を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="b7455-127">oneDrive</span></span>|<span data-ttu-id="b7455-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-128">Boolean</span></span>|<span data-ttu-id="b7455-129">値かの MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="b7455-130">oneNote</span></span>|<span data-ttu-id="b7455-131">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-131">Boolean</span></span>|<span data-ttu-id="b7455-132">値かの MS Office OneNote を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-133">outlook</span><span class="sxs-lookup"><span data-stu-id="b7455-133">outlook</span></span>|<span data-ttu-id="b7455-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-134">Boolean</span></span>|<span data-ttu-id="b7455-135">値かの MS Office Outlook を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="b7455-136">powerPoint</span></span>|<span data-ttu-id="b7455-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-137">Boolean</span></span>|<span data-ttu-id="b7455-138">値かの MS Office PowerPoint を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-139">publisher</span><span class="sxs-lookup"><span data-stu-id="b7455-139">publisher</span></span>|<span data-ttu-id="b7455-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-140">Boolean</span></span>|<span data-ttu-id="b7455-141">値かの MS Office の発行元を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="b7455-142">sharePointDesigner</span></span>|<span data-ttu-id="b7455-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-143">Boolean</span></span>|<span data-ttu-id="b7455-144">値かの MS Office の SharePointDesigner を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-145">visio</span><span class="sxs-lookup"><span data-stu-id="b7455-145">visio</span></span>|<span data-ttu-id="b7455-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-146">Boolean</span></span>|<span data-ttu-id="b7455-147">値かの MS Office Visio を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="b7455-148">単語</span><span class="sxs-lookup"><span data-stu-id="b7455-148">word</span></span>|<span data-ttu-id="b7455-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7455-149">Boolean</span></span>|<span data-ttu-id="b7455-150">値かの MS Office の Word を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7455-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7455-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7455-151">Relationships</span></span>
<span data-ttu-id="b7455-152">なし</span><span class="sxs-lookup"><span data-stu-id="b7455-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7455-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7455-153">JSON Representation</span></span>
<span data-ttu-id="b7455-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7455-154">Here is a JSON representation of the resource.</span></span>
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





