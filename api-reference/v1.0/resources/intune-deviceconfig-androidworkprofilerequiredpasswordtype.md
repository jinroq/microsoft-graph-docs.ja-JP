---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
ms.openlocfilehash: f9cdf225f9fe7dfc42fb728bad615a7abde11bef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020657"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="930e7-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="930e7-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="930e7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="930e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="930e7-105">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="930e7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="930e7-106">Members</span></span>
|<span data-ttu-id="930e7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="930e7-107">Member</span></span>|<span data-ttu-id="930e7-108">値</span><span class="sxs-lookup"><span data-stu-id="930e7-108">Value</span></span>|<span data-ttu-id="930e7-109">説明</span><span class="sxs-lookup"><span data-stu-id="930e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="930e7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="930e7-110">deviceDefault</span></span>|<span data-ttu-id="930e7-111">0</span><span class="sxs-lookup"><span data-stu-id="930e7-111">0</span></span>|<span data-ttu-id="930e7-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="930e7-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="930e7-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="930e7-113">lowSecurityBiometric</span></span>|<span data-ttu-id="930e7-114">1</span><span class="sxs-lookup"><span data-stu-id="930e7-114">1</span></span>|<span data-ttu-id="930e7-115">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="930e7-116">必須</span><span class="sxs-lookup"><span data-stu-id="930e7-116">required</span></span>|<span data-ttu-id="930e7-117">2</span><span class="sxs-lookup"><span data-stu-id="930e7-117">2</span></span>|<span data-ttu-id="930e7-118">必須。</span><span class="sxs-lookup"><span data-stu-id="930e7-118">Required.</span></span>|
|<span data-ttu-id="930e7-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="930e7-119">atLeastNumeric</span></span>|<span data-ttu-id="930e7-120">3</span><span class="sxs-lookup"><span data-stu-id="930e7-120">3</span></span>|<span data-ttu-id="930e7-121">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-121">At least numeric password required.</span></span>|
|<span data-ttu-id="930e7-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="930e7-122">numericComplex</span></span>|<span data-ttu-id="930e7-123">4</span><span class="sxs-lookup"><span data-stu-id="930e7-123">4</span></span>|<span data-ttu-id="930e7-124">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="930e7-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="930e7-125">atLeastAlphabetic</span></span>|<span data-ttu-id="930e7-126">5</span><span class="sxs-lookup"><span data-stu-id="930e7-126">5</span></span>|<span data-ttu-id="930e7-127">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="930e7-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="930e7-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="930e7-129">6</span><span class="sxs-lookup"><span data-stu-id="930e7-129">6</span></span>|<span data-ttu-id="930e7-130">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="930e7-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="930e7-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="930e7-132">7</span><span class="sxs-lookup"><span data-stu-id="930e7-132">7</span></span>|<span data-ttu-id="930e7-133">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="930e7-133">At least alphanumeric with symbols password required.</span></span>|



