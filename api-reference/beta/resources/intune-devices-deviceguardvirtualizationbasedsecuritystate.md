---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2c3d7745af4e6a93e9836f24a184e6ca90b60d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882377"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="05bdd-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="05bdd-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="05bdd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05bdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05bdd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05bdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05bdd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05bdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05bdd-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05bdd-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="05bdd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="05bdd-108">Members</span></span>
|<span data-ttu-id="05bdd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="05bdd-109">Member</span></span>|<span data-ttu-id="05bdd-110">値</span><span class="sxs-lookup"><span data-stu-id="05bdd-110">Value</span></span>|<span data-ttu-id="05bdd-111">説明</span><span class="sxs-lookup"><span data-stu-id="05bdd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05bdd-112">実行</span><span class="sxs-lookup"><span data-stu-id="05bdd-112">running</span></span>|<span data-ttu-id="05bdd-113">0</span><span class="sxs-lookup"><span data-stu-id="05bdd-113">0</span></span>|<span data-ttu-id="05bdd-114">実行中</span><span class="sxs-lookup"><span data-stu-id="05bdd-114">Running</span></span>|
|<span data-ttu-id="05bdd-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="05bdd-115">rebootRequired</span></span>|<span data-ttu-id="05bdd-116">1</span><span class="sxs-lookup"><span data-stu-id="05bdd-116">1</span></span>|<span data-ttu-id="05bdd-117">必要なルート</span><span class="sxs-lookup"><span data-stu-id="05bdd-117">Root required</span></span>|
|<span data-ttu-id="05bdd-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="05bdd-118">require64BitArchitecture</span></span>|<span data-ttu-id="05bdd-119">2</span><span class="sxs-lookup"><span data-stu-id="05bdd-119">2</span></span>|<span data-ttu-id="05bdd-120">必要な 64 ビット アーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="05bdd-120">64 bit architecture required</span></span>|
|<span data-ttu-id="05bdd-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="05bdd-121">notLicensed</span></span>|<span data-ttu-id="05bdd-122">3</span><span class="sxs-lookup"><span data-stu-id="05bdd-122">3</span></span>|<span data-ttu-id="05bdd-123">ライセンスがありません。</span><span class="sxs-lookup"><span data-stu-id="05bdd-123">Not licensed</span></span>|
|<span data-ttu-id="05bdd-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="05bdd-124">notConfigured</span></span>|<span data-ttu-id="05bdd-125">4</span><span class="sxs-lookup"><span data-stu-id="05bdd-125">4</span></span>|<span data-ttu-id="05bdd-126">構成されていません</span><span class="sxs-lookup"><span data-stu-id="05bdd-126">Not configured</span></span>|
|<span data-ttu-id="05bdd-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="05bdd-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="05bdd-128">5</span><span class="sxs-lookup"><span data-stu-id="05bdd-128">5</span></span>|<span data-ttu-id="05bdd-129">システムがハードウェア要件を満たしていません。</span><span class="sxs-lookup"><span data-stu-id="05bdd-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="05bdd-130">その他の</span><span class="sxs-lookup"><span data-stu-id="05bdd-130">other</span></span>|<span data-ttu-id="05bdd-131">42</span><span class="sxs-lookup"><span data-stu-id="05bdd-131">42</span></span>|<span data-ttu-id="05bdd-132">他の。</span><span class="sxs-lookup"><span data-stu-id="05bdd-132">Other.</span></span> <span data-ttu-id="05bdd-133">DeviceGuard-マイクロソフトの Windows のイベント ログには、詳細情報があります。</span><span class="sxs-lookup"><span data-stu-id="05bdd-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





