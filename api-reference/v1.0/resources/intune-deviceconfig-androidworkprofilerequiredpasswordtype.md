---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2e9c65138a6dee7082b85261fd62c0fe9a9fd5e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028680"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="70507-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="70507-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="70507-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70507-105">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="70507-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="70507-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="70507-106">Members</span></span>
|<span data-ttu-id="70507-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="70507-107">Member</span></span>|<span data-ttu-id="70507-108">値</span><span class="sxs-lookup"><span data-stu-id="70507-108">Value</span></span>|<span data-ttu-id="70507-109">説明</span><span class="sxs-lookup"><span data-stu-id="70507-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70507-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="70507-110">deviceDefault</span></span>|<span data-ttu-id="70507-111">.0</span><span class="sxs-lookup"><span data-stu-id="70507-111">0</span></span>|<span data-ttu-id="70507-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="70507-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="70507-113">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="70507-113">lowSecurityBiometric</span></span>|<span data-ttu-id="70507-114">1-d</span><span class="sxs-lookup"><span data-stu-id="70507-114">1</span></span>|<span data-ttu-id="70507-115">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="70507-116">必須</span><span class="sxs-lookup"><span data-stu-id="70507-116">required</span></span>|<span data-ttu-id="70507-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="70507-117">2</span></span>|<span data-ttu-id="70507-118">必須です。</span><span class="sxs-lookup"><span data-stu-id="70507-118">Required.</span></span>|
|<span data-ttu-id="70507-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="70507-119">atLeastNumeric</span></span>|<span data-ttu-id="70507-120">1/3</span><span class="sxs-lookup"><span data-stu-id="70507-120">3</span></span>|<span data-ttu-id="70507-121">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-121">At least numeric password required.</span></span>|
|<span data-ttu-id="70507-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="70507-122">numericComplex</span></span>|<span data-ttu-id="70507-123">2/4</span><span class="sxs-lookup"><span data-stu-id="70507-123">4</span></span>|<span data-ttu-id="70507-124">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="70507-125">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="70507-125">atLeastAlphabetic</span></span>|<span data-ttu-id="70507-126">5</span><span class="sxs-lookup"><span data-stu-id="70507-126">5</span></span>|<span data-ttu-id="70507-127">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="70507-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="70507-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="70507-129">シックス</span><span class="sxs-lookup"><span data-stu-id="70507-129">6</span></span>|<span data-ttu-id="70507-130">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="70507-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="70507-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="70507-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="70507-132">7</span><span class="sxs-lookup"><span data-stu-id="70507-132">7</span></span>|<span data-ttu-id="70507-133">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="70507-133">At least alphanumeric with symbols password required.</span></span>|



