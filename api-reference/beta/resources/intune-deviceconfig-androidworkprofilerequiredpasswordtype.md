---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e211fd0f793f710c31a303a73662af556c0794a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891526"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="26d4f-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="26d4f-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="26d4f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26d4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26d4f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26d4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26d4f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26d4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26d4f-107">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="26d4f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="26d4f-108">Members</span></span>
|<span data-ttu-id="26d4f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="26d4f-109">Member</span></span>|<span data-ttu-id="26d4f-110">値</span><span class="sxs-lookup"><span data-stu-id="26d4f-110">Value</span></span>|<span data-ttu-id="26d4f-111">説明</span><span class="sxs-lookup"><span data-stu-id="26d4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d4f-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="26d4f-112">deviceDefault</span></span>|<span data-ttu-id="26d4f-113">0</span><span class="sxs-lookup"><span data-stu-id="26d4f-113">0</span></span>|<span data-ttu-id="26d4f-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="26d4f-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="26d4f-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="26d4f-115">lowSecurityBiometric</span></span>|<span data-ttu-id="26d4f-116">1</span><span class="sxs-lookup"><span data-stu-id="26d4f-116">1</span></span>|<span data-ttu-id="26d4f-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="26d4f-118">必須</span><span class="sxs-lookup"><span data-stu-id="26d4f-118">required</span></span>|<span data-ttu-id="26d4f-119">2</span><span class="sxs-lookup"><span data-stu-id="26d4f-119">2</span></span>|<span data-ttu-id="26d4f-120">必須。</span><span class="sxs-lookup"><span data-stu-id="26d4f-120">Required.</span></span>|
|<span data-ttu-id="26d4f-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="26d4f-121">atLeastNumeric</span></span>|<span data-ttu-id="26d4f-122">3</span><span class="sxs-lookup"><span data-stu-id="26d4f-122">3</span></span>|<span data-ttu-id="26d4f-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-123">At least numeric password required.</span></span>|
|<span data-ttu-id="26d4f-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="26d4f-124">numericComplex</span></span>|<span data-ttu-id="26d4f-125">4</span><span class="sxs-lookup"><span data-stu-id="26d4f-125">4</span></span>|<span data-ttu-id="26d4f-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="26d4f-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="26d4f-127">atLeastAlphabetic</span></span>|<span data-ttu-id="26d4f-128">5</span><span class="sxs-lookup"><span data-stu-id="26d4f-128">5</span></span>|<span data-ttu-id="26d4f-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="26d4f-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="26d4f-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="26d4f-131">6</span><span class="sxs-lookup"><span data-stu-id="26d4f-131">6</span></span>|<span data-ttu-id="26d4f-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="26d4f-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="26d4f-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="26d4f-134">7</span><span class="sxs-lookup"><span data-stu-id="26d4f-134">7</span></span>|<span data-ttu-id="26d4f-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="26d4f-135">At least alphanumeric with symbols password required.</span></span>|





