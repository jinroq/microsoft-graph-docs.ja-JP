---
title: policyPlatformType 列挙型
description: ポリシーには、プラットフォームの種類を Suppoorted。
author: tfitzmac
ms.openlocfilehash: c36551393be37f2087c64d03a323ff82a5e6e037
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323948"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="f7493-103">policyPlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7493-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="f7493-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7493-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7493-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7493-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7493-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7493-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7493-107">ポリシーには、プラットフォームの種類を Suppoorted。</span><span class="sxs-lookup"><span data-stu-id="f7493-107">Suppoorted platform types for policies.</span></span>
## <a name="members"></a><span data-ttu-id="f7493-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7493-108">Members</span></span>
|<span data-ttu-id="f7493-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7493-109">Member</span></span>|<span data-ttu-id="f7493-110">値</span><span class="sxs-lookup"><span data-stu-id="f7493-110">Value</span></span>|<span data-ttu-id="f7493-111">説明</span><span class="sxs-lookup"><span data-stu-id="f7493-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7493-112">android</span><span class="sxs-lookup"><span data-stu-id="f7493-112">android</span></span>|<span data-ttu-id="f7493-113">0</span><span class="sxs-lookup"><span data-stu-id="f7493-113">0</span></span>|<span data-ttu-id="f7493-114">Android。</span><span class="sxs-lookup"><span data-stu-id="f7493-114">Android.</span></span>|
|<span data-ttu-id="f7493-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="f7493-115">androidForWork</span></span>|<span data-ttu-id="f7493-116">1</span><span class="sxs-lookup"><span data-stu-id="f7493-116">1</span></span>|<span data-ttu-id="f7493-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="f7493-117">AndroidForWork.</span></span>|
|<span data-ttu-id="f7493-118">iOS</span><span class="sxs-lookup"><span data-stu-id="f7493-118">iOS</span></span>|<span data-ttu-id="f7493-119">2</span><span class="sxs-lookup"><span data-stu-id="f7493-119">2</span></span>|<span data-ttu-id="f7493-120">iOS です。</span><span class="sxs-lookup"><span data-stu-id="f7493-120">iOS.</span></span>|
|<span data-ttu-id="f7493-121">macOS</span><span class="sxs-lookup"><span data-stu-id="f7493-121">macOS</span></span>|<span data-ttu-id="f7493-122">3</span><span class="sxs-lookup"><span data-stu-id="f7493-122">3</span></span>|<span data-ttu-id="f7493-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="f7493-123">MacOS.</span></span>|
|<span data-ttu-id="f7493-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="f7493-124">windowsPhone81</span></span>|<span data-ttu-id="f7493-125">4</span><span class="sxs-lookup"><span data-stu-id="f7493-125">4</span></span>|<span data-ttu-id="f7493-126">WindowsPhone 8.1 です。</span><span class="sxs-lookup"><span data-stu-id="f7493-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="f7493-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="f7493-127">windows81AndLater</span></span>|<span data-ttu-id="f7493-128">5</span><span class="sxs-lookup"><span data-stu-id="f7493-128">5</span></span>|<span data-ttu-id="f7493-129">およびそれ以降の Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="f7493-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="f7493-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="f7493-130">windows10AndLater</span></span>|<span data-ttu-id="f7493-131">6</span><span class="sxs-lookup"><span data-stu-id="f7493-131">6</span></span>|<span data-ttu-id="f7493-132">Windows 10 以降です。</span><span class="sxs-lookup"><span data-stu-id="f7493-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="f7493-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="f7493-133">androidWorkProfile</span></span>|<span data-ttu-id="f7493-134">7</span><span class="sxs-lookup"><span data-stu-id="f7493-134">7</span></span>|<span data-ttu-id="f7493-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="f7493-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="f7493-136">all</span><span class="sxs-lookup"><span data-stu-id="f7493-136">all</span></span>|<span data-ttu-id="f7493-137">100</span><span class="sxs-lookup"><span data-stu-id="f7493-137">100</span></span>|<span data-ttu-id="f7493-138">すべてのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="f7493-138">All platforms.</span></span>|





