---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者のポリシーでは、パスワード入力が必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403540"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="9e8f9-103">androidDeviceOwnerRequiredPasswordType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9e8f9-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9e8f9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e8f9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e8f9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e8f9-107">Android デバイスの所有者のポリシーでは、パスワード入力が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9e8f9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e8f9-108">Members</span></span>
|<span data-ttu-id="9e8f9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e8f9-109">Member</span></span>|<span data-ttu-id="9e8f9-110">値</span><span class="sxs-lookup"><span data-stu-id="9e8f9-110">Value</span></span>|<span data-ttu-id="9e8f9-111">説明</span><span class="sxs-lookup"><span data-stu-id="9e8f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e8f9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9e8f9-112">deviceDefault</span></span>|<span data-ttu-id="9e8f9-113">0</span><span class="sxs-lookup"><span data-stu-id="9e8f9-113">0</span></span>|<span data-ttu-id="9e8f9-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9e8f9-115">必須</span><span class="sxs-lookup"><span data-stu-id="9e8f9-115">required</span></span>|<span data-ttu-id="9e8f9-116">1</span><span class="sxs-lookup"><span data-stu-id="9e8f9-116">1</span></span>|<span data-ttu-id="9e8f9-117">パスワードのセットでは、必要がありますが、型に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="9e8f9-118">numeric</span><span class="sxs-lookup"><span data-stu-id="9e8f9-118">numeric</span></span>|<span data-ttu-id="9e8f9-119">2</span><span class="sxs-lookup"><span data-stu-id="9e8f9-119">2</span></span>|<span data-ttu-id="9e8f9-120">At は最低の数値です。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-120">At least numeric.</span></span>|
|<span data-ttu-id="9e8f9-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9e8f9-121">numericComplex</span></span>|<span data-ttu-id="9e8f9-122">3</span><span class="sxs-lookup"><span data-stu-id="9e8f9-122">3</span></span>|<span data-ttu-id="9e8f9-123">At なしまたは繰り返しの順序付けられたシーケンスでは、少なくとも数値です。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="9e8f9-124">アルファベット</span><span class="sxs-lookup"><span data-stu-id="9e8f9-124">alphabetic</span></span>|<span data-ttu-id="9e8f9-125">4</span><span class="sxs-lookup"><span data-stu-id="9e8f9-125">4</span></span>|<span data-ttu-id="9e8f9-126">少なくともアルファベットのパスワードです。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="9e8f9-127">英数字</span><span class="sxs-lookup"><span data-stu-id="9e8f9-127">alphanumeric</span></span>|<span data-ttu-id="9e8f9-128">5</span><span class="sxs-lookup"><span data-stu-id="9e8f9-128">5</span></span>|<span data-ttu-id="9e8f9-129">以上の英数字のパスワード</span><span class="sxs-lookup"><span data-stu-id="9e8f9-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="9e8f9-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9e8f9-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="9e8f9-131">6</span><span class="sxs-lookup"><span data-stu-id="9e8f9-131">6</span></span>|<span data-ttu-id="9e8f9-132">少なくとも文字の英数字の記号です。</span><span class="sxs-lookup"><span data-stu-id="9e8f9-132">At least alphanumeric with symbols.</span></span>|




