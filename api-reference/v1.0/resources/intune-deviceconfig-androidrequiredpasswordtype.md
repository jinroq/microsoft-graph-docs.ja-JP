---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
ms.openlocfilehash: f4f95308791aa443b6eb4b4fd38c70fe2d47b4b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023306"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="0030c-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0030c-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0030c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0030c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0030c-105">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="0030c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0030c-106">Members</span></span>
|<span data-ttu-id="0030c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0030c-107">Member</span></span>|<span data-ttu-id="0030c-108">値</span><span class="sxs-lookup"><span data-stu-id="0030c-108">Value</span></span>|<span data-ttu-id="0030c-109">説明</span><span class="sxs-lookup"><span data-stu-id="0030c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0030c-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0030c-110">deviceDefault</span></span>|<span data-ttu-id="0030c-111">0</span><span class="sxs-lookup"><span data-stu-id="0030c-111">0</span></span>|<span data-ttu-id="0030c-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="0030c-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="0030c-113">アルファベット</span><span class="sxs-lookup"><span data-stu-id="0030c-113">alphabetic</span></span>|<span data-ttu-id="0030c-114">1</span><span class="sxs-lookup"><span data-stu-id="0030c-114">1</span></span>|<span data-ttu-id="0030c-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="0030c-116">英数字</span><span class="sxs-lookup"><span data-stu-id="0030c-116">alphanumeric</span></span>|<span data-ttu-id="0030c-117">2</span><span class="sxs-lookup"><span data-stu-id="0030c-117">2</span></span>|<span data-ttu-id="0030c-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="0030c-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="0030c-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="0030c-120">3</span><span class="sxs-lookup"><span data-stu-id="0030c-120">3</span></span>|<span data-ttu-id="0030c-121">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="0030c-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="0030c-122">lowSecurityBiometric</span></span>|<span data-ttu-id="0030c-123">4</span><span class="sxs-lookup"><span data-stu-id="0030c-123">4</span></span>|<span data-ttu-id="0030c-124">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0030c-125">numeric</span><span class="sxs-lookup"><span data-stu-id="0030c-125">numeric</span></span>|<span data-ttu-id="0030c-126">5</span><span class="sxs-lookup"><span data-stu-id="0030c-126">5</span></span>|<span data-ttu-id="0030c-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-127">Numeric password required.</span></span>|
|<span data-ttu-id="0030c-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="0030c-128">numericComplex</span></span>|<span data-ttu-id="0030c-129">6</span><span class="sxs-lookup"><span data-stu-id="0030c-129">6</span></span>|<span data-ttu-id="0030c-130">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="0030c-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="0030c-131">any</span><span class="sxs-lookup"><span data-stu-id="0030c-131">any</span></span>|<span data-ttu-id="0030c-132">7</span><span class="sxs-lookup"><span data-stu-id="0030c-132">7</span></span>|<span data-ttu-id="0030c-133">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="0030c-133">A password or pattern is required, and any is acceptable.</span></span>|



