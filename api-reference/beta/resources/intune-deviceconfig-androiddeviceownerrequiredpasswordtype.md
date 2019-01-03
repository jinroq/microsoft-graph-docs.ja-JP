---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者のポリシーでは、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: e0903bbf5720350b35bf7e5fe5c9a5f9584810c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330227"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="b29b5-103">androidDeviceOwnerRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b29b5-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="b29b5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b29b5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b29b5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b29b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b29b5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b29b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b29b5-107">Android デバイスの所有者のポリシーでは、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="b29b5-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="b29b5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b29b5-108">Members</span></span>
|<span data-ttu-id="b29b5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b29b5-109">Member</span></span>|<span data-ttu-id="b29b5-110">値</span><span class="sxs-lookup"><span data-stu-id="b29b5-110">Value</span></span>|<span data-ttu-id="b29b5-111">説明</span><span class="sxs-lookup"><span data-stu-id="b29b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29b5-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b29b5-112">deviceDefault</span></span>|<span data-ttu-id="b29b5-113">0</span><span class="sxs-lookup"><span data-stu-id="b29b5-113">0</span></span>|<span data-ttu-id="b29b5-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="b29b5-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b29b5-115">必須</span><span class="sxs-lookup"><span data-stu-id="b29b5-115">required</span></span>|<span data-ttu-id="b29b5-116">1</span><span class="sxs-lookup"><span data-stu-id="b29b5-116">1</span></span>|<span data-ttu-id="b29b5-117">パスワードのセットでは、必要がありますが、型に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="b29b5-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="b29b5-118">numeric</span><span class="sxs-lookup"><span data-stu-id="b29b5-118">numeric</span></span>|<span data-ttu-id="b29b5-119">2</span><span class="sxs-lookup"><span data-stu-id="b29b5-119">2</span></span>|<span data-ttu-id="b29b5-120">At は最低の数値です。</span><span class="sxs-lookup"><span data-stu-id="b29b5-120">At least numeric.</span></span>|
|<span data-ttu-id="b29b5-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="b29b5-121">numericComplex</span></span>|<span data-ttu-id="b29b5-122">3</span><span class="sxs-lookup"><span data-stu-id="b29b5-122">3</span></span>|<span data-ttu-id="b29b5-123">At なしまたは繰り返しの順序付けられたシーケンスでは、少なくとも数値です。</span><span class="sxs-lookup"><span data-stu-id="b29b5-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="b29b5-124">アルファベット</span><span class="sxs-lookup"><span data-stu-id="b29b5-124">alphabetic</span></span>|<span data-ttu-id="b29b5-125">4</span><span class="sxs-lookup"><span data-stu-id="b29b5-125">4</span></span>|<span data-ttu-id="b29b5-126">少なくともアルファベットのパスワードです。</span><span class="sxs-lookup"><span data-stu-id="b29b5-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="b29b5-127">英数字</span><span class="sxs-lookup"><span data-stu-id="b29b5-127">alphanumeric</span></span>|<span data-ttu-id="b29b5-128">5</span><span class="sxs-lookup"><span data-stu-id="b29b5-128">5</span></span>|<span data-ttu-id="b29b5-129">以上の英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="b29b5-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="b29b5-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="b29b5-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="b29b5-131">6</span><span class="sxs-lookup"><span data-stu-id="b29b5-131">6</span></span>|<span data-ttu-id="b29b5-132">少なくとも文字の英数字の記号です。</span><span class="sxs-lookup"><span data-stu-id="b29b5-132">At least alphanumeric with symbols.</span></span>|




