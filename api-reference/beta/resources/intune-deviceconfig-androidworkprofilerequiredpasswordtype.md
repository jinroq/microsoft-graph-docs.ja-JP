---
title: androidWorkProfileRequiredPasswordType 列挙型
description: Android の作業プロファイルに必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5553329c8519aa40eb4f1ee3ee3cb48f66c06995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011639"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="8fa99-103">androidWorkProfileRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8fa99-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="8fa99-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fa99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fa99-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fa99-106">Android の作業プロファイルに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="8fa99-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="8fa99-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8fa99-107">Members</span></span>
|<span data-ttu-id="8fa99-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8fa99-108">Member</span></span>|<span data-ttu-id="8fa99-109">値</span><span class="sxs-lookup"><span data-stu-id="8fa99-109">Value</span></span>|<span data-ttu-id="8fa99-110">説明</span><span class="sxs-lookup"><span data-stu-id="8fa99-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fa99-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8fa99-111">deviceDefault</span></span>|<span data-ttu-id="8fa99-112">.0</span><span class="sxs-lookup"><span data-stu-id="8fa99-112">0</span></span>|<span data-ttu-id="8fa99-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="8fa99-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="8fa99-114">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="8fa99-114">lowSecurityBiometric</span></span>|<span data-ttu-id="8fa99-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8fa99-115">1</span></span>|<span data-ttu-id="8fa99-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="8fa99-117">必須</span><span class="sxs-lookup"><span data-stu-id="8fa99-117">required</span></span>|<span data-ttu-id="8fa99-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8fa99-118">2</span></span>|<span data-ttu-id="8fa99-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-119">Required.</span></span>|
|<span data-ttu-id="8fa99-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="8fa99-120">atLeastNumeric</span></span>|<span data-ttu-id="8fa99-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8fa99-121">3</span></span>|<span data-ttu-id="8fa99-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-122">At least numeric password required.</span></span>|
|<span data-ttu-id="8fa99-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="8fa99-123">numericComplex</span></span>|<span data-ttu-id="8fa99-124">2/4</span><span class="sxs-lookup"><span data-stu-id="8fa99-124">4</span></span>|<span data-ttu-id="8fa99-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="8fa99-126">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="8fa99-126">atLeastAlphabetic</span></span>|<span data-ttu-id="8fa99-127">5</span><span class="sxs-lookup"><span data-stu-id="8fa99-127">5</span></span>|<span data-ttu-id="8fa99-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="8fa99-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="8fa99-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="8fa99-130">シックス</span><span class="sxs-lookup"><span data-stu-id="8fa99-130">6</span></span>|<span data-ttu-id="8fa99-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="8fa99-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="8fa99-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="8fa99-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="8fa99-133">7</span><span class="sxs-lookup"><span data-stu-id="8fa99-133">7</span></span>|<span data-ttu-id="8fa99-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="8fa99-134">At least alphanumeric with symbols password required.</span></span>|





