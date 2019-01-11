---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06a89256920f143af923e6a3949e61843fa7aa00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814421"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="e6c63-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e6c63-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="e6c63-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6c63-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6c63-105">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="e6c63-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6c63-106">Members</span></span>
|<span data-ttu-id="e6c63-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6c63-107">Member</span></span>|<span data-ttu-id="e6c63-108">値</span><span class="sxs-lookup"><span data-stu-id="e6c63-108">Value</span></span>|<span data-ttu-id="e6c63-109">説明</span><span class="sxs-lookup"><span data-stu-id="e6c63-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c63-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e6c63-110">deviceDefault</span></span>|<span data-ttu-id="e6c63-111">0</span><span class="sxs-lookup"><span data-stu-id="e6c63-111">0</span></span>|<span data-ttu-id="e6c63-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="e6c63-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="e6c63-113">アルファベット</span><span class="sxs-lookup"><span data-stu-id="e6c63-113">alphabetic</span></span>|<span data-ttu-id="e6c63-114">1</span><span class="sxs-lookup"><span data-stu-id="e6c63-114">1</span></span>|<span data-ttu-id="e6c63-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="e6c63-116">英数字</span><span class="sxs-lookup"><span data-stu-id="e6c63-116">alphanumeric</span></span>|<span data-ttu-id="e6c63-117">2</span><span class="sxs-lookup"><span data-stu-id="e6c63-117">2</span></span>|<span data-ttu-id="e6c63-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="e6c63-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e6c63-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="e6c63-120">3</span><span class="sxs-lookup"><span data-stu-id="e6c63-120">3</span></span>|<span data-ttu-id="e6c63-121">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="e6c63-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="e6c63-122">lowSecurityBiometric</span></span>|<span data-ttu-id="e6c63-123">4</span><span class="sxs-lookup"><span data-stu-id="e6c63-123">4</span></span>|<span data-ttu-id="e6c63-124">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e6c63-125">numeric</span><span class="sxs-lookup"><span data-stu-id="e6c63-125">numeric</span></span>|<span data-ttu-id="e6c63-126">5</span><span class="sxs-lookup"><span data-stu-id="e6c63-126">5</span></span>|<span data-ttu-id="e6c63-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-127">Numeric password required.</span></span>|
|<span data-ttu-id="e6c63-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="e6c63-128">numericComplex</span></span>|<span data-ttu-id="e6c63-129">6</span><span class="sxs-lookup"><span data-stu-id="e6c63-129">6</span></span>|<span data-ttu-id="e6c63-130">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="e6c63-131">any</span><span class="sxs-lookup"><span data-stu-id="e6c63-131">any</span></span>|<span data-ttu-id="e6c63-132">7</span><span class="sxs-lookup"><span data-stu-id="e6c63-132">7</span></span>|<span data-ttu-id="e6c63-133">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="e6c63-133">A password or pattern is required, and any is acceptable.</span></span>|



