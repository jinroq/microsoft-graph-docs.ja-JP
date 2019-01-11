---
title: chassisType 列挙型
description: シャーシを入力します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2010957c48623fc5e01eeb87a95251d743f29b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806399"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="dc06b-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="dc06b-103">chassisType enum type</span></span>

> <span data-ttu-id="dc06b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc06b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc06b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc06b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc06b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc06b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc06b-107">シャーシを入力します。</span><span class="sxs-lookup"><span data-stu-id="dc06b-107">Chassis type.</span></span>
## <a name="members"></a><span data-ttu-id="dc06b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc06b-108">Members</span></span>
|<span data-ttu-id="dc06b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc06b-109">Member</span></span>|<span data-ttu-id="dc06b-110">値</span><span class="sxs-lookup"><span data-stu-id="dc06b-110">Value</span></span>|<span data-ttu-id="dc06b-111">説明</span><span class="sxs-lookup"><span data-stu-id="dc06b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc06b-112">不明</span><span class="sxs-lookup"><span data-stu-id="dc06b-112">unknown</span></span>|<span data-ttu-id="dc06b-113">0</span><span class="sxs-lookup"><span data-stu-id="dc06b-113">0</span></span>|<span data-ttu-id="dc06b-114">不明。</span><span class="sxs-lookup"><span data-stu-id="dc06b-114">Unknown.</span></span>|
|<span data-ttu-id="dc06b-115">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="dc06b-115">desktop</span></span>|<span data-ttu-id="dc06b-116">1</span><span class="sxs-lookup"><span data-stu-id="dc06b-116">1</span></span>|<span data-ttu-id="dc06b-117">デスクトップです。</span><span class="sxs-lookup"><span data-stu-id="dc06b-117">Desktop.</span></span>|
|<span data-ttu-id="dc06b-118">ラップトップ</span><span class="sxs-lookup"><span data-stu-id="dc06b-118">laptop</span></span>|<span data-ttu-id="dc06b-119">2</span><span class="sxs-lookup"><span data-stu-id="dc06b-119">2</span></span>|<span data-ttu-id="dc06b-120">ラップトップ コンピューター。</span><span class="sxs-lookup"><span data-stu-id="dc06b-120">Laptop.</span></span>|
|<span data-ttu-id="dc06b-121">worksWorkstation</span><span class="sxs-lookup"><span data-stu-id="dc06b-121">worksWorkstation</span></span>|<span data-ttu-id="dc06b-122">3</span><span class="sxs-lookup"><span data-stu-id="dc06b-122">3</span></span>|<span data-ttu-id="dc06b-123">ワークステーションです。</span><span class="sxs-lookup"><span data-stu-id="dc06b-123">Workstation.</span></span>|
|<span data-ttu-id="dc06b-124">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="dc06b-124">enterpriseServer</span></span>|<span data-ttu-id="dc06b-125">4</span><span class="sxs-lookup"><span data-stu-id="dc06b-125">4</span></span>|<span data-ttu-id="dc06b-126">エンタープライズ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="dc06b-126">Enterprise server.</span></span>|
|<span data-ttu-id="dc06b-127">phone</span><span class="sxs-lookup"><span data-stu-id="dc06b-127">phone</span></span>|<span data-ttu-id="dc06b-128">100</span><span class="sxs-lookup"><span data-stu-id="dc06b-128">100</span></span>|<span data-ttu-id="dc06b-129">電話です。</span><span class="sxs-lookup"><span data-stu-id="dc06b-129">Phone.</span></span>|
|<span data-ttu-id="dc06b-130">タブレット</span><span class="sxs-lookup"><span data-stu-id="dc06b-130">tablet</span></span>|<span data-ttu-id="dc06b-131">101</span><span class="sxs-lookup"><span data-stu-id="dc06b-131">101</span></span>|<span data-ttu-id="dc06b-132">モバイル タブレットです。</span><span class="sxs-lookup"><span data-stu-id="dc06b-132">Mobile tablet.</span></span>|
|<span data-ttu-id="dc06b-133">mobileOther</span><span class="sxs-lookup"><span data-stu-id="dc06b-133">mobileOther</span></span>|<span data-ttu-id="dc06b-134">102</span><span class="sxs-lookup"><span data-stu-id="dc06b-134">102</span></span>|<span data-ttu-id="dc06b-135">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="dc06b-135">Other mobile.</span></span>|
|<span data-ttu-id="dc06b-136">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="dc06b-136">mobileUnknown</span></span>|<span data-ttu-id="dc06b-137">103</span><span class="sxs-lookup"><span data-stu-id="dc06b-137">103</span></span>|<span data-ttu-id="dc06b-138">モバイル不明です。</span><span class="sxs-lookup"><span data-stu-id="dc06b-138">Unknown mobile.</span></span>|





