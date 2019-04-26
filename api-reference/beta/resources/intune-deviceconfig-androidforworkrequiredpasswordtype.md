---
title: androidforwork requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bfdca6204bd1745fc9a8350309e51cec2a8a718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556138"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="c8a4e-103">androidforwork requiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="c8a4e-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c8a4e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8a4e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8a4e-106">Android 用 Android が必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c8a4e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8a4e-107">Members</span></span>
|<span data-ttu-id="c8a4e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8a4e-108">Member</span></span>|<span data-ttu-id="c8a4e-109">値</span><span class="sxs-lookup"><span data-stu-id="c8a4e-109">Value</span></span>|<span data-ttu-id="c8a4e-110">説明</span><span class="sxs-lookup"><span data-stu-id="c8a4e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a4e-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="c8a4e-111">deviceDefault</span></span>|<span data-ttu-id="c8a4e-112">.0</span><span class="sxs-lookup"><span data-stu-id="c8a4e-112">0</span></span>|<span data-ttu-id="c8a4e-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c8a4e-114">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="c8a4e-114">lowSecurityBiometric</span></span>|<span data-ttu-id="c8a4e-115">1 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-115">1</span></span>|<span data-ttu-id="c8a4e-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c8a4e-117">必須</span><span class="sxs-lookup"><span data-stu-id="c8a4e-117">required</span></span>|<span data-ttu-id="c8a4e-118">2 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-118">2</span></span>|<span data-ttu-id="c8a4e-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-119">Required.</span></span>|
|<span data-ttu-id="c8a4e-120">atleastnumeric</span><span class="sxs-lookup"><span data-stu-id="c8a4e-120">atLeastNumeric</span></span>|<span data-ttu-id="c8a4e-121">3 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-121">3</span></span>|<span data-ttu-id="c8a4e-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-122">At least numeric password required.</span></span>|
|<span data-ttu-id="c8a4e-123">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="c8a4e-123">numericComplex</span></span>|<span data-ttu-id="c8a4e-124">4 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-124">4</span></span>|<span data-ttu-id="c8a4e-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="c8a4e-126">atall stアルファベット</span><span class="sxs-lookup"><span data-stu-id="c8a4e-126">atLeastAlphabetic</span></span>|<span data-ttu-id="c8a4e-127">5 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-127">5</span></span>|<span data-ttu-id="c8a4e-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c8a4e-129">atleastalphanumeric</span><span class="sxs-lookup"><span data-stu-id="c8a4e-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="c8a4e-130">6 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-130">6</span></span>|<span data-ttu-id="c8a4e-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c8a4e-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c8a4e-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="c8a4e-133">7 </span><span class="sxs-lookup"><span data-stu-id="c8a4e-133">7</span></span>|<span data-ttu-id="c8a4e-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="c8a4e-134">At least alphanumeric with symbols password required.</span></span>|





