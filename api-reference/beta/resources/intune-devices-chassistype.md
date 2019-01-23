---
title: chassisType 列挙型
description: シャーシを入力します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 29daba2a6e1c9aacf97b3b5b946d925c4163ea69
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422384"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="1eec2-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1eec2-103">chassisType enum type</span></span>

> <span data-ttu-id="1eec2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1eec2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1eec2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eec2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1eec2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1eec2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eec2-107">シャーシを入力します。</span><span class="sxs-lookup"><span data-stu-id="1eec2-107">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="1eec2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1eec2-108">Members</span></span>
|<span data-ttu-id="1eec2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1eec2-109">Member</span></span>|<span data-ttu-id="1eec2-110">値</span><span class="sxs-lookup"><span data-stu-id="1eec2-110">Value</span></span>|<span data-ttu-id="1eec2-111">説明</span><span class="sxs-lookup"><span data-stu-id="1eec2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eec2-112">不明</span><span class="sxs-lookup"><span data-stu-id="1eec2-112">unknown</span></span>|<span data-ttu-id="1eec2-113">0</span><span class="sxs-lookup"><span data-stu-id="1eec2-113">0</span></span>|<span data-ttu-id="1eec2-114">不明。</span><span class="sxs-lookup"><span data-stu-id="1eec2-114">Unknown.</span></span>|
|<span data-ttu-id="1eec2-115">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="1eec2-115">desktop</span></span>|<span data-ttu-id="1eec2-116">1</span><span class="sxs-lookup"><span data-stu-id="1eec2-116">1</span></span>|<span data-ttu-id="1eec2-117">デスクトップです。</span><span class="sxs-lookup"><span data-stu-id="1eec2-117">Desktop.</span></span>|
|<span data-ttu-id="1eec2-118">ラップトップ</span><span class="sxs-lookup"><span data-stu-id="1eec2-118">laptop</span></span>|<span data-ttu-id="1eec2-119">2</span><span class="sxs-lookup"><span data-stu-id="1eec2-119">2</span></span>|<span data-ttu-id="1eec2-120">ラップトップ コンピューター。</span><span class="sxs-lookup"><span data-stu-id="1eec2-120">Laptop.</span></span>|
|<span data-ttu-id="1eec2-121">worksWorkstation</span><span class="sxs-lookup"><span data-stu-id="1eec2-121">worksWorkstation</span></span>|<span data-ttu-id="1eec2-122">3</span><span class="sxs-lookup"><span data-stu-id="1eec2-122">3</span></span>|<span data-ttu-id="1eec2-123">ワークステーションです。</span><span class="sxs-lookup"><span data-stu-id="1eec2-123">Workstation.</span></span>|
|<span data-ttu-id="1eec2-124">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="1eec2-124">enterpriseServer</span></span>|<span data-ttu-id="1eec2-125">4</span><span class="sxs-lookup"><span data-stu-id="1eec2-125">4</span></span>|<span data-ttu-id="1eec2-126">エンタープライズ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="1eec2-126">Enterprise server.</span></span>|
|<span data-ttu-id="1eec2-127">phone</span><span class="sxs-lookup"><span data-stu-id="1eec2-127">phone</span></span>|<span data-ttu-id="1eec2-128">100</span><span class="sxs-lookup"><span data-stu-id="1eec2-128">100</span></span>|<span data-ttu-id="1eec2-129">電話です。</span><span class="sxs-lookup"><span data-stu-id="1eec2-129">Phone.</span></span>|
|<span data-ttu-id="1eec2-130">タブレット</span><span class="sxs-lookup"><span data-stu-id="1eec2-130">tablet</span></span>|<span data-ttu-id="1eec2-131">101</span><span class="sxs-lookup"><span data-stu-id="1eec2-131">101</span></span>|<span data-ttu-id="1eec2-132">モバイル タブレットです。</span><span class="sxs-lookup"><span data-stu-id="1eec2-132">Mobile tablet.</span></span>|
|<span data-ttu-id="1eec2-133">mobileOther</span><span class="sxs-lookup"><span data-stu-id="1eec2-133">mobileOther</span></span>|<span data-ttu-id="1eec2-134">102</span><span class="sxs-lookup"><span data-stu-id="1eec2-134">102</span></span>|<span data-ttu-id="1eec2-135">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="1eec2-135">Other mobile.</span></span>|
|<span data-ttu-id="1eec2-136">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="1eec2-136">mobileUnknown</span></span>|<span data-ttu-id="1eec2-137">103</span><span class="sxs-lookup"><span data-stu-id="1eec2-137">103</span></span>|<span data-ttu-id="1eec2-138">モバイル不明です。</span><span class="sxs-lookup"><span data-stu-id="1eec2-138">Unknown mobile.</span></span>|




