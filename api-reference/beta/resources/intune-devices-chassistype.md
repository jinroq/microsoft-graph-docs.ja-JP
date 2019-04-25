---
title: chassisType 列挙型
description: シャーシの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeee3eefb63c5387b134daeb75f920dbe13d1236
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576403"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="092d8-103">chassisType 列挙型</span><span class="sxs-lookup"><span data-stu-id="092d8-103">chassisType enum type</span></span>

> <span data-ttu-id="092d8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="092d8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="092d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="092d8-106">シャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="092d8-106">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="092d8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="092d8-107">Members</span></span>
|<span data-ttu-id="092d8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="092d8-108">Member</span></span>|<span data-ttu-id="092d8-109">値</span><span class="sxs-lookup"><span data-stu-id="092d8-109">Value</span></span>|<span data-ttu-id="092d8-110">説明</span><span class="sxs-lookup"><span data-stu-id="092d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="092d8-111">不明</span><span class="sxs-lookup"><span data-stu-id="092d8-111">unknown</span></span>|<span data-ttu-id="092d8-112">.0</span><span class="sxs-lookup"><span data-stu-id="092d8-112">0</span></span>|<span data-ttu-id="092d8-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="092d8-113">Unknown.</span></span>|
|<span data-ttu-id="092d8-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="092d8-114">desktop</span></span>|<span data-ttu-id="092d8-115">1 </span><span class="sxs-lookup"><span data-stu-id="092d8-115">1</span></span>|<span data-ttu-id="092d8-116">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="092d8-116">Desktop.</span></span>|
|<span data-ttu-id="092d8-117">機</span><span class="sxs-lookup"><span data-stu-id="092d8-117">laptop</span></span>|<span data-ttu-id="092d8-118">2 </span><span class="sxs-lookup"><span data-stu-id="092d8-118">2</span></span>|<span data-ttu-id="092d8-119">機.</span><span class="sxs-lookup"><span data-stu-id="092d8-119">Laptop.</span></span>|
|<span data-ttu-id="092d8-120">ワークステーション</span><span class="sxs-lookup"><span data-stu-id="092d8-120">worksWorkstation</span></span>|<span data-ttu-id="092d8-121">3 </span><span class="sxs-lookup"><span data-stu-id="092d8-121">3</span></span>|<span data-ttu-id="092d8-122">オフィス.</span><span class="sxs-lookup"><span data-stu-id="092d8-122">Workstation.</span></span>|
|<span data-ttu-id="092d8-123">enterpriseserver</span><span class="sxs-lookup"><span data-stu-id="092d8-123">enterpriseServer</span></span>|<span data-ttu-id="092d8-124">4 </span><span class="sxs-lookup"><span data-stu-id="092d8-124">4</span></span>|<span data-ttu-id="092d8-125">エンタープライズサーバー。</span><span class="sxs-lookup"><span data-stu-id="092d8-125">Enterprise server.</span></span>|
|<span data-ttu-id="092d8-126">phone</span><span class="sxs-lookup"><span data-stu-id="092d8-126">phone</span></span>|<span data-ttu-id="092d8-127">100</span><span class="sxs-lookup"><span data-stu-id="092d8-127">100</span></span>|<span data-ttu-id="092d8-128">代わり.</span><span class="sxs-lookup"><span data-stu-id="092d8-128">Phone.</span></span>|
|<span data-ttu-id="092d8-129">タブレット</span><span class="sxs-lookup"><span data-stu-id="092d8-129">tablet</span></span>|<span data-ttu-id="092d8-130">101</span><span class="sxs-lookup"><span data-stu-id="092d8-130">101</span></span>|<span data-ttu-id="092d8-131">モバイルタブレット。</span><span class="sxs-lookup"><span data-stu-id="092d8-131">Mobile tablet.</span></span>|
|<span data-ttu-id="092d8-132">mobileOther</span><span class="sxs-lookup"><span data-stu-id="092d8-132">mobileOther</span></span>|<span data-ttu-id="092d8-133">102</span><span class="sxs-lookup"><span data-stu-id="092d8-133">102</span></span>|<span data-ttu-id="092d8-134">その他のモバイル。</span><span class="sxs-lookup"><span data-stu-id="092d8-134">Other mobile.</span></span>|
|<span data-ttu-id="092d8-135">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="092d8-135">mobileUnknown</span></span>|<span data-ttu-id="092d8-136">103</span><span class="sxs-lookup"><span data-stu-id="092d8-136">103</span></span>|<span data-ttu-id="092d8-137">不明なモバイル。</span><span class="sxs-lookup"><span data-stu-id="092d8-137">Unknown mobile.</span></span>|





