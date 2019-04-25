---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1dbb0b7e523ea6ca3ac1be3328cf58e30d9a892
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575157"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="f542e-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f542e-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f542e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f542e-105">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f542e-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f542e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f542e-106">Members</span></span>
|<span data-ttu-id="f542e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f542e-107">Member</span></span>|<span data-ttu-id="f542e-108">値</span><span class="sxs-lookup"><span data-stu-id="f542e-108">Value</span></span>|<span data-ttu-id="f542e-109">説明</span><span class="sxs-lookup"><span data-stu-id="f542e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f542e-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="f542e-110">deviceDefault</span></span>|<span data-ttu-id="f542e-111">.0</span><span class="sxs-lookup"><span data-stu-id="f542e-111">0</span></span>|<span data-ttu-id="f542e-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f542e-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="f542e-113">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="f542e-113">lowSecurityBiometric</span></span>|<span data-ttu-id="f542e-114">1 </span><span class="sxs-lookup"><span data-stu-id="f542e-114">1</span></span>|<span data-ttu-id="f542e-115">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f542e-116">必須</span><span class="sxs-lookup"><span data-stu-id="f542e-116">required</span></span>|<span data-ttu-id="f542e-117">2 </span><span class="sxs-lookup"><span data-stu-id="f542e-117">2</span></span>|<span data-ttu-id="f542e-118">必須です。</span><span class="sxs-lookup"><span data-stu-id="f542e-118">Required.</span></span>|
|<span data-ttu-id="f542e-119">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="f542e-119">atLeastNumeric</span></span>|<span data-ttu-id="f542e-120">3 </span><span class="sxs-lookup"><span data-stu-id="f542e-120">3</span></span>|<span data-ttu-id="f542e-121">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-121">At least numeric password required.</span></span>|
|<span data-ttu-id="f542e-122">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="f542e-122">numericComplex</span></span>|<span data-ttu-id="f542e-123">4 </span><span class="sxs-lookup"><span data-stu-id="f542e-123">4</span></span>|<span data-ttu-id="f542e-124">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="f542e-125">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="f542e-125">atLeastAlphabetic</span></span>|<span data-ttu-id="f542e-126">5 </span><span class="sxs-lookup"><span data-stu-id="f542e-126">5</span></span>|<span data-ttu-id="f542e-127">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="f542e-128">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="f542e-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="f542e-129">6 </span><span class="sxs-lookup"><span data-stu-id="f542e-129">6</span></span>|<span data-ttu-id="f542e-130">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f542e-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="f542e-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f542e-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="f542e-132">7 </span><span class="sxs-lookup"><span data-stu-id="f542e-132">7</span></span>|<span data-ttu-id="f542e-133">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="f542e-133">At least alphanumeric with symbols password required.</span></span>|



