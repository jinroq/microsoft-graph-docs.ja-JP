---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1845656d43ec2a8f567506ed61b5ee3bc6d8a9ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151521"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f36ee-103">androidrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="f36ee-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f36ee-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f36ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f36ee-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f36ee-106">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f36ee-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f36ee-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f36ee-107">Members</span></span>
|<span data-ttu-id="f36ee-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f36ee-108">Member</span></span>|<span data-ttu-id="f36ee-109">値</span><span class="sxs-lookup"><span data-stu-id="f36ee-109">Value</span></span>|<span data-ttu-id="f36ee-110">説明</span><span class="sxs-lookup"><span data-stu-id="f36ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f36ee-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="f36ee-111">deviceDefault</span></span>|<span data-ttu-id="f36ee-112">.0</span><span class="sxs-lookup"><span data-stu-id="f36ee-112">0</span></span>|<span data-ttu-id="f36ee-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f36ee-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f36ee-114">読み</span><span class="sxs-lookup"><span data-stu-id="f36ee-114">alphabetic</span></span>|<span data-ttu-id="f36ee-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f36ee-115">1</span></span>|<span data-ttu-id="f36ee-116">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="f36ee-117">英数字</span><span class="sxs-lookup"><span data-stu-id="f36ee-117">alphanumeric</span></span>|<span data-ttu-id="f36ee-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f36ee-118">2</span></span>|<span data-ttu-id="f36ee-119">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f36ee-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f36ee-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="f36ee-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f36ee-121">3</span></span>|<span data-ttu-id="f36ee-122">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="f36ee-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f36ee-123">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="f36ee-123">lowSecurityBiometric</span></span>|<span data-ttu-id="f36ee-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f36ee-124">4</span></span>|<span data-ttu-id="f36ee-125">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f36ee-126">numeric</span><span class="sxs-lookup"><span data-stu-id="f36ee-126">numeric</span></span>|<span data-ttu-id="f36ee-127">5</span><span class="sxs-lookup"><span data-stu-id="f36ee-127">5</span></span>|<span data-ttu-id="f36ee-128">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-128">Numeric password required.</span></span>|
|<span data-ttu-id="f36ee-129">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="f36ee-129">numericComplex</span></span>|<span data-ttu-id="f36ee-130">シックス</span><span class="sxs-lookup"><span data-stu-id="f36ee-130">6</span></span>|<span data-ttu-id="f36ee-131">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f36ee-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="f36ee-132">any</span><span class="sxs-lookup"><span data-stu-id="f36ee-132">any</span></span>|<span data-ttu-id="f36ee-133">7</span><span class="sxs-lookup"><span data-stu-id="f36ee-133">7</span></span>|<span data-ttu-id="f36ee-134">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="f36ee-134">A password or pattern is required, and any is acceptable.</span></span>|




