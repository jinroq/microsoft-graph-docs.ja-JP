---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b384c6d5bcc3c79a967d1a4c4cdfc8299d1a56d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947667"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="c2b06-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c2b06-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c2b06-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2b06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b06-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b06-106">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c2b06-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c2b06-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c2b06-107">Members</span></span>
|<span data-ttu-id="c2b06-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c2b06-108">Member</span></span>|<span data-ttu-id="c2b06-109">値</span><span class="sxs-lookup"><span data-stu-id="c2b06-109">Value</span></span>|<span data-ttu-id="c2b06-110">説明</span><span class="sxs-lookup"><span data-stu-id="c2b06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b06-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c2b06-111">deviceDefault</span></span>|<span data-ttu-id="c2b06-112">.0</span><span class="sxs-lookup"><span data-stu-id="c2b06-112">0</span></span>|<span data-ttu-id="c2b06-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c2b06-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c2b06-114">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="c2b06-114">lowSecurityBiometric</span></span>|<span data-ttu-id="c2b06-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c2b06-115">1</span></span>|<span data-ttu-id="c2b06-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c2b06-117">必須</span><span class="sxs-lookup"><span data-stu-id="c2b06-117">required</span></span>|<span data-ttu-id="c2b06-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c2b06-118">2</span></span>|<span data-ttu-id="c2b06-119">必須。</span><span class="sxs-lookup"><span data-stu-id="c2b06-119">Required.</span></span>|
|<span data-ttu-id="c2b06-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="c2b06-120">atLeastNumeric</span></span>|<span data-ttu-id="c2b06-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c2b06-121">3</span></span>|<span data-ttu-id="c2b06-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-122">At least numeric password required.</span></span>|
|<span data-ttu-id="c2b06-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c2b06-123">numericComplex</span></span>|<span data-ttu-id="c2b06-124">2/4</span><span class="sxs-lookup"><span data-stu-id="c2b06-124">4</span></span>|<span data-ttu-id="c2b06-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="c2b06-126">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="c2b06-126">atLeastAlphabetic</span></span>|<span data-ttu-id="c2b06-127">5</span><span class="sxs-lookup"><span data-stu-id="c2b06-127">5</span></span>|<span data-ttu-id="c2b06-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c2b06-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="c2b06-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="c2b06-130">シックス</span><span class="sxs-lookup"><span data-stu-id="c2b06-130">6</span></span>|<span data-ttu-id="c2b06-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c2b06-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c2b06-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c2b06-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="c2b06-133">7</span><span class="sxs-lookup"><span data-stu-id="c2b06-133">7</span></span>|<span data-ttu-id="c2b06-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="c2b06-134">At least alphanumeric with symbols password required.</span></span>|




