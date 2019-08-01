---
title: androidRequiredPasswordType 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0562d059ca69358190c49fb6b518abccdc98c449
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028708"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="4a2b0-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a2b0-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="4a2b0-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a2b0-105">Android 必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="4a2b0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a2b0-106">Members</span></span>
|<span data-ttu-id="4a2b0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a2b0-107">Member</span></span>|<span data-ttu-id="4a2b0-108">値</span><span class="sxs-lookup"><span data-stu-id="4a2b0-108">Value</span></span>|<span data-ttu-id="4a2b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="4a2b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a2b0-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4a2b0-110">deviceDefault</span></span>|<span data-ttu-id="4a2b0-111">.0</span><span class="sxs-lookup"><span data-stu-id="4a2b0-111">0</span></span>|<span data-ttu-id="4a2b0-112">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="4a2b0-113">読み</span><span class="sxs-lookup"><span data-stu-id="4a2b0-113">alphabetic</span></span>|<span data-ttu-id="4a2b0-114">1-d</span><span class="sxs-lookup"><span data-stu-id="4a2b0-114">1</span></span>|<span data-ttu-id="4a2b0-115">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="4a2b0-116">文字</span><span class="sxs-lookup"><span data-stu-id="4a2b0-116">alphanumeric</span></span>|<span data-ttu-id="4a2b0-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4a2b0-117">2</span></span>|<span data-ttu-id="4a2b0-118">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="4a2b0-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4a2b0-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="4a2b0-120">1/3</span><span class="sxs-lookup"><span data-stu-id="4a2b0-120">3</span></span>|<span data-ttu-id="4a2b0-121">記号パスワードが必要な英数字。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="4a2b0-122">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="4a2b0-122">lowSecurityBiometric</span></span>|<span data-ttu-id="4a2b0-123">2/4</span><span class="sxs-lookup"><span data-stu-id="4a2b0-123">4</span></span>|<span data-ttu-id="4a2b0-124">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="4a2b0-125">数値</span><span class="sxs-lookup"><span data-stu-id="4a2b0-125">numeric</span></span>|<span data-ttu-id="4a2b0-126">5</span><span class="sxs-lookup"><span data-stu-id="4a2b0-126">5</span></span>|<span data-ttu-id="4a2b0-127">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-127">Numeric password required.</span></span>|
|<span data-ttu-id="4a2b0-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4a2b0-128">numericComplex</span></span>|<span data-ttu-id="4a2b0-129">シックス</span><span class="sxs-lookup"><span data-stu-id="4a2b0-129">6</span></span>|<span data-ttu-id="4a2b0-130">数字の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="4a2b0-131">any</span><span class="sxs-lookup"><span data-stu-id="4a2b0-131">any</span></span>|<span data-ttu-id="4a2b0-132">7</span><span class="sxs-lookup"><span data-stu-id="4a2b0-132">7</span></span>|<span data-ttu-id="4a2b0-133">パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。</span><span class="sxs-lookup"><span data-stu-id="4a2b0-133">A password or pattern is required, and any is acceptable.</span></span>|



