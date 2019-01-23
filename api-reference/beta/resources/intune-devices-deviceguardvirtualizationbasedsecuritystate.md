---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 39588aff1385bb14e1bf52f5d41b4848c1384138
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399767"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="bacd9-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="bacd9-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="bacd9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bacd9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bacd9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bacd9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bacd9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bacd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacd9-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bacd9-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="bacd9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bacd9-108">Members</span></span>
|<span data-ttu-id="bacd9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="bacd9-109">Member</span></span>|<span data-ttu-id="bacd9-110">値</span><span class="sxs-lookup"><span data-stu-id="bacd9-110">Value</span></span>|<span data-ttu-id="bacd9-111">説明</span><span class="sxs-lookup"><span data-stu-id="bacd9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacd9-112">実行</span><span class="sxs-lookup"><span data-stu-id="bacd9-112">running</span></span>|<span data-ttu-id="bacd9-113">0</span><span class="sxs-lookup"><span data-stu-id="bacd9-113">0</span></span>|<span data-ttu-id="bacd9-114">実行中</span><span class="sxs-lookup"><span data-stu-id="bacd9-114">Running</span></span>|
|<span data-ttu-id="bacd9-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="bacd9-115">rebootRequired</span></span>|<span data-ttu-id="bacd9-116">1</span><span class="sxs-lookup"><span data-stu-id="bacd9-116">1</span></span>|<span data-ttu-id="bacd9-117">必要なルート</span><span class="sxs-lookup"><span data-stu-id="bacd9-117">Root required</span></span>|
|<span data-ttu-id="bacd9-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="bacd9-118">require64BitArchitecture</span></span>|<span data-ttu-id="bacd9-119">2</span><span class="sxs-lookup"><span data-stu-id="bacd9-119">2</span></span>|<span data-ttu-id="bacd9-120">必要な 64 ビット アーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="bacd9-120">64 bit architecture required</span></span>|
|<span data-ttu-id="bacd9-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="bacd9-121">notLicensed</span></span>|<span data-ttu-id="bacd9-122">3</span><span class="sxs-lookup"><span data-stu-id="bacd9-122">3</span></span>|<span data-ttu-id="bacd9-123">ライセンスがありません。</span><span class="sxs-lookup"><span data-stu-id="bacd9-123">Not licensed</span></span>|
|<span data-ttu-id="bacd9-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bacd9-124">notConfigured</span></span>|<span data-ttu-id="bacd9-125">4</span><span class="sxs-lookup"><span data-stu-id="bacd9-125">4</span></span>|<span data-ttu-id="bacd9-126">構成されていません</span><span class="sxs-lookup"><span data-stu-id="bacd9-126">Not configured</span></span>|
|<span data-ttu-id="bacd9-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="bacd9-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="bacd9-128">5</span><span class="sxs-lookup"><span data-stu-id="bacd9-128">5</span></span>|<span data-ttu-id="bacd9-129">システムがハードウェア要件を満たしていません。</span><span class="sxs-lookup"><span data-stu-id="bacd9-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="bacd9-130">その他の</span><span class="sxs-lookup"><span data-stu-id="bacd9-130">other</span></span>|<span data-ttu-id="bacd9-131">42</span><span class="sxs-lookup"><span data-stu-id="bacd9-131">42</span></span>|<span data-ttu-id="bacd9-132">他の。</span><span class="sxs-lookup"><span data-stu-id="bacd9-132">Other.</span></span> <span data-ttu-id="bacd9-133">DeviceGuard-マイクロソフトの Windows のイベント ログには、詳細情報があります。</span><span class="sxs-lookup"><span data-stu-id="bacd9-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|




