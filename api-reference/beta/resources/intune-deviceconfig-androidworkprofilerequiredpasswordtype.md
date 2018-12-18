---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: 8d41b4c516ee4aa393ea3a26034e5f575b58fa02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330234"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="9304d-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9304d-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9304d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9304d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9304d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9304d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9304d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9304d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9304d-107">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="9304d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9304d-108">Members</span></span>
|<span data-ttu-id="9304d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9304d-109">Member</span></span>|<span data-ttu-id="9304d-110">値</span><span class="sxs-lookup"><span data-stu-id="9304d-110">Value</span></span>|<span data-ttu-id="9304d-111">説明</span><span class="sxs-lookup"><span data-stu-id="9304d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9304d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9304d-112">deviceDefault</span></span>|<span data-ttu-id="9304d-113">0</span><span class="sxs-lookup"><span data-stu-id="9304d-113">0</span></span>|<span data-ttu-id="9304d-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="9304d-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9304d-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9304d-115">lowSecurityBiometric</span></span>|<span data-ttu-id="9304d-116">1</span><span class="sxs-lookup"><span data-stu-id="9304d-116">1</span></span>|<span data-ttu-id="9304d-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9304d-118">必須</span><span class="sxs-lookup"><span data-stu-id="9304d-118">required</span></span>|<span data-ttu-id="9304d-119">2</span><span class="sxs-lookup"><span data-stu-id="9304d-119">2</span></span>|<span data-ttu-id="9304d-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="9304d-120">Required.</span></span>|
|<span data-ttu-id="9304d-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="9304d-121">atLeastNumeric</span></span>|<span data-ttu-id="9304d-122">3</span><span class="sxs-lookup"><span data-stu-id="9304d-122">3</span></span>|<span data-ttu-id="9304d-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-123">At least numeric password required.</span></span>|
|<span data-ttu-id="9304d-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9304d-124">numericComplex</span></span>|<span data-ttu-id="9304d-125">4</span><span class="sxs-lookup"><span data-stu-id="9304d-125">4</span></span>|<span data-ttu-id="9304d-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="9304d-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="9304d-127">atLeastAlphabetic</span></span>|<span data-ttu-id="9304d-128">5</span><span class="sxs-lookup"><span data-stu-id="9304d-128">5</span></span>|<span data-ttu-id="9304d-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9304d-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="9304d-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="9304d-131">6</span><span class="sxs-lookup"><span data-stu-id="9304d-131">6</span></span>|<span data-ttu-id="9304d-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9304d-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9304d-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="9304d-134">7</span><span class="sxs-lookup"><span data-stu-id="9304d-134">7</span></span>|<span data-ttu-id="9304d-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9304d-135">At least alphanumeric with symbols password required.</span></span>|





