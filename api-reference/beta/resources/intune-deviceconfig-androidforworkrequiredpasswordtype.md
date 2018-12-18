---
title: androidForWorkRequiredPasswordType 列挙型
description: Android の作業には、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: cefb41dea7a92f1b1a640d8c9bf701a321ad9ead
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357282"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="efd3c-103">androidForWorkRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="efd3c-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="efd3c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="efd3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efd3c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efd3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd3c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="efd3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efd3c-107">Android の作業には、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="efd3c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="efd3c-108">Members</span></span>
|<span data-ttu-id="efd3c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="efd3c-109">Member</span></span>|<span data-ttu-id="efd3c-110">値</span><span class="sxs-lookup"><span data-stu-id="efd3c-110">Value</span></span>|<span data-ttu-id="efd3c-111">説明</span><span class="sxs-lookup"><span data-stu-id="efd3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd3c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="efd3c-112">deviceDefault</span></span>|<span data-ttu-id="efd3c-113">0</span><span class="sxs-lookup"><span data-stu-id="efd3c-113">0</span></span>|<span data-ttu-id="efd3c-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="efd3c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="efd3c-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="efd3c-115">lowSecurityBiometric</span></span>|<span data-ttu-id="efd3c-116">1</span><span class="sxs-lookup"><span data-stu-id="efd3c-116">1</span></span>|<span data-ttu-id="efd3c-117">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="efd3c-118">必須</span><span class="sxs-lookup"><span data-stu-id="efd3c-118">required</span></span>|<span data-ttu-id="efd3c-119">2</span><span class="sxs-lookup"><span data-stu-id="efd3c-119">2</span></span>|<span data-ttu-id="efd3c-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-120">Required.</span></span>|
|<span data-ttu-id="efd3c-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="efd3c-121">atLeastNumeric</span></span>|<span data-ttu-id="efd3c-122">3</span><span class="sxs-lookup"><span data-stu-id="efd3c-122">3</span></span>|<span data-ttu-id="efd3c-123">数値以上のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-123">At least numeric password required.</span></span>|
|<span data-ttu-id="efd3c-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="efd3c-124">numericComplex</span></span>|<span data-ttu-id="efd3c-125">4</span><span class="sxs-lookup"><span data-stu-id="efd3c-125">4</span></span>|<span data-ttu-id="efd3c-126">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="efd3c-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="efd3c-127">atLeastAlphabetic</span></span>|<span data-ttu-id="efd3c-128">5</span><span class="sxs-lookup"><span data-stu-id="efd3c-128">5</span></span>|<span data-ttu-id="efd3c-129">少なくともアルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="efd3c-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="efd3c-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="efd3c-131">6</span><span class="sxs-lookup"><span data-stu-id="efd3c-131">6</span></span>|<span data-ttu-id="efd3c-132">以上の英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="efd3c-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="efd3c-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="efd3c-134">7</span><span class="sxs-lookup"><span data-stu-id="efd3c-134">7</span></span>|<span data-ttu-id="efd3c-135">少なくとも文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="efd3c-135">At least alphanumeric with symbols password required.</span></span>|





