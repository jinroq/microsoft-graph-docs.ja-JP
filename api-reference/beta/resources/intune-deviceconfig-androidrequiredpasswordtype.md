---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eebc6b0ad6eed346927fd48a2dc1f82b5e529b28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392914"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="e8a18-103">androidRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e8a18-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="e8a18-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8a18-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8a18-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8a18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8a18-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8a18-107">Android では、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e8a18-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8a18-108">Members</span></span>
|<span data-ttu-id="e8a18-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8a18-109">Member</span></span>|<span data-ttu-id="e8a18-110">値</span><span class="sxs-lookup"><span data-stu-id="e8a18-110">Value</span></span>|<span data-ttu-id="e8a18-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8a18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8a18-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e8a18-112">deviceDefault</span></span>|<span data-ttu-id="e8a18-113">0</span><span class="sxs-lookup"><span data-stu-id="e8a18-113">0</span></span>|<span data-ttu-id="e8a18-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="e8a18-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e8a18-115">アルファベット</span><span class="sxs-lookup"><span data-stu-id="e8a18-115">alphabetic</span></span>|<span data-ttu-id="e8a18-116">1</span><span class="sxs-lookup"><span data-stu-id="e8a18-116">1</span></span>|<span data-ttu-id="e8a18-117">アルファベットのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="e8a18-118">英数字</span><span class="sxs-lookup"><span data-stu-id="e8a18-118">alphanumeric</span></span>|<span data-ttu-id="e8a18-119">2</span><span class="sxs-lookup"><span data-stu-id="e8a18-119">2</span></span>|<span data-ttu-id="e8a18-120">英数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="e8a18-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e8a18-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="e8a18-122">3</span><span class="sxs-lookup"><span data-stu-id="e8a18-122">3</span></span>|<span data-ttu-id="e8a18-123">文字の英数字の記号のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="e8a18-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="e8a18-124">lowSecurityBiometric</span></span>|<span data-ttu-id="e8a18-125">4</span><span class="sxs-lookup"><span data-stu-id="e8a18-125">4</span></span>|<span data-ttu-id="e8a18-126">低レベルのセキュリティ ベースの生体認証パスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e8a18-127">numeric</span><span class="sxs-lookup"><span data-stu-id="e8a18-127">numeric</span></span>|<span data-ttu-id="e8a18-128">5</span><span class="sxs-lookup"><span data-stu-id="e8a18-128">5</span></span>|<span data-ttu-id="e8a18-129">数字のパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-129">Numeric password required.</span></span>|
|<span data-ttu-id="e8a18-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="e8a18-130">numericComplex</span></span>|<span data-ttu-id="e8a18-131">6</span><span class="sxs-lookup"><span data-stu-id="e8a18-131">6</span></span>|<span data-ttu-id="e8a18-132">数値の複雑なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="e8a18-133">any</span><span class="sxs-lookup"><span data-stu-id="e8a18-133">any</span></span>|<span data-ttu-id="e8a18-134">7</span><span class="sxs-lookup"><span data-stu-id="e8a18-134">7</span></span>|<span data-ttu-id="e8a18-135">パスワードまたはパターンは、必須では、いずれかの許容可能です。</span><span class="sxs-lookup"><span data-stu-id="e8a18-135">A password or pattern is required, and any is acceptable.</span></span>|




