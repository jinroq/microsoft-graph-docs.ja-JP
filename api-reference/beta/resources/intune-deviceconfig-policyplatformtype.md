---
title: policyPlatformType 列挙型
description: ポリシーには、プラットフォームの種類を Suppoorted。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0eef91313b308824b4e2395efb8e7aa95cf0c1ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919309"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="5a1fd-103">policyPlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5a1fd-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="5a1fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a1fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a1fd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a1fd-107">ポリシーには、プラットフォームの種類を Suppoorted。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-107">Suppoorted platform types for policies.</span></span>
## <a name="members"></a><span data-ttu-id="5a1fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a1fd-108">Members</span></span>
|<span data-ttu-id="5a1fd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a1fd-109">Member</span></span>|<span data-ttu-id="5a1fd-110">値</span><span class="sxs-lookup"><span data-stu-id="5a1fd-110">Value</span></span>|<span data-ttu-id="5a1fd-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a1fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1fd-112">android</span><span class="sxs-lookup"><span data-stu-id="5a1fd-112">android</span></span>|<span data-ttu-id="5a1fd-113">0</span><span class="sxs-lookup"><span data-stu-id="5a1fd-113">0</span></span>|<span data-ttu-id="5a1fd-114">Android。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-114">Android.</span></span>|
|<span data-ttu-id="5a1fd-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="5a1fd-115">androidForWork</span></span>|<span data-ttu-id="5a1fd-116">1</span><span class="sxs-lookup"><span data-stu-id="5a1fd-116">1</span></span>|<span data-ttu-id="5a1fd-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-117">AndroidForWork.</span></span>|
|<span data-ttu-id="5a1fd-118">iOS</span><span class="sxs-lookup"><span data-stu-id="5a1fd-118">iOS</span></span>|<span data-ttu-id="5a1fd-119">2</span><span class="sxs-lookup"><span data-stu-id="5a1fd-119">2</span></span>|<span data-ttu-id="5a1fd-120">iOS です。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-120">iOS.</span></span>|
|<span data-ttu-id="5a1fd-121">macOS</span><span class="sxs-lookup"><span data-stu-id="5a1fd-121">macOS</span></span>|<span data-ttu-id="5a1fd-122">3</span><span class="sxs-lookup"><span data-stu-id="5a1fd-122">3</span></span>|<span data-ttu-id="5a1fd-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-123">MacOS.</span></span>|
|<span data-ttu-id="5a1fd-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="5a1fd-124">windowsPhone81</span></span>|<span data-ttu-id="5a1fd-125">4</span><span class="sxs-lookup"><span data-stu-id="5a1fd-125">4</span></span>|<span data-ttu-id="5a1fd-126">WindowsPhone 8.1 です。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="5a1fd-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="5a1fd-127">windows81AndLater</span></span>|<span data-ttu-id="5a1fd-128">5</span><span class="sxs-lookup"><span data-stu-id="5a1fd-128">5</span></span>|<span data-ttu-id="5a1fd-129">およびそれ以降の Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="5a1fd-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="5a1fd-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="5a1fd-130">windows10AndLater</span></span>|<span data-ttu-id="5a1fd-131">6</span><span class="sxs-lookup"><span data-stu-id="5a1fd-131">6</span></span>|<span data-ttu-id="5a1fd-132">Windows 10 以降です。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="5a1fd-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="5a1fd-133">androidWorkProfile</span></span>|<span data-ttu-id="5a1fd-134">7</span><span class="sxs-lookup"><span data-stu-id="5a1fd-134">7</span></span>|<span data-ttu-id="5a1fd-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="5a1fd-136">all</span><span class="sxs-lookup"><span data-stu-id="5a1fd-136">all</span></span>|<span data-ttu-id="5a1fd-137">100</span><span class="sxs-lookup"><span data-stu-id="5a1fd-137">100</span></span>|<span data-ttu-id="5a1fd-138">すべてのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="5a1fd-138">All platforms.</span></span>|





