---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c85466cf722848efa684fc7b5643293d49de2459
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964089"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="136da-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="136da-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="136da-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="136da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="136da-105">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="136da-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="136da-106">Members</span></span>
|<span data-ttu-id="136da-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="136da-107">Member</span></span>|<span data-ttu-id="136da-108">値</span><span class="sxs-lookup"><span data-stu-id="136da-108">Value</span></span>|<span data-ttu-id="136da-109">説明</span><span class="sxs-lookup"><span data-stu-id="136da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="136da-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="136da-110">deviceDefault</span></span>|<span data-ttu-id="136da-111">0</span><span class="sxs-lookup"><span data-stu-id="136da-111">0</span></span>|<span data-ttu-id="136da-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="136da-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="136da-113">アルファベット</span><span class="sxs-lookup"><span data-stu-id="136da-113">alphabetic</span></span>|<span data-ttu-id="136da-114">1</span><span class="sxs-lookup"><span data-stu-id="136da-114">1</span></span>|<span data-ttu-id="136da-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="136da-116">英数字</span><span class="sxs-lookup"><span data-stu-id="136da-116">alphanumeric</span></span>|<span data-ttu-id="136da-117">2</span><span class="sxs-lookup"><span data-stu-id="136da-117">2</span></span>|<span data-ttu-id="136da-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="136da-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="136da-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="136da-120">3</span><span class="sxs-lookup"><span data-stu-id="136da-120">3</span></span>|<span data-ttu-id="136da-121">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="136da-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="136da-122">lowSecurityBiometric</span></span>|<span data-ttu-id="136da-123">4</span><span class="sxs-lookup"><span data-stu-id="136da-123">4</span></span>|<span data-ttu-id="136da-124">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="136da-125">numeric</span><span class="sxs-lookup"><span data-stu-id="136da-125">numeric</span></span>|<span data-ttu-id="136da-126">5</span><span class="sxs-lookup"><span data-stu-id="136da-126">5</span></span>|<span data-ttu-id="136da-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-127">Numeric password required.</span></span>|
|<span data-ttu-id="136da-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="136da-128">numericComplex</span></span>|<span data-ttu-id="136da-129">6</span><span class="sxs-lookup"><span data-stu-id="136da-129">6</span></span>|<span data-ttu-id="136da-130">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="136da-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="136da-131">any</span><span class="sxs-lookup"><span data-stu-id="136da-131">any</span></span>|<span data-ttu-id="136da-132">7</span><span class="sxs-lookup"><span data-stu-id="136da-132">7</span></span>|<span data-ttu-id="136da-133">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="136da-133">A password or pattern is required, and any is acceptable.</span></span>|



