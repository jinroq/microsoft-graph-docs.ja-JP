---
title: androidRequiredPasswordType 列挙型
description: Android 必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9112074842e3dc661786acfa6c6c223aa5fe225b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334375"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="3497c-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3497c-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="3497c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3497c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3497c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3497c-106">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="3497c-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3497c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3497c-107">Members</span></span>
|<span data-ttu-id="3497c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3497c-108">Member</span></span>|<span data-ttu-id="3497c-109">値</span><span class="sxs-lookup"><span data-stu-id="3497c-109">Value</span></span>|<span data-ttu-id="3497c-110">説明</span><span class="sxs-lookup"><span data-stu-id="3497c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3497c-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3497c-111">deviceDefault</span></span>|<span data-ttu-id="3497c-112">.0</span><span class="sxs-lookup"><span data-stu-id="3497c-112">0</span></span>|<span data-ttu-id="3497c-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="3497c-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="3497c-114">読み</span><span class="sxs-lookup"><span data-stu-id="3497c-114">alphabetic</span></span>|<span data-ttu-id="3497c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3497c-115">1</span></span>|<span data-ttu-id="3497c-116">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="3497c-117">文字</span><span class="sxs-lookup"><span data-stu-id="3497c-117">alphanumeric</span></span>|<span data-ttu-id="3497c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3497c-118">2</span></span>|<span data-ttu-id="3497c-119">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="3497c-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3497c-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="3497c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3497c-121">3</span></span>|<span data-ttu-id="3497c-122">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="3497c-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="3497c-123">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="3497c-123">lowSecurityBiometric</span></span>|<span data-ttu-id="3497c-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3497c-124">4</span></span>|<span data-ttu-id="3497c-125">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3497c-126">数値</span><span class="sxs-lookup"><span data-stu-id="3497c-126">numeric</span></span>|<span data-ttu-id="3497c-127">5</span><span class="sxs-lookup"><span data-stu-id="3497c-127">5</span></span>|<span data-ttu-id="3497c-128">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-128">Numeric password required.</span></span>|
|<span data-ttu-id="3497c-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3497c-129">numericComplex</span></span>|<span data-ttu-id="3497c-130">シックス</span><span class="sxs-lookup"><span data-stu-id="3497c-130">6</span></span>|<span data-ttu-id="3497c-131">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="3497c-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="3497c-132">any</span><span class="sxs-lookup"><span data-stu-id="3497c-132">any</span></span>|<span data-ttu-id="3497c-133">7</span><span class="sxs-lookup"><span data-stu-id="3497c-133">7</span></span>|<span data-ttu-id="3497c-134">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="3497c-134">A password or pattern is required, and any is acceptable.</span></span>|



