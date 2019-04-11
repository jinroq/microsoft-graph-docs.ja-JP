---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bbe0e64fdbbca78766bf7471d29d6cdf17b0714
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802724"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="f95b4-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f95b4-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f95b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f95b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f95b4-106">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f95b4-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f95b4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f95b4-107">Members</span></span>
|<span data-ttu-id="f95b4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f95b4-108">Member</span></span>|<span data-ttu-id="f95b4-109">値</span><span class="sxs-lookup"><span data-stu-id="f95b4-109">Value</span></span>|<span data-ttu-id="f95b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="f95b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f95b4-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="f95b4-111">deviceDefault</span></span>|<span data-ttu-id="f95b4-112">.0</span><span class="sxs-lookup"><span data-stu-id="f95b4-112">0</span></span>|<span data-ttu-id="f95b4-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f95b4-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f95b4-114">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="f95b4-114">lowSecurityBiometric</span></span>|<span data-ttu-id="f95b4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f95b4-115">1</span></span>|<span data-ttu-id="f95b4-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f95b4-117">必須</span><span class="sxs-lookup"><span data-stu-id="f95b4-117">required</span></span>|<span data-ttu-id="f95b4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f95b4-118">2</span></span>|<span data-ttu-id="f95b4-119">必須。</span><span class="sxs-lookup"><span data-stu-id="f95b4-119">Required.</span></span>|
|<span data-ttu-id="f95b4-120">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="f95b4-120">atLeastNumeric</span></span>|<span data-ttu-id="f95b4-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f95b4-121">3</span></span>|<span data-ttu-id="f95b4-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-122">At least numeric password required.</span></span>|
|<span data-ttu-id="f95b4-123">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="f95b4-123">numericComplex</span></span>|<span data-ttu-id="f95b4-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f95b4-124">4</span></span>|<span data-ttu-id="f95b4-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="f95b4-126">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="f95b4-126">atLeastAlphabetic</span></span>|<span data-ttu-id="f95b4-127">5</span><span class="sxs-lookup"><span data-stu-id="f95b4-127">5</span></span>|<span data-ttu-id="f95b4-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="f95b4-129">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="f95b4-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="f95b4-130">シックス</span><span class="sxs-lookup"><span data-stu-id="f95b4-130">6</span></span>|<span data-ttu-id="f95b4-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f95b4-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="f95b4-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f95b4-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="f95b4-133">7</span><span class="sxs-lookup"><span data-stu-id="f95b4-133">7</span></span>|<span data-ttu-id="f95b4-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="f95b4-134">At least alphanumeric with symbols password required.</span></span>|





