---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbe1eb1482e979d236c1f8bf92f687077fb189f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986279"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="aecd5-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="aecd5-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="aecd5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aecd5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aecd5-105">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="aecd5-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="aecd5-106">Members</span></span>
|<span data-ttu-id="aecd5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="aecd5-107">Member</span></span>|<span data-ttu-id="aecd5-108">値</span><span class="sxs-lookup"><span data-stu-id="aecd5-108">Value</span></span>|<span data-ttu-id="aecd5-109">説明</span><span class="sxs-lookup"><span data-stu-id="aecd5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aecd5-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="aecd5-110">deviceDefault</span></span>|<span data-ttu-id="aecd5-111">0</span><span class="sxs-lookup"><span data-stu-id="aecd5-111">0</span></span>|<span data-ttu-id="aecd5-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="aecd5-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="aecd5-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="aecd5-113">lowSecurityBiometric</span></span>|<span data-ttu-id="aecd5-114">1</span><span class="sxs-lookup"><span data-stu-id="aecd5-114">1</span></span>|<span data-ttu-id="aecd5-115">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="aecd5-116">必須</span><span class="sxs-lookup"><span data-stu-id="aecd5-116">required</span></span>|<span data-ttu-id="aecd5-117">2</span><span class="sxs-lookup"><span data-stu-id="aecd5-117">2</span></span>|<span data-ttu-id="aecd5-118">必須。</span><span class="sxs-lookup"><span data-stu-id="aecd5-118">Required.</span></span>|
|<span data-ttu-id="aecd5-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="aecd5-119">atLeastNumeric</span></span>|<span data-ttu-id="aecd5-120">3</span><span class="sxs-lookup"><span data-stu-id="aecd5-120">3</span></span>|<span data-ttu-id="aecd5-121">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-121">At least numeric password required.</span></span>|
|<span data-ttu-id="aecd5-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="aecd5-122">numericComplex</span></span>|<span data-ttu-id="aecd5-123">4</span><span class="sxs-lookup"><span data-stu-id="aecd5-123">4</span></span>|<span data-ttu-id="aecd5-124">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="aecd5-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="aecd5-125">atLeastAlphabetic</span></span>|<span data-ttu-id="aecd5-126">5</span><span class="sxs-lookup"><span data-stu-id="aecd5-126">5</span></span>|<span data-ttu-id="aecd5-127">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="aecd5-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="aecd5-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="aecd5-129">6</span><span class="sxs-lookup"><span data-stu-id="aecd5-129">6</span></span>|<span data-ttu-id="aecd5-130">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="aecd5-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="aecd5-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="aecd5-132">7</span><span class="sxs-lookup"><span data-stu-id="aecd5-132">7</span></span>|<span data-ttu-id="aecd5-133">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="aecd5-133">At least alphanumeric with symbols password required.</span></span>|



