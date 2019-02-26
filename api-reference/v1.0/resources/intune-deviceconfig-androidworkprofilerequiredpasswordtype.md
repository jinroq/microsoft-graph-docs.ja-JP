---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1dbb0b7e523ea6ca3ac1be3328cf58e30d9a892
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252939"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="d4545-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d4545-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d4545-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4545-105">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="d4545-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d4545-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d4545-106">Members</span></span>
|<span data-ttu-id="d4545-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d4545-107">Member</span></span>|<span data-ttu-id="d4545-108">値</span><span class="sxs-lookup"><span data-stu-id="d4545-108">Value</span></span>|<span data-ttu-id="d4545-109">説明</span><span class="sxs-lookup"><span data-stu-id="d4545-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4545-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="d4545-110">deviceDefault</span></span>|<span data-ttu-id="d4545-111">.0</span><span class="sxs-lookup"><span data-stu-id="d4545-111">0</span></span>|<span data-ttu-id="d4545-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="d4545-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="d4545-113">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="d4545-113">lowSecurityBiometric</span></span>|<span data-ttu-id="d4545-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d4545-114">1</span></span>|<span data-ttu-id="d4545-115">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d4545-116">必須</span><span class="sxs-lookup"><span data-stu-id="d4545-116">required</span></span>|<span data-ttu-id="d4545-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d4545-117">2</span></span>|<span data-ttu-id="d4545-118">必須です。</span><span class="sxs-lookup"><span data-stu-id="d4545-118">Required.</span></span>|
|<span data-ttu-id="d4545-119">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="d4545-119">atLeastNumeric</span></span>|<span data-ttu-id="d4545-120">1/3</span><span class="sxs-lookup"><span data-stu-id="d4545-120">3</span></span>|<span data-ttu-id="d4545-121">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-121">At least numeric password required.</span></span>|
|<span data-ttu-id="d4545-122">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="d4545-122">numericComplex</span></span>|<span data-ttu-id="d4545-123">2/4</span><span class="sxs-lookup"><span data-stu-id="d4545-123">4</span></span>|<span data-ttu-id="d4545-124">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="d4545-125">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="d4545-125">atLeastAlphabetic</span></span>|<span data-ttu-id="d4545-126">5</span><span class="sxs-lookup"><span data-stu-id="d4545-126">5</span></span>|<span data-ttu-id="d4545-127">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="d4545-128">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="d4545-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="d4545-129">シックス</span><span class="sxs-lookup"><span data-stu-id="d4545-129">6</span></span>|<span data-ttu-id="d4545-130">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d4545-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="d4545-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d4545-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="d4545-132">7</span><span class="sxs-lookup"><span data-stu-id="d4545-132">7</span></span>|<span data-ttu-id="d4545-133">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="d4545-133">At least alphanumeric with symbols password required.</span></span>|



