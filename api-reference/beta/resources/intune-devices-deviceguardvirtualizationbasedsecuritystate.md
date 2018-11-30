---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
ms.openlocfilehash: 719916717f711fa9230bc111e12d492557329830
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073775"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="81210-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="81210-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="81210-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81210-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81210-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81210-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81210-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81210-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81210-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="81210-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="81210-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81210-108">Members</span></span>
|<span data-ttu-id="81210-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="81210-109">Member</span></span>|<span data-ttu-id="81210-110">値</span><span class="sxs-lookup"><span data-stu-id="81210-110">Value</span></span>|<span data-ttu-id="81210-111">説明</span><span class="sxs-lookup"><span data-stu-id="81210-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81210-112">実行</span><span class="sxs-lookup"><span data-stu-id="81210-112">running</span></span>|<span data-ttu-id="81210-113">0</span><span class="sxs-lookup"><span data-stu-id="81210-113">0</span></span>|<span data-ttu-id="81210-114">実行中</span><span class="sxs-lookup"><span data-stu-id="81210-114">Running</span></span>|
|<span data-ttu-id="81210-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="81210-115">rebootRequired</span></span>|<span data-ttu-id="81210-116">1</span><span class="sxs-lookup"><span data-stu-id="81210-116">1</span></span>|<span data-ttu-id="81210-117">必要なルート</span><span class="sxs-lookup"><span data-stu-id="81210-117">Root required</span></span>|
|<span data-ttu-id="81210-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="81210-118">require64BitArchitecture</span></span>|<span data-ttu-id="81210-119">2</span><span class="sxs-lookup"><span data-stu-id="81210-119">2</span></span>|<span data-ttu-id="81210-120">必要な 64 ビット アーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="81210-120">64 bit architecture required</span></span>|
|<span data-ttu-id="81210-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="81210-121">notLicensed</span></span>|<span data-ttu-id="81210-122">3</span><span class="sxs-lookup"><span data-stu-id="81210-122">3</span></span>|<span data-ttu-id="81210-123">ライセンスがありません。</span><span class="sxs-lookup"><span data-stu-id="81210-123">Not licensed</span></span>|
|<span data-ttu-id="81210-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="81210-124">notConfigured</span></span>|<span data-ttu-id="81210-125">4</span><span class="sxs-lookup"><span data-stu-id="81210-125">4</span></span>|<span data-ttu-id="81210-126">構成されていません</span><span class="sxs-lookup"><span data-stu-id="81210-126">Not configured</span></span>|
|<span data-ttu-id="81210-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="81210-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="81210-128">5</span><span class="sxs-lookup"><span data-stu-id="81210-128">5</span></span>|<span data-ttu-id="81210-129">システムがハードウェア要件を満たしていません。</span><span class="sxs-lookup"><span data-stu-id="81210-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="81210-130">その他の</span><span class="sxs-lookup"><span data-stu-id="81210-130">other</span></span>|<span data-ttu-id="81210-131">42</span><span class="sxs-lookup"><span data-stu-id="81210-131">42</span></span>|<span data-ttu-id="81210-132">他の。</span><span class="sxs-lookup"><span data-stu-id="81210-132">Other.</span></span> <span data-ttu-id="81210-133">DeviceGuard-マイクロソフトの Windows のイベント ログには、詳細情報があります。</span><span class="sxs-lookup"><span data-stu-id="81210-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





