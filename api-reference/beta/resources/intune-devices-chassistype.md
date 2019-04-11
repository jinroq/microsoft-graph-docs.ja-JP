---
title: chassisType 列挙型
description: シャーシの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeee3eefb63c5387b134daeb75f920dbe13d1236
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772574"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="65d72-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="65d72-103">chassisType enum type</span></span>

> <span data-ttu-id="65d72-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65d72-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65d72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65d72-106">シャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="65d72-106">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="65d72-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="65d72-107">Members</span></span>
|<span data-ttu-id="65d72-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="65d72-108">Member</span></span>|<span data-ttu-id="65d72-109">値</span><span class="sxs-lookup"><span data-stu-id="65d72-109">Value</span></span>|<span data-ttu-id="65d72-110">説明</span><span class="sxs-lookup"><span data-stu-id="65d72-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d72-111">不明</span><span class="sxs-lookup"><span data-stu-id="65d72-111">unknown</span></span>|<span data-ttu-id="65d72-112">.0</span><span class="sxs-lookup"><span data-stu-id="65d72-112">0</span></span>|<span data-ttu-id="65d72-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="65d72-113">Unknown.</span></span>|
|<span data-ttu-id="65d72-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="65d72-114">desktop</span></span>|<span data-ttu-id="65d72-115">1-d</span><span class="sxs-lookup"><span data-stu-id="65d72-115">1</span></span>|<span data-ttu-id="65d72-116">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="65d72-116">Desktop.</span></span>|
|<span data-ttu-id="65d72-117">機</span><span class="sxs-lookup"><span data-stu-id="65d72-117">laptop</span></span>|<span data-ttu-id="65d72-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="65d72-118">2</span></span>|<span data-ttu-id="65d72-119">機.</span><span class="sxs-lookup"><span data-stu-id="65d72-119">Laptop.</span></span>|
|<span data-ttu-id="65d72-120">ワークステーション</span><span class="sxs-lookup"><span data-stu-id="65d72-120">worksWorkstation</span></span>|<span data-ttu-id="65d72-121">1/3</span><span class="sxs-lookup"><span data-stu-id="65d72-121">3</span></span>|<span data-ttu-id="65d72-122">オフィス.</span><span class="sxs-lookup"><span data-stu-id="65d72-122">Workstation.</span></span>|
|<span data-ttu-id="65d72-123">enterpriseserver</span><span class="sxs-lookup"><span data-stu-id="65d72-123">enterpriseServer</span></span>|<span data-ttu-id="65d72-124">2/4</span><span class="sxs-lookup"><span data-stu-id="65d72-124">4</span></span>|<span data-ttu-id="65d72-125">エンタープライズサーバー。</span><span class="sxs-lookup"><span data-stu-id="65d72-125">Enterprise server.</span></span>|
|<span data-ttu-id="65d72-126">phone</span><span class="sxs-lookup"><span data-stu-id="65d72-126">phone</span></span>|<span data-ttu-id="65d72-127">100</span><span class="sxs-lookup"><span data-stu-id="65d72-127">100</span></span>|<span data-ttu-id="65d72-128">代わり.</span><span class="sxs-lookup"><span data-stu-id="65d72-128">Phone.</span></span>|
|<span data-ttu-id="65d72-129">タブレット</span><span class="sxs-lookup"><span data-stu-id="65d72-129">tablet</span></span>|<span data-ttu-id="65d72-130">101</span><span class="sxs-lookup"><span data-stu-id="65d72-130">101</span></span>|<span data-ttu-id="65d72-131">モバイルタブレット。</span><span class="sxs-lookup"><span data-stu-id="65d72-131">Mobile tablet.</span></span>|
|<span data-ttu-id="65d72-132">mobileOther</span><span class="sxs-lookup"><span data-stu-id="65d72-132">mobileOther</span></span>|<span data-ttu-id="65d72-133">102</span><span class="sxs-lookup"><span data-stu-id="65d72-133">102</span></span>|<span data-ttu-id="65d72-134">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="65d72-134">Other mobile.</span></span>|
|<span data-ttu-id="65d72-135">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="65d72-135">mobileUnknown</span></span>|<span data-ttu-id="65d72-136">103</span><span class="sxs-lookup"><span data-stu-id="65d72-136">103</span></span>|<span data-ttu-id="65d72-137">不明なモバイル。</span><span class="sxs-lookup"><span data-stu-id="65d72-137">Unknown mobile.</span></span>|





