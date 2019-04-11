---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51def159e90b256e772138264139f2a96fbd3344
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778531"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="e58f8-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e58f8-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="e58f8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e58f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e58f8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e58f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e58f8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e58f8-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e58f8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e58f8-107">Members</span></span>
|<span data-ttu-id="e58f8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e58f8-108">Member</span></span>|<span data-ttu-id="e58f8-109">値</span><span class="sxs-lookup"><span data-stu-id="e58f8-109">Value</span></span>|<span data-ttu-id="e58f8-110">説明</span><span class="sxs-lookup"><span data-stu-id="e58f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e58f8-111">起動</span><span class="sxs-lookup"><span data-stu-id="e58f8-111">running</span></span>|<span data-ttu-id="e58f8-112">.0</span><span class="sxs-lookup"><span data-stu-id="e58f8-112">0</span></span>|<span data-ttu-id="e58f8-113">実行中</span><span class="sxs-lookup"><span data-stu-id="e58f8-113">Running</span></span>|
|<span data-ttu-id="e58f8-114">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="e58f8-114">rebootRequired</span></span>|<span data-ttu-id="e58f8-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e58f8-115">1</span></span>|<span data-ttu-id="e58f8-116">必要なルート</span><span class="sxs-lookup"><span data-stu-id="e58f8-116">Root required</span></span>|
|<span data-ttu-id="e58f8-117">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="e58f8-117">require64BitArchitecture</span></span>|<span data-ttu-id="e58f8-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e58f8-118">2</span></span>|<span data-ttu-id="e58f8-119">64ビットアーキテクチャが必要</span><span class="sxs-lookup"><span data-stu-id="e58f8-119">64 bit architecture required</span></span>|
|<span data-ttu-id="e58f8-120">notlicensed</span><span class="sxs-lookup"><span data-stu-id="e58f8-120">notLicensed</span></span>|<span data-ttu-id="e58f8-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e58f8-121">3</span></span>|<span data-ttu-id="e58f8-122">ライセンスなし</span><span class="sxs-lookup"><span data-stu-id="e58f8-122">Not licensed</span></span>|
|<span data-ttu-id="e58f8-123">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e58f8-123">notConfigured</span></span>|<span data-ttu-id="e58f8-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e58f8-124">4</span></span>|<span data-ttu-id="e58f8-125">未構成</span><span class="sxs-lookup"><span data-stu-id="e58f8-125">Not configured</span></span>|
|<span data-ttu-id="e58f8-126">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="e58f8-126">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="e58f8-127">5</span><span class="sxs-lookup"><span data-stu-id="e58f8-127">5</span></span>|<span data-ttu-id="e58f8-128">システムがハードウェア要件を満たしていない</span><span class="sxs-lookup"><span data-stu-id="e58f8-128">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="e58f8-129">も</span><span class="sxs-lookup"><span data-stu-id="e58f8-129">other</span></span>|<span data-ttu-id="e58f8-130">42</span><span class="sxs-lookup"><span data-stu-id="e58f8-130">42</span></span>|<span data-ttu-id="e58f8-131">も.</span><span class="sxs-lookup"><span data-stu-id="e58f8-131">Other.</span></span> <span data-ttu-id="e58f8-132">microsoft-deviceguard のイベントログには、詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e58f8-132">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





