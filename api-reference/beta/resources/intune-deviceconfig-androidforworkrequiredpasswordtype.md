---
title: androidForWorkRequiredPasswordType 列挙型
description: Android の作業には、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc944cf87e9a8daa5c50f31fbb095f09dbee1a65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933583"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="9db77-103">androidForWorkRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9db77-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9db77-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9db77-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9db77-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9db77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9db77-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9db77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9db77-107">Android の作業には、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="9db77-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9db77-108">Members</span></span>
|<span data-ttu-id="9db77-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9db77-109">Member</span></span>|<span data-ttu-id="9db77-110">値</span><span class="sxs-lookup"><span data-stu-id="9db77-110">Value</span></span>|<span data-ttu-id="9db77-111">説明</span><span class="sxs-lookup"><span data-stu-id="9db77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db77-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9db77-112">deviceDefault</span></span>|<span data-ttu-id="9db77-113">0</span><span class="sxs-lookup"><span data-stu-id="9db77-113">0</span></span>|<span data-ttu-id="9db77-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="9db77-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9db77-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9db77-115">lowSecurityBiometric</span></span>|<span data-ttu-id="9db77-116">1</span><span class="sxs-lookup"><span data-stu-id="9db77-116">1</span></span>|<span data-ttu-id="9db77-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9db77-118">必須</span><span class="sxs-lookup"><span data-stu-id="9db77-118">required</span></span>|<span data-ttu-id="9db77-119">2</span><span class="sxs-lookup"><span data-stu-id="9db77-119">2</span></span>|<span data-ttu-id="9db77-120">必須。</span><span class="sxs-lookup"><span data-stu-id="9db77-120">Required.</span></span>|
|<span data-ttu-id="9db77-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="9db77-121">atLeastNumeric</span></span>|<span data-ttu-id="9db77-122">3</span><span class="sxs-lookup"><span data-stu-id="9db77-122">3</span></span>|<span data-ttu-id="9db77-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-123">At least numeric password required.</span></span>|
|<span data-ttu-id="9db77-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9db77-124">numericComplex</span></span>|<span data-ttu-id="9db77-125">4</span><span class="sxs-lookup"><span data-stu-id="9db77-125">4</span></span>|<span data-ttu-id="9db77-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="9db77-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="9db77-127">atLeastAlphabetic</span></span>|<span data-ttu-id="9db77-128">5</span><span class="sxs-lookup"><span data-stu-id="9db77-128">5</span></span>|<span data-ttu-id="9db77-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9db77-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="9db77-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="9db77-131">6</span><span class="sxs-lookup"><span data-stu-id="9db77-131">6</span></span>|<span data-ttu-id="9db77-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9db77-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9db77-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="9db77-134">7</span><span class="sxs-lookup"><span data-stu-id="9db77-134">7</span></span>|<span data-ttu-id="9db77-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9db77-135">At least alphanumeric with symbols password required.</span></span>|





