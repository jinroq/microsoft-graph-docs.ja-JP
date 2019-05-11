---
title: chassisType 列挙型
description: シャーシの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5805828091425ba9a0a949c69dcbab2c5bc752fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943026"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="468d4-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="468d4-103">chassisType enum type</span></span>

> <span data-ttu-id="468d4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="468d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="468d4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="468d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="468d4-106">シャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="468d4-106">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="468d4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="468d4-107">Members</span></span>
|<span data-ttu-id="468d4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="468d4-108">Member</span></span>|<span data-ttu-id="468d4-109">値</span><span class="sxs-lookup"><span data-stu-id="468d4-109">Value</span></span>|<span data-ttu-id="468d4-110">説明</span><span class="sxs-lookup"><span data-stu-id="468d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="468d4-111">不明</span><span class="sxs-lookup"><span data-stu-id="468d4-111">unknown</span></span>|<span data-ttu-id="468d4-112">.0</span><span class="sxs-lookup"><span data-stu-id="468d4-112">0</span></span>|<span data-ttu-id="468d4-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="468d4-113">Unknown.</span></span>|
|<span data-ttu-id="468d4-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="468d4-114">desktop</span></span>|<span data-ttu-id="468d4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="468d4-115">1</span></span>|<span data-ttu-id="468d4-116">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="468d4-116">Desktop.</span></span>|
|<span data-ttu-id="468d4-117">機</span><span class="sxs-lookup"><span data-stu-id="468d4-117">laptop</span></span>|<span data-ttu-id="468d4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="468d4-118">2</span></span>|<span data-ttu-id="468d4-119">機.</span><span class="sxs-lookup"><span data-stu-id="468d4-119">Laptop.</span></span>|
|<span data-ttu-id="468d4-120">ワークステーション</span><span class="sxs-lookup"><span data-stu-id="468d4-120">worksWorkstation</span></span>|<span data-ttu-id="468d4-121">1/3</span><span class="sxs-lookup"><span data-stu-id="468d4-121">3</span></span>|<span data-ttu-id="468d4-122">オフィス.</span><span class="sxs-lookup"><span data-stu-id="468d4-122">Workstation.</span></span>|
|<span data-ttu-id="468d4-123">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="468d4-123">enterpriseServer</span></span>|<span data-ttu-id="468d4-124">2/4</span><span class="sxs-lookup"><span data-stu-id="468d4-124">4</span></span>|<span data-ttu-id="468d4-125">エンタープライズサーバー。</span><span class="sxs-lookup"><span data-stu-id="468d4-125">Enterprise server.</span></span>|
|<span data-ttu-id="468d4-126">phone</span><span class="sxs-lookup"><span data-stu-id="468d4-126">phone</span></span>|<span data-ttu-id="468d4-127">100</span><span class="sxs-lookup"><span data-stu-id="468d4-127">100</span></span>|<span data-ttu-id="468d4-128">代わり.</span><span class="sxs-lookup"><span data-stu-id="468d4-128">Phone.</span></span>|
|<span data-ttu-id="468d4-129">タブレット</span><span class="sxs-lookup"><span data-stu-id="468d4-129">tablet</span></span>|<span data-ttu-id="468d4-130">101</span><span class="sxs-lookup"><span data-stu-id="468d4-130">101</span></span>|<span data-ttu-id="468d4-131">モバイルタブレット。</span><span class="sxs-lookup"><span data-stu-id="468d4-131">Mobile tablet.</span></span>|
|<span data-ttu-id="468d4-132">mobileOther</span><span class="sxs-lookup"><span data-stu-id="468d4-132">mobileOther</span></span>|<span data-ttu-id="468d4-133">102</span><span class="sxs-lookup"><span data-stu-id="468d4-133">102</span></span>|<span data-ttu-id="468d4-134">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="468d4-134">Other mobile.</span></span>|
|<span data-ttu-id="468d4-135">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="468d4-135">mobileUnknown</span></span>|<span data-ttu-id="468d4-136">103</span><span class="sxs-lookup"><span data-stu-id="468d4-136">103</span></span>|<span data-ttu-id="468d4-137">不明なモバイル。</span><span class="sxs-lookup"><span data-stu-id="468d4-137">Unknown mobile.</span></span>|




