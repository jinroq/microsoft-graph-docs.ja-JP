---
title: devicePlatformType 列挙型
description: プラットフォーム ・ タイプをサポートします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50fbe24b39d3edaa5b6b5c5487aea42f63854eb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974365"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="c1e4a-103">devicePlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c1e4a-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="c1e4a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1e4a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1e4a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1e4a-107">プラットフォーム ・ タイプをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-107">Supported platform types.</span></span>
## <a name="members"></a><span data-ttu-id="c1e4a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c1e4a-108">Members</span></span>
|<span data-ttu-id="c1e4a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c1e4a-109">Member</span></span>|<span data-ttu-id="c1e4a-110">値</span><span class="sxs-lookup"><span data-stu-id="c1e4a-110">Value</span></span>|<span data-ttu-id="c1e4a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1e4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1e4a-112">android</span><span class="sxs-lookup"><span data-stu-id="c1e4a-112">android</span></span>|<span data-ttu-id="c1e4a-113">0</span><span class="sxs-lookup"><span data-stu-id="c1e4a-113">0</span></span>|<span data-ttu-id="c1e4a-114">Android。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-114">Android.</span></span>|
|<span data-ttu-id="c1e4a-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="c1e4a-115">androidForWork</span></span>|<span data-ttu-id="c1e4a-116">1</span><span class="sxs-lookup"><span data-stu-id="c1e4a-116">1</span></span>|<span data-ttu-id="c1e4a-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-117">AndroidForWork.</span></span>|
|<span data-ttu-id="c1e4a-118">iOS</span><span class="sxs-lookup"><span data-stu-id="c1e4a-118">iOS</span></span>|<span data-ttu-id="c1e4a-119">2</span><span class="sxs-lookup"><span data-stu-id="c1e4a-119">2</span></span>|<span data-ttu-id="c1e4a-120">iOS です。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-120">iOS.</span></span>|
|<span data-ttu-id="c1e4a-121">macOS</span><span class="sxs-lookup"><span data-stu-id="c1e4a-121">macOS</span></span>|<span data-ttu-id="c1e4a-122">3</span><span class="sxs-lookup"><span data-stu-id="c1e4a-122">3</span></span>|<span data-ttu-id="c1e4a-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-123">MacOS.</span></span>|
|<span data-ttu-id="c1e4a-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c1e4a-124">windowsPhone81</span></span>|<span data-ttu-id="c1e4a-125">4</span><span class="sxs-lookup"><span data-stu-id="c1e4a-125">4</span></span>|<span data-ttu-id="c1e4a-126">WindowsPhone 8.1 です。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="c1e4a-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="c1e4a-127">windows81AndLater</span></span>|<span data-ttu-id="c1e4a-128">5</span><span class="sxs-lookup"><span data-stu-id="c1e4a-128">5</span></span>|<span data-ttu-id="c1e4a-129">およびそれ以降の Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="c1e4a-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="c1e4a-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="c1e4a-130">windows10AndLater</span></span>|<span data-ttu-id="c1e4a-131">6</span><span class="sxs-lookup"><span data-stu-id="c1e4a-131">6</span></span>|<span data-ttu-id="c1e4a-132">Windows 10 以降です。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="c1e4a-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="c1e4a-133">androidWorkProfile</span></span>|<span data-ttu-id="c1e4a-134">7</span><span class="sxs-lookup"><span data-stu-id="c1e4a-134">7</span></span>|<span data-ttu-id="c1e4a-135">Android 作業プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="c1e4a-135">Android Work Profile.</span></span>|





