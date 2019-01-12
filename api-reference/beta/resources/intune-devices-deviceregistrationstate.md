---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6d6b38beb34b8725587d9284dd524008320bba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961863"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="378e4-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="378e4-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="378e4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="378e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="378e4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="378e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="378e4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="378e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="378e4-107">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="378e4-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="378e4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="378e4-108">Members</span></span>
|<span data-ttu-id="378e4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="378e4-109">Member</span></span>|<span data-ttu-id="378e4-110">値</span><span class="sxs-lookup"><span data-stu-id="378e4-110">Value</span></span>|<span data-ttu-id="378e4-111">説明</span><span class="sxs-lookup"><span data-stu-id="378e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="378e4-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="378e4-112">notRegistered</span></span>|<span data-ttu-id="378e4-113">0</span><span class="sxs-lookup"><span data-stu-id="378e4-113">0</span></span>|<span data-ttu-id="378e4-114">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="378e4-114">The device is not registered.</span></span>|
|<span data-ttu-id="378e4-115">登録</span><span class="sxs-lookup"><span data-stu-id="378e4-115">registered</span></span>|<span data-ttu-id="378e4-116">2</span><span class="sxs-lookup"><span data-stu-id="378e4-116">2</span></span>|<span data-ttu-id="378e4-117">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="378e4-117">The device is registered.</span></span>|
|<span data-ttu-id="378e4-118">失効</span><span class="sxs-lookup"><span data-stu-id="378e4-118">revoked</span></span>|<span data-ttu-id="378e4-119">3</span><span class="sxs-lookup"><span data-stu-id="378e4-119">3</span></span>|<span data-ttu-id="378e4-120">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="378e4-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="378e4-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="378e4-121">keyConflict</span></span>|<span data-ttu-id="378e4-122">4</span><span class="sxs-lookup"><span data-stu-id="378e4-122">4</span></span>|<span data-ttu-id="378e4-123">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="378e4-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="378e4-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="378e4-124">approvalPending</span></span>|<span data-ttu-id="378e4-125">5</span><span class="sxs-lookup"><span data-stu-id="378e4-125">5</span></span>|<span data-ttu-id="378e4-126">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="378e4-126">The device is pending approval.</span></span>|
|<span data-ttu-id="378e4-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="378e4-127">certificateReset</span></span>|<span data-ttu-id="378e4-128">6</span><span class="sxs-lookup"><span data-stu-id="378e4-128">6</span></span>|<span data-ttu-id="378e4-129">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="378e4-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="378e4-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="378e4-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="378e4-131">7</span><span class="sxs-lookup"><span data-stu-id="378e4-131">7</span></span>|<span data-ttu-id="378e4-132">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="378e4-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="378e4-133">不明</span><span class="sxs-lookup"><span data-stu-id="378e4-133">unknown</span></span>|<span data-ttu-id="378e4-134">8</span><span class="sxs-lookup"><span data-stu-id="378e4-134">8</span></span>|<span data-ttu-id="378e4-135">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="378e4-135">The device registration status is unknown.</span></span>|





