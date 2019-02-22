---
title: chassisType 列挙型
description: シャーシの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e925dcf502c28951bb8636652e5d429d0cd0916
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161524"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="b8a5f-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b8a5f-103">chassisType enum type</span></span>

> <span data-ttu-id="b8a5f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a5f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a5f-106">シャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-106">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="b8a5f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8a5f-107">Members</span></span>
|<span data-ttu-id="b8a5f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8a5f-108">Member</span></span>|<span data-ttu-id="b8a5f-109">値</span><span class="sxs-lookup"><span data-stu-id="b8a5f-109">Value</span></span>|<span data-ttu-id="b8a5f-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8a5f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a5f-111">不明</span><span class="sxs-lookup"><span data-stu-id="b8a5f-111">unknown</span></span>|<span data-ttu-id="b8a5f-112">.0</span><span class="sxs-lookup"><span data-stu-id="b8a5f-112">0</span></span>|<span data-ttu-id="b8a5f-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="b8a5f-113">Unknown.</span></span>|
|<span data-ttu-id="b8a5f-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="b8a5f-114">desktop</span></span>|<span data-ttu-id="b8a5f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b8a5f-115">1</span></span>|<span data-ttu-id="b8a5f-116">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="b8a5f-116">Desktop.</span></span>|
|<span data-ttu-id="b8a5f-117">機</span><span class="sxs-lookup"><span data-stu-id="b8a5f-117">laptop</span></span>|<span data-ttu-id="b8a5f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b8a5f-118">2</span></span>|<span data-ttu-id="b8a5f-119">機.</span><span class="sxs-lookup"><span data-stu-id="b8a5f-119">Laptop.</span></span>|
|<span data-ttu-id="b8a5f-120">ワークステーション</span><span class="sxs-lookup"><span data-stu-id="b8a5f-120">worksWorkstation</span></span>|<span data-ttu-id="b8a5f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="b8a5f-121">3</span></span>|<span data-ttu-id="b8a5f-122">オフィス.</span><span class="sxs-lookup"><span data-stu-id="b8a5f-122">Workstation.</span></span>|
|<span data-ttu-id="b8a5f-123">enterpriseserver</span><span class="sxs-lookup"><span data-stu-id="b8a5f-123">enterpriseServer</span></span>|<span data-ttu-id="b8a5f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="b8a5f-124">4</span></span>|<span data-ttu-id="b8a5f-125">エンタープライズサーバー。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-125">Enterprise server.</span></span>|
|<span data-ttu-id="b8a5f-126">phone</span><span class="sxs-lookup"><span data-stu-id="b8a5f-126">phone</span></span>|<span data-ttu-id="b8a5f-127">100</span><span class="sxs-lookup"><span data-stu-id="b8a5f-127">100</span></span>|<span data-ttu-id="b8a5f-128">代わり.</span><span class="sxs-lookup"><span data-stu-id="b8a5f-128">Phone.</span></span>|
|<span data-ttu-id="b8a5f-129">タブレット</span><span class="sxs-lookup"><span data-stu-id="b8a5f-129">tablet</span></span>|<span data-ttu-id="b8a5f-130">101</span><span class="sxs-lookup"><span data-stu-id="b8a5f-130">101</span></span>|<span data-ttu-id="b8a5f-131">モバイルタブレット。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-131">Mobile tablet.</span></span>|
|<span data-ttu-id="b8a5f-132">mobileOther</span><span class="sxs-lookup"><span data-stu-id="b8a5f-132">mobileOther</span></span>|<span data-ttu-id="b8a5f-133">102</span><span class="sxs-lookup"><span data-stu-id="b8a5f-133">102</span></span>|<span data-ttu-id="b8a5f-134">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-134">Other mobile.</span></span>|
|<span data-ttu-id="b8a5f-135">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="b8a5f-135">mobileUnknown</span></span>|<span data-ttu-id="b8a5f-136">103</span><span class="sxs-lookup"><span data-stu-id="b8a5f-136">103</span></span>|<span data-ttu-id="b8a5f-137">不明なモバイル。</span><span class="sxs-lookup"><span data-stu-id="b8a5f-137">Unknown mobile.</span></span>|




