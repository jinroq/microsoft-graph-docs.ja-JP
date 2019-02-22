---
title: androidforwork requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e0e99a5e54797441070308882d4137859390820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169476"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="e62cd-103">androidforwork requiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="e62cd-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="e62cd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e62cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e62cd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e62cd-106">Android 用 Android が必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="e62cd-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e62cd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e62cd-107">Members</span></span>
|<span data-ttu-id="e62cd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e62cd-108">Member</span></span>|<span data-ttu-id="e62cd-109">値</span><span class="sxs-lookup"><span data-stu-id="e62cd-109">Value</span></span>|<span data-ttu-id="e62cd-110">説明</span><span class="sxs-lookup"><span data-stu-id="e62cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62cd-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="e62cd-111">deviceDefault</span></span>|<span data-ttu-id="e62cd-112">.0</span><span class="sxs-lookup"><span data-stu-id="e62cd-112">0</span></span>|<span data-ttu-id="e62cd-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e62cd-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="e62cd-114">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="e62cd-114">lowSecurityBiometric</span></span>|<span data-ttu-id="e62cd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e62cd-115">1</span></span>|<span data-ttu-id="e62cd-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e62cd-117">必須</span><span class="sxs-lookup"><span data-stu-id="e62cd-117">required</span></span>|<span data-ttu-id="e62cd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e62cd-118">2</span></span>|<span data-ttu-id="e62cd-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-119">Required.</span></span>|
|<span data-ttu-id="e62cd-120">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="e62cd-120">atLeastNumeric</span></span>|<span data-ttu-id="e62cd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e62cd-121">3</span></span>|<span data-ttu-id="e62cd-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-122">At least numeric password required.</span></span>|
|<span data-ttu-id="e62cd-123">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="e62cd-123">numericComplex</span></span>|<span data-ttu-id="e62cd-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e62cd-124">4</span></span>|<span data-ttu-id="e62cd-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="e62cd-126">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="e62cd-126">atLeastAlphabetic</span></span>|<span data-ttu-id="e62cd-127">5</span><span class="sxs-lookup"><span data-stu-id="e62cd-127">5</span></span>|<span data-ttu-id="e62cd-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="e62cd-129">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="e62cd-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="e62cd-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e62cd-130">6</span></span>|<span data-ttu-id="e62cd-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e62cd-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="e62cd-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e62cd-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="e62cd-133">7</span><span class="sxs-lookup"><span data-stu-id="e62cd-133">7</span></span>|<span data-ttu-id="e62cd-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="e62cd-134">At least alphanumeric with symbols password required.</span></span>|




