---
title: Androidforwork Requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78e9a5dc041330fb625568f5de1efeabaac3a833
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334529"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="88db7-103">Androidforwork Requiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="88db7-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="88db7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88db7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88db7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88db7-106">Android 用 Android が必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="88db7-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="88db7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="88db7-107">Members</span></span>
|<span data-ttu-id="88db7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="88db7-108">Member</span></span>|<span data-ttu-id="88db7-109">値</span><span class="sxs-lookup"><span data-stu-id="88db7-109">Value</span></span>|<span data-ttu-id="88db7-110">説明</span><span class="sxs-lookup"><span data-stu-id="88db7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88db7-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="88db7-111">deviceDefault</span></span>|<span data-ttu-id="88db7-112">.0</span><span class="sxs-lookup"><span data-stu-id="88db7-112">0</span></span>|<span data-ttu-id="88db7-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="88db7-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="88db7-114">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="88db7-114">lowSecurityBiometric</span></span>|<span data-ttu-id="88db7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="88db7-115">1</span></span>|<span data-ttu-id="88db7-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="88db7-117">必須</span><span class="sxs-lookup"><span data-stu-id="88db7-117">required</span></span>|<span data-ttu-id="88db7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="88db7-118">2</span></span>|<span data-ttu-id="88db7-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="88db7-119">Required.</span></span>|
|<span data-ttu-id="88db7-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="88db7-120">atLeastNumeric</span></span>|<span data-ttu-id="88db7-121">1/3</span><span class="sxs-lookup"><span data-stu-id="88db7-121">3</span></span>|<span data-ttu-id="88db7-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-122">At least numeric password required.</span></span>|
|<span data-ttu-id="88db7-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="88db7-123">numericComplex</span></span>|<span data-ttu-id="88db7-124">2/4</span><span class="sxs-lookup"><span data-stu-id="88db7-124">4</span></span>|<span data-ttu-id="88db7-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="88db7-126">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="88db7-126">atLeastAlphabetic</span></span>|<span data-ttu-id="88db7-127">5</span><span class="sxs-lookup"><span data-stu-id="88db7-127">5</span></span>|<span data-ttu-id="88db7-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="88db7-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="88db7-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="88db7-130">シックス</span><span class="sxs-lookup"><span data-stu-id="88db7-130">6</span></span>|<span data-ttu-id="88db7-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="88db7-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="88db7-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="88db7-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="88db7-133">7</span><span class="sxs-lookup"><span data-stu-id="88db7-133">7</span></span>|<span data-ttu-id="88db7-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="88db7-134">At least alphanumeric with symbols password required.</span></span>|



