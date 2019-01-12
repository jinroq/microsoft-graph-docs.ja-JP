---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6719dc370355c82d18c0a416cba02899ad03e183
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944265"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="4880a-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4880a-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="4880a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4880a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4880a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4880a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4880a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4880a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4880a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4880a-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="4880a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4880a-108">Members</span></span>
|<span data-ttu-id="4880a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4880a-109">Member</span></span>|<span data-ttu-id="4880a-110">値</span><span class="sxs-lookup"><span data-stu-id="4880a-110">Value</span></span>|<span data-ttu-id="4880a-111">説明</span><span class="sxs-lookup"><span data-stu-id="4880a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4880a-112">実行</span><span class="sxs-lookup"><span data-stu-id="4880a-112">running</span></span>|<span data-ttu-id="4880a-113">0</span><span class="sxs-lookup"><span data-stu-id="4880a-113">0</span></span>|<span data-ttu-id="4880a-114">実行中</span><span class="sxs-lookup"><span data-stu-id="4880a-114">Running</span></span>|
|<span data-ttu-id="4880a-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="4880a-115">rebootRequired</span></span>|<span data-ttu-id="4880a-116">1</span><span class="sxs-lookup"><span data-stu-id="4880a-116">1</span></span>|<span data-ttu-id="4880a-117">必要なルート</span><span class="sxs-lookup"><span data-stu-id="4880a-117">Root required</span></span>|
|<span data-ttu-id="4880a-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="4880a-118">require64BitArchitecture</span></span>|<span data-ttu-id="4880a-119">2</span><span class="sxs-lookup"><span data-stu-id="4880a-119">2</span></span>|<span data-ttu-id="4880a-120">必要な 64 ビット アーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="4880a-120">64 bit architecture required</span></span>|
|<span data-ttu-id="4880a-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="4880a-121">notLicensed</span></span>|<span data-ttu-id="4880a-122">3</span><span class="sxs-lookup"><span data-stu-id="4880a-122">3</span></span>|<span data-ttu-id="4880a-123">ライセンスがありません。</span><span class="sxs-lookup"><span data-stu-id="4880a-123">Not licensed</span></span>|
|<span data-ttu-id="4880a-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4880a-124">notConfigured</span></span>|<span data-ttu-id="4880a-125">4</span><span class="sxs-lookup"><span data-stu-id="4880a-125">4</span></span>|<span data-ttu-id="4880a-126">構成されていません</span><span class="sxs-lookup"><span data-stu-id="4880a-126">Not configured</span></span>|
|<span data-ttu-id="4880a-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="4880a-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="4880a-128">5</span><span class="sxs-lookup"><span data-stu-id="4880a-128">5</span></span>|<span data-ttu-id="4880a-129">システムがハードウェア要件を満たしていません。</span><span class="sxs-lookup"><span data-stu-id="4880a-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="4880a-130">その他の</span><span class="sxs-lookup"><span data-stu-id="4880a-130">other</span></span>|<span data-ttu-id="4880a-131">42</span><span class="sxs-lookup"><span data-stu-id="4880a-131">42</span></span>|<span data-ttu-id="4880a-132">他の。</span><span class="sxs-lookup"><span data-stu-id="4880a-132">Other.</span></span> <span data-ttu-id="4880a-133">DeviceGuard-マイクロソフトの Windows のイベント ログには、詳細情報があります。</span><span class="sxs-lookup"><span data-stu-id="4880a-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





