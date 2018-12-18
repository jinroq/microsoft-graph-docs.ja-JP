---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: e08df0ef61b6d60227f9dec2382a57884c2f4bdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355987"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f7f14-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7f14-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f7f14-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7f14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7f14-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7f14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7f14-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7f14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7f14-107">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-107">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="f7f14-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7f14-108">Members</span></span>
|<span data-ttu-id="f7f14-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7f14-109">Member</span></span>|<span data-ttu-id="f7f14-110">値</span><span class="sxs-lookup"><span data-stu-id="f7f14-110">Value</span></span>|<span data-ttu-id="f7f14-111">説明</span><span class="sxs-lookup"><span data-stu-id="f7f14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f14-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f7f14-112">deviceDefault</span></span>|<span data-ttu-id="f7f14-113">0</span><span class="sxs-lookup"><span data-stu-id="f7f14-113">0</span></span>|<span data-ttu-id="f7f14-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="f7f14-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f7f14-115">アルファベット</span><span class="sxs-lookup"><span data-stu-id="f7f14-115">alphabetic</span></span>|<span data-ttu-id="f7f14-116">1</span><span class="sxs-lookup"><span data-stu-id="f7f14-116">1</span></span>|<span data-ttu-id="f7f14-117">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="f7f14-118">英数字</span><span class="sxs-lookup"><span data-stu-id="f7f14-118">alphanumeric</span></span>|<span data-ttu-id="f7f14-119">2</span><span class="sxs-lookup"><span data-stu-id="f7f14-119">2</span></span>|<span data-ttu-id="f7f14-120">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f7f14-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f7f14-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="f7f14-122">3</span><span class="sxs-lookup"><span data-stu-id="f7f14-122">3</span></span>|<span data-ttu-id="f7f14-123">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f7f14-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="f7f14-124">lowSecurityBiometric</span></span>|<span data-ttu-id="f7f14-125">4</span><span class="sxs-lookup"><span data-stu-id="f7f14-125">4</span></span>|<span data-ttu-id="f7f14-126">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f7f14-127">numeric</span><span class="sxs-lookup"><span data-stu-id="f7f14-127">numeric</span></span>|<span data-ttu-id="f7f14-128">5</span><span class="sxs-lookup"><span data-stu-id="f7f14-128">5</span></span>|<span data-ttu-id="f7f14-129">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-129">Numeric password required.</span></span>|
|<span data-ttu-id="f7f14-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f7f14-130">numericComplex</span></span>|<span data-ttu-id="f7f14-131">6</span><span class="sxs-lookup"><span data-stu-id="f7f14-131">6</span></span>|<span data-ttu-id="f7f14-132">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="f7f14-133">any</span><span class="sxs-lookup"><span data-stu-id="f7f14-133">any</span></span>|<span data-ttu-id="f7f14-134">7</span><span class="sxs-lookup"><span data-stu-id="f7f14-134">7</span></span>|<span data-ttu-id="f7f14-135">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="f7f14-135">A password or pattern is required, and any is acceptable.</span></span>|





