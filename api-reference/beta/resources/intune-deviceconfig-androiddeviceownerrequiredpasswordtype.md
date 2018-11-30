---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者のポリシーでは、パスワード入力が必要です。
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070887"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="1e97c-103">androidDeviceOwnerRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1e97c-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="1e97c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e97c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e97c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e97c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e97c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e97c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e97c-107">Android デバイスの所有者のポリシーでは、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e97c-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="1e97c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1e97c-108">Members</span></span>
|<span data-ttu-id="1e97c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1e97c-109">Member</span></span>|<span data-ttu-id="1e97c-110">値</span><span class="sxs-lookup"><span data-stu-id="1e97c-110">Value</span></span>|<span data-ttu-id="1e97c-111">説明</span><span class="sxs-lookup"><span data-stu-id="1e97c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e97c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1e97c-112">deviceDefault</span></span>|<span data-ttu-id="1e97c-113">0</span><span class="sxs-lookup"><span data-stu-id="1e97c-113">0</span></span>|<span data-ttu-id="1e97c-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="1e97c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1e97c-115">必須</span><span class="sxs-lookup"><span data-stu-id="1e97c-115">required</span></span>|<span data-ttu-id="1e97c-116">1</span><span class="sxs-lookup"><span data-stu-id="1e97c-116">1</span></span>|<span data-ttu-id="1e97c-117">パスワードのセットでは、必要がありますが、型に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="1e97c-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="1e97c-118">numeric</span><span class="sxs-lookup"><span data-stu-id="1e97c-118">numeric</span></span>|<span data-ttu-id="1e97c-119">2</span><span class="sxs-lookup"><span data-stu-id="1e97c-119">2</span></span>|<span data-ttu-id="1e97c-120">At は最低の数値です。</span><span class="sxs-lookup"><span data-stu-id="1e97c-120">At least numeric.</span></span>|
|<span data-ttu-id="1e97c-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="1e97c-121">numericComplex</span></span>|<span data-ttu-id="1e97c-122">3</span><span class="sxs-lookup"><span data-stu-id="1e97c-122">3</span></span>|<span data-ttu-id="1e97c-123">At なしまたは繰り返しの順序付けられたシーケンスでは、少なくとも数値です。</span><span class="sxs-lookup"><span data-stu-id="1e97c-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="1e97c-124">アルファベット</span><span class="sxs-lookup"><span data-stu-id="1e97c-124">alphabetic</span></span>|<span data-ttu-id="1e97c-125">4</span><span class="sxs-lookup"><span data-stu-id="1e97c-125">4</span></span>|<span data-ttu-id="1e97c-126">少なくともアルファベットのパスワードです。</span><span class="sxs-lookup"><span data-stu-id="1e97c-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="1e97c-127">英数字</span><span class="sxs-lookup"><span data-stu-id="1e97c-127">alphanumeric</span></span>|<span data-ttu-id="1e97c-128">5</span><span class="sxs-lookup"><span data-stu-id="1e97c-128">5</span></span>|<span data-ttu-id="1e97c-129">以上の英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="1e97c-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="1e97c-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="1e97c-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="1e97c-131">6</span><span class="sxs-lookup"><span data-stu-id="1e97c-131">6</span></span>|<span data-ttu-id="1e97c-132">少なくとも文字の英数字の記号です。</span><span class="sxs-lookup"><span data-stu-id="1e97c-132">At least alphanumeric with symbols.</span></span>|





