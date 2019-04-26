---
title: androiddeviceownerrequiredpasswordtype 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556380"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="d3042-103">androiddeviceownerrequiredpasswordtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3042-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d3042-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3042-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3042-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3042-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3042-106">Android デバイスの所有者ポリシーに必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="d3042-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d3042-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3042-107">Members</span></span>
|<span data-ttu-id="d3042-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3042-108">Member</span></span>|<span data-ttu-id="d3042-109">値</span><span class="sxs-lookup"><span data-stu-id="d3042-109">Value</span></span>|<span data-ttu-id="d3042-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3042-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3042-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="d3042-111">deviceDefault</span></span>|<span data-ttu-id="d3042-112">.0</span><span class="sxs-lookup"><span data-stu-id="d3042-112">0</span></span>|<span data-ttu-id="d3042-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="d3042-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d3042-114">必須</span><span class="sxs-lookup"><span data-stu-id="d3042-114">required</span></span>|<span data-ttu-id="d3042-115">1 </span><span class="sxs-lookup"><span data-stu-id="d3042-115">1</span></span>|<span data-ttu-id="d3042-116">パスワードを設定する必要がありますが、種類に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="d3042-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="d3042-117">数値</span><span class="sxs-lookup"><span data-stu-id="d3042-117">numeric</span></span>|<span data-ttu-id="d3042-118">2 </span><span class="sxs-lookup"><span data-stu-id="d3042-118">2</span></span>|<span data-ttu-id="d3042-119">少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="d3042-119">At least numeric.</span></span>|
|<span data-ttu-id="d3042-120">numericcomplex</span><span class="sxs-lookup"><span data-stu-id="d3042-120">numericComplex</span></span>|<span data-ttu-id="d3042-121">3 </span><span class="sxs-lookup"><span data-stu-id="d3042-121">3</span></span>|<span data-ttu-id="d3042-122">繰り返しまたは順序付けられていない、少なくとも数値。</span><span class="sxs-lookup"><span data-stu-id="d3042-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="d3042-123">読み</span><span class="sxs-lookup"><span data-stu-id="d3042-123">alphabetic</span></span>|<span data-ttu-id="d3042-124">4 </span><span class="sxs-lookup"><span data-stu-id="d3042-124">4</span></span>|<span data-ttu-id="d3042-125">少なくとも英字のパスワード。</span><span class="sxs-lookup"><span data-stu-id="d3042-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="d3042-126">文字</span><span class="sxs-lookup"><span data-stu-id="d3042-126">alphanumeric</span></span>|<span data-ttu-id="d3042-127">5 </span><span class="sxs-lookup"><span data-stu-id="d3042-127">5</span></span>|<span data-ttu-id="d3042-128">少なくとも英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="d3042-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="d3042-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d3042-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="d3042-130">6 </span><span class="sxs-lookup"><span data-stu-id="d3042-130">6</span></span>|<span data-ttu-id="d3042-131">記号を含む、少なくとも英数字。</span><span class="sxs-lookup"><span data-stu-id="d3042-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="d3042-132">lowsecuritybiometric 認証</span><span class="sxs-lookup"><span data-stu-id="d3042-132">lowSecurityBiometric</span></span>|<span data-ttu-id="d3042-133">7 </span><span class="sxs-lookup"><span data-stu-id="d3042-133">7</span></span>|<span data-ttu-id="d3042-134">低セキュリティ生体認証ベースのパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="d3042-134">Low security biometrics based password required.</span></span>|





