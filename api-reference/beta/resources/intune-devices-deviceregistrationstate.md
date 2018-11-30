---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
ms.openlocfilehash: 5496bce53e061894a829745fce0687815c855c01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073447"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a7ce3-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="a7ce3-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="a7ce3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7ce3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7ce3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7ce3-107">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="a7ce3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7ce3-108">Members</span></span>
|<span data-ttu-id="a7ce3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7ce3-109">Member</span></span>|<span data-ttu-id="a7ce3-110">値</span><span class="sxs-lookup"><span data-stu-id="a7ce3-110">Value</span></span>|<span data-ttu-id="a7ce3-111">説明</span><span class="sxs-lookup"><span data-stu-id="a7ce3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ce3-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="a7ce3-112">notRegistered</span></span>|<span data-ttu-id="a7ce3-113">0</span><span class="sxs-lookup"><span data-stu-id="a7ce3-113">0</span></span>|<span data-ttu-id="a7ce3-114">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-114">The device is not registered.</span></span>|
|<span data-ttu-id="a7ce3-115">登録</span><span class="sxs-lookup"><span data-stu-id="a7ce3-115">registered</span></span>|<span data-ttu-id="a7ce3-116">2</span><span class="sxs-lookup"><span data-stu-id="a7ce3-116">2</span></span>|<span data-ttu-id="a7ce3-117">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-117">The device is registered.</span></span>|
|<span data-ttu-id="a7ce3-118">失効</span><span class="sxs-lookup"><span data-stu-id="a7ce3-118">revoked</span></span>|<span data-ttu-id="a7ce3-119">3</span><span class="sxs-lookup"><span data-stu-id="a7ce3-119">3</span></span>|<span data-ttu-id="a7ce3-120">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a7ce3-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="a7ce3-121">keyConflict</span></span>|<span data-ttu-id="a7ce3-122">4</span><span class="sxs-lookup"><span data-stu-id="a7ce3-122">4</span></span>|<span data-ttu-id="a7ce3-123">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="a7ce3-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a7ce3-124">approvalPending</span></span>|<span data-ttu-id="a7ce3-125">5</span><span class="sxs-lookup"><span data-stu-id="a7ce3-125">5</span></span>|<span data-ttu-id="a7ce3-126">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-126">The device is pending approval.</span></span>|
|<span data-ttu-id="a7ce3-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a7ce3-127">certificateReset</span></span>|<span data-ttu-id="a7ce3-128">6</span><span class="sxs-lookup"><span data-stu-id="a7ce3-128">6</span></span>|<span data-ttu-id="a7ce3-129">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a7ce3-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a7ce3-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a7ce3-131">7</span><span class="sxs-lookup"><span data-stu-id="a7ce3-131">7</span></span>|<span data-ttu-id="a7ce3-132">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a7ce3-133">不明</span><span class="sxs-lookup"><span data-stu-id="a7ce3-133">unknown</span></span>|<span data-ttu-id="a7ce3-134">8</span><span class="sxs-lookup"><span data-stu-id="a7ce3-134">8</span></span>|<span data-ttu-id="a7ce3-135">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="a7ce3-135">The device registration status is unknown.</span></span>|





