---
title: androidRequiredPasswordType 列挙型
description: Android 必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2cfbf31bc2c263031e2e850e4caf479abb325ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988951"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="170f3-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="170f3-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="170f3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="170f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="170f3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="170f3-106">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="170f3-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="170f3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="170f3-107">Members</span></span>
|<span data-ttu-id="170f3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="170f3-108">Member</span></span>|<span data-ttu-id="170f3-109">値</span><span class="sxs-lookup"><span data-stu-id="170f3-109">Value</span></span>|<span data-ttu-id="170f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="170f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="170f3-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="170f3-111">deviceDefault</span></span>|<span data-ttu-id="170f3-112">.0</span><span class="sxs-lookup"><span data-stu-id="170f3-112">0</span></span>|<span data-ttu-id="170f3-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="170f3-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="170f3-114">読み</span><span class="sxs-lookup"><span data-stu-id="170f3-114">alphabetic</span></span>|<span data-ttu-id="170f3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="170f3-115">1</span></span>|<span data-ttu-id="170f3-116">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="170f3-117">文字</span><span class="sxs-lookup"><span data-stu-id="170f3-117">alphanumeric</span></span>|<span data-ttu-id="170f3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="170f3-118">2</span></span>|<span data-ttu-id="170f3-119">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="170f3-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="170f3-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="170f3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="170f3-121">3</span></span>|<span data-ttu-id="170f3-122">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="170f3-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="170f3-123">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="170f3-123">lowSecurityBiometric</span></span>|<span data-ttu-id="170f3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="170f3-124">4</span></span>|<span data-ttu-id="170f3-125">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="170f3-126">数値</span><span class="sxs-lookup"><span data-stu-id="170f3-126">numeric</span></span>|<span data-ttu-id="170f3-127">5</span><span class="sxs-lookup"><span data-stu-id="170f3-127">5</span></span>|<span data-ttu-id="170f3-128">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-128">Numeric password required.</span></span>|
|<span data-ttu-id="170f3-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="170f3-129">numericComplex</span></span>|<span data-ttu-id="170f3-130">シックス</span><span class="sxs-lookup"><span data-stu-id="170f3-130">6</span></span>|<span data-ttu-id="170f3-131">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="170f3-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="170f3-132">any</span><span class="sxs-lookup"><span data-stu-id="170f3-132">any</span></span>|<span data-ttu-id="170f3-133">7</span><span class="sxs-lookup"><span data-stu-id="170f3-133">7</span></span>|<span data-ttu-id="170f3-134">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="170f3-134">A password or pattern is required, and any is acceptable.</span></span>|





