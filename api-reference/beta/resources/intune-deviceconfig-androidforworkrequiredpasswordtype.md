---
title: androidForWorkRequiredPasswordType 列挙型
description: Android の作業には、パスワード入力が必要です。
ms.openlocfilehash: 8866ac49126f39204e0323082bf80e27f5f59962
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069098"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="0e702-103">androidForWorkRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0e702-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0e702-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e702-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e702-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e702-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e702-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e702-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e702-107">Android の作業には、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="0e702-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e702-108">Members</span></span>
|<span data-ttu-id="0e702-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e702-109">Member</span></span>|<span data-ttu-id="0e702-110">値</span><span class="sxs-lookup"><span data-stu-id="0e702-110">Value</span></span>|<span data-ttu-id="0e702-111">説明</span><span class="sxs-lookup"><span data-stu-id="0e702-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e702-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0e702-112">deviceDefault</span></span>|<span data-ttu-id="0e702-113">0</span><span class="sxs-lookup"><span data-stu-id="0e702-113">0</span></span>|<span data-ttu-id="0e702-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="0e702-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="0e702-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="0e702-115">lowSecurityBiometric</span></span>|<span data-ttu-id="0e702-116">1</span><span class="sxs-lookup"><span data-stu-id="0e702-116">1</span></span>|<span data-ttu-id="0e702-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0e702-118">必須</span><span class="sxs-lookup"><span data-stu-id="0e702-118">required</span></span>|<span data-ttu-id="0e702-119">2</span><span class="sxs-lookup"><span data-stu-id="0e702-119">2</span></span>|<span data-ttu-id="0e702-120">必須。</span><span class="sxs-lookup"><span data-stu-id="0e702-120">Required.</span></span>|
|<span data-ttu-id="0e702-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="0e702-121">atLeastNumeric</span></span>|<span data-ttu-id="0e702-122">3</span><span class="sxs-lookup"><span data-stu-id="0e702-122">3</span></span>|<span data-ttu-id="0e702-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-123">At least numeric password required.</span></span>|
|<span data-ttu-id="0e702-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="0e702-124">numericComplex</span></span>|<span data-ttu-id="0e702-125">4</span><span class="sxs-lookup"><span data-stu-id="0e702-125">4</span></span>|<span data-ttu-id="0e702-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="0e702-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="0e702-127">atLeastAlphabetic</span></span>|<span data-ttu-id="0e702-128">5</span><span class="sxs-lookup"><span data-stu-id="0e702-128">5</span></span>|<span data-ttu-id="0e702-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="0e702-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="0e702-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="0e702-131">6</span><span class="sxs-lookup"><span data-stu-id="0e702-131">6</span></span>|<span data-ttu-id="0e702-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="0e702-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="0e702-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="0e702-134">7</span><span class="sxs-lookup"><span data-stu-id="0e702-134">7</span></span>|<span data-ttu-id="0e702-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e702-135">At least alphanumeric with symbols password required.</span></span>|





