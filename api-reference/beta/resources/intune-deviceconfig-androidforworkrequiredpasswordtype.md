---
title: Androidforwork Requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14d6e1bf888ce2053ef1d77da36dc06395380193
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948591"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="9cbab-103">Androidforwork Requiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="9cbab-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9cbab-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cbab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cbab-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbab-106">Android 用 Android が必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="9cbab-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9cbab-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9cbab-107">Members</span></span>
|<span data-ttu-id="9cbab-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9cbab-108">Member</span></span>|<span data-ttu-id="9cbab-109">値</span><span class="sxs-lookup"><span data-stu-id="9cbab-109">Value</span></span>|<span data-ttu-id="9cbab-110">説明</span><span class="sxs-lookup"><span data-stu-id="9cbab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbab-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9cbab-111">deviceDefault</span></span>|<span data-ttu-id="9cbab-112">.0</span><span class="sxs-lookup"><span data-stu-id="9cbab-112">0</span></span>|<span data-ttu-id="9cbab-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="9cbab-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="9cbab-114">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="9cbab-114">lowSecurityBiometric</span></span>|<span data-ttu-id="9cbab-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9cbab-115">1</span></span>|<span data-ttu-id="9cbab-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9cbab-117">必須</span><span class="sxs-lookup"><span data-stu-id="9cbab-117">required</span></span>|<span data-ttu-id="9cbab-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9cbab-118">2</span></span>|<span data-ttu-id="9cbab-119">必須。</span><span class="sxs-lookup"><span data-stu-id="9cbab-119">Required.</span></span>|
|<span data-ttu-id="9cbab-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="9cbab-120">atLeastNumeric</span></span>|<span data-ttu-id="9cbab-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9cbab-121">3</span></span>|<span data-ttu-id="9cbab-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-122">At least numeric password required.</span></span>|
|<span data-ttu-id="9cbab-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9cbab-123">numericComplex</span></span>|<span data-ttu-id="9cbab-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9cbab-124">4</span></span>|<span data-ttu-id="9cbab-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="9cbab-126">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="9cbab-126">atLeastAlphabetic</span></span>|<span data-ttu-id="9cbab-127">5</span><span class="sxs-lookup"><span data-stu-id="9cbab-127">5</span></span>|<span data-ttu-id="9cbab-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9cbab-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="9cbab-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="9cbab-130">シックス</span><span class="sxs-lookup"><span data-stu-id="9cbab-130">6</span></span>|<span data-ttu-id="9cbab-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbab-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9cbab-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9cbab-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="9cbab-133">7</span><span class="sxs-lookup"><span data-stu-id="9cbab-133">7</span></span>|<span data-ttu-id="9cbab-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="9cbab-134">At least alphanumeric with symbols password required.</span></span>|




