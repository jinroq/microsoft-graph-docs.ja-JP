---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575171"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="dc328-103">androidrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="dc328-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="dc328-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc328-105">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="dc328-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="dc328-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc328-106">Members</span></span>
|<span data-ttu-id="dc328-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc328-107">Member</span></span>|<span data-ttu-id="dc328-108">値</span><span class="sxs-lookup"><span data-stu-id="dc328-108">Value</span></span>|<span data-ttu-id="dc328-109">説明</span><span class="sxs-lookup"><span data-stu-id="dc328-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc328-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="dc328-110">deviceDefault</span></span>|<span data-ttu-id="dc328-111">.0</span><span class="sxs-lookup"><span data-stu-id="dc328-111">0</span></span>|<span data-ttu-id="dc328-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="dc328-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="dc328-113">読み</span><span class="sxs-lookup"><span data-stu-id="dc328-113">alphabetic</span></span>|<span data-ttu-id="dc328-114">1 </span><span class="sxs-lookup"><span data-stu-id="dc328-114">1</span></span>|<span data-ttu-id="dc328-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="dc328-116">文字</span><span class="sxs-lookup"><span data-stu-id="dc328-116">alphanumeric</span></span>|<span data-ttu-id="dc328-117">2 </span><span class="sxs-lookup"><span data-stu-id="dc328-117">2</span></span>|<span data-ttu-id="dc328-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="dc328-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="dc328-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="dc328-120">3 </span><span class="sxs-lookup"><span data-stu-id="dc328-120">3</span></span>|<span data-ttu-id="dc328-121">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="dc328-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="dc328-122">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="dc328-122">lowSecurityBiometric</span></span>|<span data-ttu-id="dc328-123">4 </span><span class="sxs-lookup"><span data-stu-id="dc328-123">4</span></span>|<span data-ttu-id="dc328-124">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="dc328-125">数値</span><span class="sxs-lookup"><span data-stu-id="dc328-125">numeric</span></span>|<span data-ttu-id="dc328-126">5 </span><span class="sxs-lookup"><span data-stu-id="dc328-126">5</span></span>|<span data-ttu-id="dc328-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-127">Numeric password required.</span></span>|
|<span data-ttu-id="dc328-128">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="dc328-128">numericComplex</span></span>|<span data-ttu-id="dc328-129">6 </span><span class="sxs-lookup"><span data-stu-id="dc328-129">6</span></span>|<span data-ttu-id="dc328-130">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="dc328-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="dc328-131">any</span><span class="sxs-lookup"><span data-stu-id="dc328-131">any</span></span>|<span data-ttu-id="dc328-132">7 </span><span class="sxs-lookup"><span data-stu-id="dc328-132">7</span></span>|<span data-ttu-id="dc328-133">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="dc328-133">A password or pattern is required, and any is acceptable.</span></span>|



