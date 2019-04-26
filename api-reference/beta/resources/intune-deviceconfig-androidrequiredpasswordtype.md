---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562497"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="2d9c3-103">androidrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="2d9c3-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="2d9c3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d9c3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9c3-106">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="2d9c3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2d9c3-107">Members</span></span>
|<span data-ttu-id="2d9c3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2d9c3-108">Member</span></span>|<span data-ttu-id="2d9c3-109">値</span><span class="sxs-lookup"><span data-stu-id="2d9c3-109">Value</span></span>|<span data-ttu-id="2d9c3-110">説明</span><span class="sxs-lookup"><span data-stu-id="2d9c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9c3-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="2d9c3-111">deviceDefault</span></span>|<span data-ttu-id="2d9c3-112">.0</span><span class="sxs-lookup"><span data-stu-id="2d9c3-112">0</span></span>|<span data-ttu-id="2d9c3-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="2d9c3-114">読み</span><span class="sxs-lookup"><span data-stu-id="2d9c3-114">alphabetic</span></span>|<span data-ttu-id="2d9c3-115">1 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-115">1</span></span>|<span data-ttu-id="2d9c3-116">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="2d9c3-117">文字</span><span class="sxs-lookup"><span data-stu-id="2d9c3-117">alphanumeric</span></span>|<span data-ttu-id="2d9c3-118">2 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-118">2</span></span>|<span data-ttu-id="2d9c3-119">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="2d9c3-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="2d9c3-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="2d9c3-121">3 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-121">3</span></span>|<span data-ttu-id="2d9c3-122">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="2d9c3-123">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="2d9c3-123">lowSecurityBiometric</span></span>|<span data-ttu-id="2d9c3-124">4 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-124">4</span></span>|<span data-ttu-id="2d9c3-125">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="2d9c3-126">数値</span><span class="sxs-lookup"><span data-stu-id="2d9c3-126">numeric</span></span>|<span data-ttu-id="2d9c3-127">5 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-127">5</span></span>|<span data-ttu-id="2d9c3-128">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-128">Numeric password required.</span></span>|
|<span data-ttu-id="2d9c3-129">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="2d9c3-129">numericComplex</span></span>|<span data-ttu-id="2d9c3-130">6 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-130">6</span></span>|<span data-ttu-id="2d9c3-131">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="2d9c3-132">any</span><span class="sxs-lookup"><span data-stu-id="2d9c3-132">any</span></span>|<span data-ttu-id="2d9c3-133">7 </span><span class="sxs-lookup"><span data-stu-id="2d9c3-133">7</span></span>|<span data-ttu-id="2d9c3-134">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="2d9c3-134">A password or pattern is required, and any is acceptable.</span></span>|





