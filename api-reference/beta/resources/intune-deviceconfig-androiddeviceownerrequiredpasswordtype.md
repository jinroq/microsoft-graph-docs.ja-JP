---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e55aa24896e72a2351cfbfc2ac8a88ac2a2d3dd8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983793"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="76909-103">androidDeviceOwnerRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="76909-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="76909-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76909-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76909-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76909-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76909-106">Android デバイスの所有者ポリシーに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="76909-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="76909-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="76909-107">Members</span></span>
|<span data-ttu-id="76909-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="76909-108">Member</span></span>|<span data-ttu-id="76909-109">値</span><span class="sxs-lookup"><span data-stu-id="76909-109">Value</span></span>|<span data-ttu-id="76909-110">説明</span><span class="sxs-lookup"><span data-stu-id="76909-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76909-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="76909-111">deviceDefault</span></span>|<span data-ttu-id="76909-112">.0</span><span class="sxs-lookup"><span data-stu-id="76909-112">0</span></span>|<span data-ttu-id="76909-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="76909-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="76909-114">必須</span><span class="sxs-lookup"><span data-stu-id="76909-114">required</span></span>|<span data-ttu-id="76909-115">1-d</span><span class="sxs-lookup"><span data-stu-id="76909-115">1</span></span>|<span data-ttu-id="76909-116">パスワードを設定する必要がありますが、種類に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="76909-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="76909-117">数値</span><span class="sxs-lookup"><span data-stu-id="76909-117">numeric</span></span>|<span data-ttu-id="76909-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="76909-118">2</span></span>|<span data-ttu-id="76909-119">少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="76909-119">At least numeric.</span></span>|
|<span data-ttu-id="76909-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="76909-120">numericComplex</span></span>|<span data-ttu-id="76909-121">1/3</span><span class="sxs-lookup"><span data-stu-id="76909-121">3</span></span>|<span data-ttu-id="76909-122">繰り返しまたは順序付けられていない、少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="76909-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="76909-123">読み</span><span class="sxs-lookup"><span data-stu-id="76909-123">alphabetic</span></span>|<span data-ttu-id="76909-124">2/4</span><span class="sxs-lookup"><span data-stu-id="76909-124">4</span></span>|<span data-ttu-id="76909-125">少なくとも英字のパスワード。</span><span class="sxs-lookup"><span data-stu-id="76909-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="76909-126">文字</span><span class="sxs-lookup"><span data-stu-id="76909-126">alphanumeric</span></span>|<span data-ttu-id="76909-127">5</span><span class="sxs-lookup"><span data-stu-id="76909-127">5</span></span>|<span data-ttu-id="76909-128">少なくとも英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="76909-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="76909-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="76909-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="76909-130">シックス</span><span class="sxs-lookup"><span data-stu-id="76909-130">6</span></span>|<span data-ttu-id="76909-131">記号を含む、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="76909-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="76909-132">lowSecurityBiometric 認証</span><span class="sxs-lookup"><span data-stu-id="76909-132">lowSecurityBiometric</span></span>|<span data-ttu-id="76909-133">7</span><span class="sxs-lookup"><span data-stu-id="76909-133">7</span></span>|<span data-ttu-id="76909-134">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="76909-134">Low security biometrics based password required.</span></span>|





