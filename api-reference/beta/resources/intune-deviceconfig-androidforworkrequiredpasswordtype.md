---
title: Androidforwork Requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab11ed4951fb61e96afc55381986e83fad7ce440
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991059"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="a32c8-103">Androidforwork Requiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="a32c8-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a32c8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a32c8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a32c8-106">Android 用 Android が必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="a32c8-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a32c8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a32c8-107">Members</span></span>
|<span data-ttu-id="a32c8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a32c8-108">Member</span></span>|<span data-ttu-id="a32c8-109">値</span><span class="sxs-lookup"><span data-stu-id="a32c8-109">Value</span></span>|<span data-ttu-id="a32c8-110">説明</span><span class="sxs-lookup"><span data-stu-id="a32c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a32c8-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a32c8-111">deviceDefault</span></span>|<span data-ttu-id="a32c8-112">.0</span><span class="sxs-lookup"><span data-stu-id="a32c8-112">0</span></span>|<span data-ttu-id="a32c8-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="a32c8-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a32c8-114">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="a32c8-114">lowSecurityBiometric</span></span>|<span data-ttu-id="a32c8-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a32c8-115">1</span></span>|<span data-ttu-id="a32c8-116">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a32c8-117">必須</span><span class="sxs-lookup"><span data-stu-id="a32c8-117">required</span></span>|<span data-ttu-id="a32c8-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a32c8-118">2</span></span>|<span data-ttu-id="a32c8-119">必須です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-119">Required.</span></span>|
|<span data-ttu-id="a32c8-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="a32c8-120">atLeastNumeric</span></span>|<span data-ttu-id="a32c8-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a32c8-121">3</span></span>|<span data-ttu-id="a32c8-122">少なくとも数値のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-122">At least numeric password required.</span></span>|
|<span data-ttu-id="a32c8-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a32c8-123">numericComplex</span></span>|<span data-ttu-id="a32c8-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a32c8-124">4</span></span>|<span data-ttu-id="a32c8-125">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="a32c8-126">Atall Stアルファベット</span><span class="sxs-lookup"><span data-stu-id="a32c8-126">atLeastAlphabetic</span></span>|<span data-ttu-id="a32c8-127">5</span><span class="sxs-lookup"><span data-stu-id="a32c8-127">5</span></span>|<span data-ttu-id="a32c8-128">少なくとも英字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a32c8-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="a32c8-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="a32c8-130">シックス</span><span class="sxs-lookup"><span data-stu-id="a32c8-130">6</span></span>|<span data-ttu-id="a32c8-131">少なくとも英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a32c8-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a32c8-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a32c8-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="a32c8-133">7</span><span class="sxs-lookup"><span data-stu-id="a32c8-133">7</span></span>|<span data-ttu-id="a32c8-134">記号パスワードが必要な、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="a32c8-134">At least alphanumeric with symbols password required.</span></span>|





