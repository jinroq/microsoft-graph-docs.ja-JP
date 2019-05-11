---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc6d81a71fe01addb6111252b28aee01072fe0dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949067"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="a3ea1-103">androidDeviceOwnerRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a3ea1-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a3ea1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3ea1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3ea1-106">Android デバイスの所有者ポリシーに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a3ea1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a3ea1-107">Members</span></span>
|<span data-ttu-id="a3ea1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a3ea1-108">Member</span></span>|<span data-ttu-id="a3ea1-109">値</span><span class="sxs-lookup"><span data-stu-id="a3ea1-109">Value</span></span>|<span data-ttu-id="a3ea1-110">説明</span><span class="sxs-lookup"><span data-stu-id="a3ea1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3ea1-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a3ea1-111">deviceDefault</span></span>|<span data-ttu-id="a3ea1-112">.0</span><span class="sxs-lookup"><span data-stu-id="a3ea1-112">0</span></span>|<span data-ttu-id="a3ea1-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a3ea1-114">必須</span><span class="sxs-lookup"><span data-stu-id="a3ea1-114">required</span></span>|<span data-ttu-id="a3ea1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a3ea1-115">1</span></span>|<span data-ttu-id="a3ea1-116">パスワードを設定する必要がありますが、種類に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="a3ea1-117">数値</span><span class="sxs-lookup"><span data-stu-id="a3ea1-117">numeric</span></span>|<span data-ttu-id="a3ea1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a3ea1-118">2</span></span>|<span data-ttu-id="a3ea1-119">少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-119">At least numeric.</span></span>|
|<span data-ttu-id="a3ea1-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a3ea1-120">numericComplex</span></span>|<span data-ttu-id="a3ea1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a3ea1-121">3</span></span>|<span data-ttu-id="a3ea1-122">繰り返しまたは順序付けられていない、少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="a3ea1-123">読み</span><span class="sxs-lookup"><span data-stu-id="a3ea1-123">alphabetic</span></span>|<span data-ttu-id="a3ea1-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a3ea1-124">4</span></span>|<span data-ttu-id="a3ea1-125">少なくとも英字のパスワード。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="a3ea1-126">文字</span><span class="sxs-lookup"><span data-stu-id="a3ea1-126">alphanumeric</span></span>|<span data-ttu-id="a3ea1-127">5</span><span class="sxs-lookup"><span data-stu-id="a3ea1-127">5</span></span>|<span data-ttu-id="a3ea1-128">少なくとも英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="a3ea1-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="a3ea1-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a3ea1-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="a3ea1-130">シックス</span><span class="sxs-lookup"><span data-stu-id="a3ea1-130">6</span></span>|<span data-ttu-id="a3ea1-131">記号を含む、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="a3ea1-132">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="a3ea1-132">lowSecurityBiometric</span></span>|<span data-ttu-id="a3ea1-133">7</span><span class="sxs-lookup"><span data-stu-id="a3ea1-133">7</span></span>|<span data-ttu-id="a3ea1-134">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="a3ea1-134">Low security biometrics based password required.</span></span>|




