---
title: chassisType 列挙型
description: シャーシを入力します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7ad3d520042b44feb3bdd32ca07e6d783ce7d228
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947401"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="b2755-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b2755-103">chassisType enum type</span></span>

> <span data-ttu-id="b2755-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2755-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2755-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2755-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2755-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2755-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2755-107">シャーシを入力します。</span><span class="sxs-lookup"><span data-stu-id="b2755-107">Chassis type.</span></span>
## <a name="members"></a><span data-ttu-id="b2755-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2755-108">Members</span></span>
|<span data-ttu-id="b2755-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2755-109">Member</span></span>|<span data-ttu-id="b2755-110">値</span><span class="sxs-lookup"><span data-stu-id="b2755-110">Value</span></span>|<span data-ttu-id="b2755-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2755-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2755-112">不明</span><span class="sxs-lookup"><span data-stu-id="b2755-112">unknown</span></span>|<span data-ttu-id="b2755-113">0</span><span class="sxs-lookup"><span data-stu-id="b2755-113">0</span></span>|<span data-ttu-id="b2755-114">不明。</span><span class="sxs-lookup"><span data-stu-id="b2755-114">Unknown.</span></span>|
|<span data-ttu-id="b2755-115">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="b2755-115">desktop</span></span>|<span data-ttu-id="b2755-116">1</span><span class="sxs-lookup"><span data-stu-id="b2755-116">1</span></span>|<span data-ttu-id="b2755-117">デスクトップです。</span><span class="sxs-lookup"><span data-stu-id="b2755-117">Desktop.</span></span>|
|<span data-ttu-id="b2755-118">ラップトップ</span><span class="sxs-lookup"><span data-stu-id="b2755-118">laptop</span></span>|<span data-ttu-id="b2755-119">2</span><span class="sxs-lookup"><span data-stu-id="b2755-119">2</span></span>|<span data-ttu-id="b2755-120">ラップトップ コンピューター。</span><span class="sxs-lookup"><span data-stu-id="b2755-120">Laptop.</span></span>|
|<span data-ttu-id="b2755-121">worksWorkstation</span><span class="sxs-lookup"><span data-stu-id="b2755-121">worksWorkstation</span></span>|<span data-ttu-id="b2755-122">3</span><span class="sxs-lookup"><span data-stu-id="b2755-122">3</span></span>|<span data-ttu-id="b2755-123">ワークステーションです。</span><span class="sxs-lookup"><span data-stu-id="b2755-123">Workstation.</span></span>|
|<span data-ttu-id="b2755-124">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="b2755-124">enterpriseServer</span></span>|<span data-ttu-id="b2755-125">4</span><span class="sxs-lookup"><span data-stu-id="b2755-125">4</span></span>|<span data-ttu-id="b2755-126">エンタープライズ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="b2755-126">Enterprise server.</span></span>|
|<span data-ttu-id="b2755-127">phone</span><span class="sxs-lookup"><span data-stu-id="b2755-127">phone</span></span>|<span data-ttu-id="b2755-128">100</span><span class="sxs-lookup"><span data-stu-id="b2755-128">100</span></span>|<span data-ttu-id="b2755-129">電話です。</span><span class="sxs-lookup"><span data-stu-id="b2755-129">Phone.</span></span>|
|<span data-ttu-id="b2755-130">タブレット</span><span class="sxs-lookup"><span data-stu-id="b2755-130">tablet</span></span>|<span data-ttu-id="b2755-131">101</span><span class="sxs-lookup"><span data-stu-id="b2755-131">101</span></span>|<span data-ttu-id="b2755-132">モバイル タブレットです。</span><span class="sxs-lookup"><span data-stu-id="b2755-132">Mobile tablet.</span></span>|
|<span data-ttu-id="b2755-133">mobileOther</span><span class="sxs-lookup"><span data-stu-id="b2755-133">mobileOther</span></span>|<span data-ttu-id="b2755-134">102</span><span class="sxs-lookup"><span data-stu-id="b2755-134">102</span></span>|<span data-ttu-id="b2755-135">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="b2755-135">Other mobile.</span></span>|
|<span data-ttu-id="b2755-136">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="b2755-136">mobileUnknown</span></span>|<span data-ttu-id="b2755-137">103</span><span class="sxs-lookup"><span data-stu-id="b2755-137">103</span></span>|<span data-ttu-id="b2755-138">モバイル不明です。</span><span class="sxs-lookup"><span data-stu-id="b2755-138">Unknown mobile.</span></span>|





