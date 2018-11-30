---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
ms.openlocfilehash: 9f9ee23d385ce4a7fca73e2d296c3f34063fc218
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020589"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="83fa3-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="83fa3-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="83fa3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83fa3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83fa3-105">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="83fa3-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="83fa3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="83fa3-106">Members</span></span>
|<span data-ttu-id="83fa3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="83fa3-107">Member</span></span>|<span data-ttu-id="83fa3-108">値</span><span class="sxs-lookup"><span data-stu-id="83fa3-108">Value</span></span>|<span data-ttu-id="83fa3-109">説明</span><span class="sxs-lookup"><span data-stu-id="83fa3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83fa3-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="83fa3-110">notRegistered</span></span>|<span data-ttu-id="83fa3-111">0</span><span class="sxs-lookup"><span data-stu-id="83fa3-111">0</span></span>|<span data-ttu-id="83fa3-112">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="83fa3-112">The device is not registered.</span></span>|
|<span data-ttu-id="83fa3-113">登録</span><span class="sxs-lookup"><span data-stu-id="83fa3-113">registered</span></span>|<span data-ttu-id="83fa3-114">2</span><span class="sxs-lookup"><span data-stu-id="83fa3-114">2</span></span>|<span data-ttu-id="83fa3-115">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="83fa3-115">The device is registered.</span></span>|
|<span data-ttu-id="83fa3-116">失効</span><span class="sxs-lookup"><span data-stu-id="83fa3-116">revoked</span></span>|<span data-ttu-id="83fa3-117">3</span><span class="sxs-lookup"><span data-stu-id="83fa3-117">3</span></span>|<span data-ttu-id="83fa3-118">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="83fa3-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="83fa3-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="83fa3-119">keyConflict</span></span>|<span data-ttu-id="83fa3-120">4</span><span class="sxs-lookup"><span data-stu-id="83fa3-120">4</span></span>|<span data-ttu-id="83fa3-121">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="83fa3-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="83fa3-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="83fa3-122">approvalPending</span></span>|<span data-ttu-id="83fa3-123">5</span><span class="sxs-lookup"><span data-stu-id="83fa3-123">5</span></span>|<span data-ttu-id="83fa3-124">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="83fa3-124">The device is pending approval.</span></span>|
|<span data-ttu-id="83fa3-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="83fa3-125">certificateReset</span></span>|<span data-ttu-id="83fa3-126">6</span><span class="sxs-lookup"><span data-stu-id="83fa3-126">6</span></span>|<span data-ttu-id="83fa3-127">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="83fa3-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="83fa3-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="83fa3-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="83fa3-129">7</span><span class="sxs-lookup"><span data-stu-id="83fa3-129">7</span></span>|<span data-ttu-id="83fa3-130">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="83fa3-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="83fa3-131">不明</span><span class="sxs-lookup"><span data-stu-id="83fa3-131">unknown</span></span>|<span data-ttu-id="83fa3-132">8</span><span class="sxs-lookup"><span data-stu-id="83fa3-132">8</span></span>|<span data-ttu-id="83fa3-133">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="83fa3-133">The device registration status is unknown.</span></span>|



