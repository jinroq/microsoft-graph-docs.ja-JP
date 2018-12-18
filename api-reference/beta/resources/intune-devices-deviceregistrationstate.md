---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360544"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="8172c-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="8172c-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="8172c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8172c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8172c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8172c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8172c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8172c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8172c-107">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="8172c-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="8172c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8172c-108">Members</span></span>
|<span data-ttu-id="8172c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8172c-109">Member</span></span>|<span data-ttu-id="8172c-110">値</span><span class="sxs-lookup"><span data-stu-id="8172c-110">Value</span></span>|<span data-ttu-id="8172c-111">説明</span><span class="sxs-lookup"><span data-stu-id="8172c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8172c-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="8172c-112">notRegistered</span></span>|<span data-ttu-id="8172c-113">0</span><span class="sxs-lookup"><span data-stu-id="8172c-113">0</span></span>|<span data-ttu-id="8172c-114">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="8172c-114">The device is not registered.</span></span>|
|<span data-ttu-id="8172c-115">登録</span><span class="sxs-lookup"><span data-stu-id="8172c-115">registered</span></span>|<span data-ttu-id="8172c-116">2</span><span class="sxs-lookup"><span data-stu-id="8172c-116">2</span></span>|<span data-ttu-id="8172c-117">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="8172c-117">The device is registered.</span></span>|
|<span data-ttu-id="8172c-118">失効</span><span class="sxs-lookup"><span data-stu-id="8172c-118">revoked</span></span>|<span data-ttu-id="8172c-119">3</span><span class="sxs-lookup"><span data-stu-id="8172c-119">3</span></span>|<span data-ttu-id="8172c-120">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="8172c-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="8172c-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="8172c-121">keyConflict</span></span>|<span data-ttu-id="8172c-122">4</span><span class="sxs-lookup"><span data-stu-id="8172c-122">4</span></span>|<span data-ttu-id="8172c-123">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="8172c-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="8172c-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="8172c-124">approvalPending</span></span>|<span data-ttu-id="8172c-125">5</span><span class="sxs-lookup"><span data-stu-id="8172c-125">5</span></span>|<span data-ttu-id="8172c-126">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="8172c-126">The device is pending approval.</span></span>|
|<span data-ttu-id="8172c-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="8172c-127">certificateReset</span></span>|<span data-ttu-id="8172c-128">6</span><span class="sxs-lookup"><span data-stu-id="8172c-128">6</span></span>|<span data-ttu-id="8172c-129">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="8172c-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="8172c-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="8172c-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="8172c-131">7</span><span class="sxs-lookup"><span data-stu-id="8172c-131">7</span></span>|<span data-ttu-id="8172c-132">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="8172c-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="8172c-133">不明</span><span class="sxs-lookup"><span data-stu-id="8172c-133">unknown</span></span>|<span data-ttu-id="8172c-134">8</span><span class="sxs-lookup"><span data-stu-id="8172c-134">8</span></span>|<span data-ttu-id="8172c-135">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="8172c-135">The device registration status is unknown.</span></span>|





