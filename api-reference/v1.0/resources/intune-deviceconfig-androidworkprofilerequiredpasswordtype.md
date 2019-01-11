---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c77b9b3265a5c3f64da93df58d5a605923dff69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809934"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="4b56b-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4b56b-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="4b56b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b56b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b56b-105">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="4b56b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b56b-106">Members</span></span>
|<span data-ttu-id="4b56b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b56b-107">Member</span></span>|<span data-ttu-id="4b56b-108">値</span><span class="sxs-lookup"><span data-stu-id="4b56b-108">Value</span></span>|<span data-ttu-id="4b56b-109">説明</span><span class="sxs-lookup"><span data-stu-id="4b56b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b56b-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4b56b-110">deviceDefault</span></span>|<span data-ttu-id="4b56b-111">0</span><span class="sxs-lookup"><span data-stu-id="4b56b-111">0</span></span>|<span data-ttu-id="4b56b-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="4b56b-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="4b56b-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="4b56b-113">lowSecurityBiometric</span></span>|<span data-ttu-id="4b56b-114">1</span><span class="sxs-lookup"><span data-stu-id="4b56b-114">1</span></span>|<span data-ttu-id="4b56b-115">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="4b56b-116">必須</span><span class="sxs-lookup"><span data-stu-id="4b56b-116">required</span></span>|<span data-ttu-id="4b56b-117">2</span><span class="sxs-lookup"><span data-stu-id="4b56b-117">2</span></span>|<span data-ttu-id="4b56b-118">必須。</span><span class="sxs-lookup"><span data-stu-id="4b56b-118">Required.</span></span>|
|<span data-ttu-id="4b56b-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="4b56b-119">atLeastNumeric</span></span>|<span data-ttu-id="4b56b-120">3</span><span class="sxs-lookup"><span data-stu-id="4b56b-120">3</span></span>|<span data-ttu-id="4b56b-121">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-121">At least numeric password required.</span></span>|
|<span data-ttu-id="4b56b-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4b56b-122">numericComplex</span></span>|<span data-ttu-id="4b56b-123">4</span><span class="sxs-lookup"><span data-stu-id="4b56b-123">4</span></span>|<span data-ttu-id="4b56b-124">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="4b56b-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="4b56b-125">atLeastAlphabetic</span></span>|<span data-ttu-id="4b56b-126">5</span><span class="sxs-lookup"><span data-stu-id="4b56b-126">5</span></span>|<span data-ttu-id="4b56b-127">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="4b56b-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="4b56b-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="4b56b-129">6</span><span class="sxs-lookup"><span data-stu-id="4b56b-129">6</span></span>|<span data-ttu-id="4b56b-130">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="4b56b-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4b56b-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="4b56b-132">7</span><span class="sxs-lookup"><span data-stu-id="4b56b-132">7</span></span>|<span data-ttu-id="4b56b-133">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b56b-133">At least alphanumeric with symbols password required.</span></span>|



