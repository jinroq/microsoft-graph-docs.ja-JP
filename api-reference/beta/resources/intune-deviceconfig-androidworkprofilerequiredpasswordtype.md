---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルには、パスワード入力が必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cdf8c03dab6642cf6859ca822001a71b041c0e54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399900"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="61c95-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="61c95-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="61c95-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61c95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61c95-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61c95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61c95-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61c95-107">Android の作業プロファイルには、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="61c95-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="61c95-108">Members</span></span>
|<span data-ttu-id="61c95-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="61c95-109">Member</span></span>|<span data-ttu-id="61c95-110">値</span><span class="sxs-lookup"><span data-stu-id="61c95-110">Value</span></span>|<span data-ttu-id="61c95-111">説明</span><span class="sxs-lookup"><span data-stu-id="61c95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c95-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="61c95-112">deviceDefault</span></span>|<span data-ttu-id="61c95-113">0</span><span class="sxs-lookup"><span data-stu-id="61c95-113">0</span></span>|<span data-ttu-id="61c95-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="61c95-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="61c95-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="61c95-115">lowSecurityBiometric</span></span>|<span data-ttu-id="61c95-116">1</span><span class="sxs-lookup"><span data-stu-id="61c95-116">1</span></span>|<span data-ttu-id="61c95-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="61c95-118">必須</span><span class="sxs-lookup"><span data-stu-id="61c95-118">required</span></span>|<span data-ttu-id="61c95-119">2</span><span class="sxs-lookup"><span data-stu-id="61c95-119">2</span></span>|<span data-ttu-id="61c95-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="61c95-120">Required.</span></span>|
|<span data-ttu-id="61c95-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="61c95-121">atLeastNumeric</span></span>|<span data-ttu-id="61c95-122">3</span><span class="sxs-lookup"><span data-stu-id="61c95-122">3</span></span>|<span data-ttu-id="61c95-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-123">At least numeric password required.</span></span>|
|<span data-ttu-id="61c95-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="61c95-124">numericComplex</span></span>|<span data-ttu-id="61c95-125">4</span><span class="sxs-lookup"><span data-stu-id="61c95-125">4</span></span>|<span data-ttu-id="61c95-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="61c95-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="61c95-127">atLeastAlphabetic</span></span>|<span data-ttu-id="61c95-128">5</span><span class="sxs-lookup"><span data-stu-id="61c95-128">5</span></span>|<span data-ttu-id="61c95-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="61c95-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="61c95-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="61c95-131">6</span><span class="sxs-lookup"><span data-stu-id="61c95-131">6</span></span>|<span data-ttu-id="61c95-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="61c95-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="61c95-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="61c95-134">7</span><span class="sxs-lookup"><span data-stu-id="61c95-134">7</span></span>|<span data-ttu-id="61c95-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="61c95-135">At least alphanumeric with symbols password required.</span></span>|




