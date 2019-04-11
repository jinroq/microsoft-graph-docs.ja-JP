---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782073"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="bcd53-103">androidrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="bcd53-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="bcd53-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcd53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcd53-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcd53-106">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="bcd53-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="bcd53-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bcd53-107">Members</span></span>
|<span data-ttu-id="bcd53-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bcd53-108">Member</span></span>|<span data-ttu-id="bcd53-109">値</span><span class="sxs-lookup"><span data-stu-id="bcd53-109">Value</span></span>|<span data-ttu-id="bcd53-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcd53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcd53-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="bcd53-111">deviceDefault</span></span>|<span data-ttu-id="bcd53-112">.0</span><span class="sxs-lookup"><span data-stu-id="bcd53-112">0</span></span>|<span data-ttu-id="bcd53-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="bcd53-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="bcd53-114">読み</span><span class="sxs-lookup"><span data-stu-id="bcd53-114">alphabetic</span></span>|<span data-ttu-id="bcd53-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bcd53-115">1</span></span>|<span data-ttu-id="bcd53-116">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="bcd53-117">文字</span><span class="sxs-lookup"><span data-stu-id="bcd53-117">alphanumeric</span></span>|<span data-ttu-id="bcd53-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bcd53-118">2</span></span>|<span data-ttu-id="bcd53-119">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="bcd53-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="bcd53-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="bcd53-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bcd53-121">3</span></span>|<span data-ttu-id="bcd53-122">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="bcd53-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="bcd53-123">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="bcd53-123">lowSecurityBiometric</span></span>|<span data-ttu-id="bcd53-124">2/4</span><span class="sxs-lookup"><span data-stu-id="bcd53-124">4</span></span>|<span data-ttu-id="bcd53-125">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="bcd53-126">数値</span><span class="sxs-lookup"><span data-stu-id="bcd53-126">numeric</span></span>|<span data-ttu-id="bcd53-127">5</span><span class="sxs-lookup"><span data-stu-id="bcd53-127">5</span></span>|<span data-ttu-id="bcd53-128">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-128">Numeric password required.</span></span>|
|<span data-ttu-id="bcd53-129">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="bcd53-129">numericComplex</span></span>|<span data-ttu-id="bcd53-130">シックス</span><span class="sxs-lookup"><span data-stu-id="bcd53-130">6</span></span>|<span data-ttu-id="bcd53-131">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd53-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="bcd53-132">any</span><span class="sxs-lookup"><span data-stu-id="bcd53-132">any</span></span>|<span data-ttu-id="bcd53-133">7</span><span class="sxs-lookup"><span data-stu-id="bcd53-133">7</span></span>|<span data-ttu-id="bcd53-134">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="bcd53-134">A password or pattern is required, and any is acceptable.</span></span>|





