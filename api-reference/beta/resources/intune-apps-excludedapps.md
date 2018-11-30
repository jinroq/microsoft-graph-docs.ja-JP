---
title: excludedApps リソースの種類
description: Office365 アプリケーションの除外プロパティが含まれています。
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068900"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="3b85e-103">excludedApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b85e-103">excludedApps resource type</span></span>

> <span data-ttu-id="3b85e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b85e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b85e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b85e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b85e-107">Office365 アプリケーションの除外プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3b85e-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="3b85e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b85e-108">Properties</span></span>
|<span data-ttu-id="3b85e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b85e-109">Property</span></span>|<span data-ttu-id="3b85e-110">型</span><span class="sxs-lookup"><span data-stu-id="3b85e-110">Type</span></span>|<span data-ttu-id="3b85e-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b85e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b85e-112">アクセス</span><span class="sxs-lookup"><span data-stu-id="3b85e-112">access</span></span>|<span data-ttu-id="3b85e-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-113">Boolean</span></span>|<span data-ttu-id="3b85e-114">値かの MS Office のアクセスを除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-115">excel</span><span class="sxs-lookup"><span data-stu-id="3b85e-115">excel</span></span>|<span data-ttu-id="3b85e-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-116">Boolean</span></span>|<span data-ttu-id="3b85e-117">値かの MS Office Excel を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-118">溝</span><span class="sxs-lookup"><span data-stu-id="3b85e-118">groove</span></span>|<span data-ttu-id="3b85e-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-119">Boolean</span></span>|<span data-ttu-id="3b85e-120">値か、ビジネスの Groove の MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="3b85e-121">infoPath</span></span>|<span data-ttu-id="3b85e-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-122">Boolean</span></span>|<span data-ttu-id="3b85e-123">値かの MS Office InfoPath を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-124">lync</span><span class="sxs-lookup"><span data-stu-id="3b85e-124">lync</span></span>|<span data-ttu-id="3b85e-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-125">Boolean</span></span>|<span data-ttu-id="3b85e-126">値か、ビジネス - Lync の MS Office の Skype を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="3b85e-127">oneDrive</span></span>|<span data-ttu-id="3b85e-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-128">Boolean</span></span>|<span data-ttu-id="3b85e-129">値かの MS Office の OneDrive を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="3b85e-130">oneNote</span></span>|<span data-ttu-id="3b85e-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-131">Boolean</span></span>|<span data-ttu-id="3b85e-132">値かの MS Office OneNote を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-133">outlook</span><span class="sxs-lookup"><span data-stu-id="3b85e-133">outlook</span></span>|<span data-ttu-id="3b85e-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-134">Boolean</span></span>|<span data-ttu-id="3b85e-135">値かの MS Office Outlook を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="3b85e-136">powerPoint</span></span>|<span data-ttu-id="3b85e-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-137">Boolean</span></span>|<span data-ttu-id="3b85e-138">値かの MS Office PowerPoint を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-139">publisher</span><span class="sxs-lookup"><span data-stu-id="3b85e-139">publisher</span></span>|<span data-ttu-id="3b85e-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-140">Boolean</span></span>|<span data-ttu-id="3b85e-141">値かの MS Office の発行元を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="3b85e-142">sharePointDesigner</span></span>|<span data-ttu-id="3b85e-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-143">Boolean</span></span>|<span data-ttu-id="3b85e-144">値かの MS Office の SharePointDesigner を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-145">visio</span><span class="sxs-lookup"><span data-stu-id="3b85e-145">visio</span></span>|<span data-ttu-id="3b85e-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-146">Boolean</span></span>|<span data-ttu-id="3b85e-147">値かの MS Office Visio を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="3b85e-148">単語</span><span class="sxs-lookup"><span data-stu-id="3b85e-148">word</span></span>|<span data-ttu-id="3b85e-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="3b85e-149">Boolean</span></span>|<span data-ttu-id="3b85e-150">値かの MS Office の Word を除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b85e-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b85e-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b85e-151">Relationships</span></span>
<span data-ttu-id="3b85e-152">なし</span><span class="sxs-lookup"><span data-stu-id="3b85e-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b85e-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b85e-153">JSON Representation</span></span>
<span data-ttu-id="3b85e-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b85e-154">Here is a JSON representation of the resource.</span></span>
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





