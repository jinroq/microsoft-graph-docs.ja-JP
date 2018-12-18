---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: e9b757dc86bf71462f7f987cedfcd9e04497880e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349218"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="a0aa1-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a0aa1-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a0aa1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0aa1-105">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="a0aa1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0aa1-106">Members</span></span>
|<span data-ttu-id="a0aa1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0aa1-107">Member</span></span>|<span data-ttu-id="a0aa1-108">値</span><span class="sxs-lookup"><span data-stu-id="a0aa1-108">Value</span></span>|<span data-ttu-id="a0aa1-109">説明</span><span class="sxs-lookup"><span data-stu-id="a0aa1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0aa1-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a0aa1-110">deviceDefault</span></span>|<span data-ttu-id="a0aa1-111">0</span><span class="sxs-lookup"><span data-stu-id="a0aa1-111">0</span></span>|<span data-ttu-id="a0aa1-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="a0aa1-113">アルファベット</span><span class="sxs-lookup"><span data-stu-id="a0aa1-113">alphabetic</span></span>|<span data-ttu-id="a0aa1-114">1</span><span class="sxs-lookup"><span data-stu-id="a0aa1-114">1</span></span>|<span data-ttu-id="a0aa1-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="a0aa1-116">英数字</span><span class="sxs-lookup"><span data-stu-id="a0aa1-116">alphanumeric</span></span>|<span data-ttu-id="a0aa1-117">2</span><span class="sxs-lookup"><span data-stu-id="a0aa1-117">2</span></span>|<span data-ttu-id="a0aa1-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="a0aa1-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a0aa1-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="a0aa1-120">3</span><span class="sxs-lookup"><span data-stu-id="a0aa1-120">3</span></span>|<span data-ttu-id="a0aa1-121">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="a0aa1-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a0aa1-122">lowSecurityBiometric</span></span>|<span data-ttu-id="a0aa1-123">4</span><span class="sxs-lookup"><span data-stu-id="a0aa1-123">4</span></span>|<span data-ttu-id="a0aa1-124">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a0aa1-125">numeric</span><span class="sxs-lookup"><span data-stu-id="a0aa1-125">numeric</span></span>|<span data-ttu-id="a0aa1-126">5</span><span class="sxs-lookup"><span data-stu-id="a0aa1-126">5</span></span>|<span data-ttu-id="a0aa1-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-127">Numeric password required.</span></span>|
|<span data-ttu-id="a0aa1-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a0aa1-128">numericComplex</span></span>|<span data-ttu-id="a0aa1-129">6</span><span class="sxs-lookup"><span data-stu-id="a0aa1-129">6</span></span>|<span data-ttu-id="a0aa1-130">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="a0aa1-131">any</span><span class="sxs-lookup"><span data-stu-id="a0aa1-131">any</span></span>|<span data-ttu-id="a0aa1-132">7</span><span class="sxs-lookup"><span data-stu-id="a0aa1-132">7</span></span>|<span data-ttu-id="a0aa1-133">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="a0aa1-133">A password or pattern is required, and any is acceptable.</span></span>|



