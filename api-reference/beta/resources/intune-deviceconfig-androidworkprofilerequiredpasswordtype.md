---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bbe0e64fdbbca78766bf7471d29d6cdf17b0714
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562357"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="5eb1c-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5eb1c-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="5eb1c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5eb1c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eb1c-106">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="5eb1c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5eb1c-107">Members</span></span>
|<span data-ttu-id="5eb1c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5eb1c-108">Member</span></span>|<span data-ttu-id="5eb1c-109">値</span><span class="sxs-lookup"><span data-stu-id="5eb1c-109">Value</span></span>|<span data-ttu-id="5eb1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="5eb1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb1c-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="5eb1c-111">deviceDefault</span></span>|<span data-ttu-id="5eb1c-112">.0</span><span class="sxs-lookup"><span data-stu-id="5eb1c-112">0</span></span>|<span data-ttu-id="5eb1c-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="5eb1c-114">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="5eb1c-114">lowSecurityBiometric</span></span>|<span data-ttu-id="5eb1c-115">1 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-115">1</span></span>|<span data-ttu-id="5eb1c-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="5eb1c-117">必須</span><span class="sxs-lookup"><span data-stu-id="5eb1c-117">required</span></span>|<span data-ttu-id="5eb1c-118">2 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-118">2</span></span>|<span data-ttu-id="5eb1c-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-119">Required.</span></span>|
|<span data-ttu-id="5eb1c-120">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="5eb1c-120">atLeastNumeric</span></span>|<span data-ttu-id="5eb1c-121">3 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-121">3</span></span>|<span data-ttu-id="5eb1c-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-122">At least numeric password required.</span></span>|
|<span data-ttu-id="5eb1c-123">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="5eb1c-123">numericComplex</span></span>|<span data-ttu-id="5eb1c-124">4 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-124">4</span></span>|<span data-ttu-id="5eb1c-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="5eb1c-126">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="5eb1c-126">atLeastAlphabetic</span></span>|<span data-ttu-id="5eb1c-127">5 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-127">5</span></span>|<span data-ttu-id="5eb1c-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="5eb1c-129">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="5eb1c-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="5eb1c-130">6 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-130">6</span></span>|<span data-ttu-id="5eb1c-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="5eb1c-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="5eb1c-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="5eb1c-133">7 </span><span class="sxs-lookup"><span data-stu-id="5eb1c-133">7</span></span>|<span data-ttu-id="5eb1c-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="5eb1c-134">At least alphanumeric with symbols password required.</span></span>|





