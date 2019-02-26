---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255403"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="64ef7-103">androidrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="64ef7-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="64ef7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64ef7-105">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="64ef7-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="64ef7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="64ef7-106">Members</span></span>
|<span data-ttu-id="64ef7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="64ef7-107">Member</span></span>|<span data-ttu-id="64ef7-108">値</span><span class="sxs-lookup"><span data-stu-id="64ef7-108">Value</span></span>|<span data-ttu-id="64ef7-109">説明</span><span class="sxs-lookup"><span data-stu-id="64ef7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64ef7-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="64ef7-110">deviceDefault</span></span>|<span data-ttu-id="64ef7-111">.0</span><span class="sxs-lookup"><span data-stu-id="64ef7-111">0</span></span>|<span data-ttu-id="64ef7-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="64ef7-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="64ef7-113">読み</span><span class="sxs-lookup"><span data-stu-id="64ef7-113">alphabetic</span></span>|<span data-ttu-id="64ef7-114">1-d</span><span class="sxs-lookup"><span data-stu-id="64ef7-114">1</span></span>|<span data-ttu-id="64ef7-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="64ef7-116">英数字</span><span class="sxs-lookup"><span data-stu-id="64ef7-116">alphanumeric</span></span>|<span data-ttu-id="64ef7-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="64ef7-117">2</span></span>|<span data-ttu-id="64ef7-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="64ef7-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="64ef7-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="64ef7-120">1/3</span><span class="sxs-lookup"><span data-stu-id="64ef7-120">3</span></span>|<span data-ttu-id="64ef7-121">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="64ef7-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="64ef7-122">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="64ef7-122">lowSecurityBiometric</span></span>|<span data-ttu-id="64ef7-123">2/4</span><span class="sxs-lookup"><span data-stu-id="64ef7-123">4</span></span>|<span data-ttu-id="64ef7-124">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="64ef7-125">numeric</span><span class="sxs-lookup"><span data-stu-id="64ef7-125">numeric</span></span>|<span data-ttu-id="64ef7-126">5</span><span class="sxs-lookup"><span data-stu-id="64ef7-126">5</span></span>|<span data-ttu-id="64ef7-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-127">Numeric password required.</span></span>|
|<span data-ttu-id="64ef7-128">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="64ef7-128">numericComplex</span></span>|<span data-ttu-id="64ef7-129">シックス</span><span class="sxs-lookup"><span data-stu-id="64ef7-129">6</span></span>|<span data-ttu-id="64ef7-130">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="64ef7-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="64ef7-131">any</span><span class="sxs-lookup"><span data-stu-id="64ef7-131">any</span></span>|<span data-ttu-id="64ef7-132">7</span><span class="sxs-lookup"><span data-stu-id="64ef7-132">7</span></span>|<span data-ttu-id="64ef7-133">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="64ef7-133">A password or pattern is required, and any is acceptable.</span></span>|



