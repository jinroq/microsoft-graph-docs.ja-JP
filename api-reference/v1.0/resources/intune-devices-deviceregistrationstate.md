---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
author: tfitzmac
ms.openlocfilehash: 9fdd5cd3a63472e841f0d97f8cbee3a0f548380d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320091"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="faa41-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="faa41-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="faa41-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="faa41-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faa41-105">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="faa41-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="faa41-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="faa41-106">Members</span></span>
|<span data-ttu-id="faa41-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="faa41-107">Member</span></span>|<span data-ttu-id="faa41-108">値</span><span class="sxs-lookup"><span data-stu-id="faa41-108">Value</span></span>|<span data-ttu-id="faa41-109">説明</span><span class="sxs-lookup"><span data-stu-id="faa41-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa41-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="faa41-110">notRegistered</span></span>|<span data-ttu-id="faa41-111">0</span><span class="sxs-lookup"><span data-stu-id="faa41-111">0</span></span>|<span data-ttu-id="faa41-112">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="faa41-112">The device is not registered.</span></span>|
|<span data-ttu-id="faa41-113">登録</span><span class="sxs-lookup"><span data-stu-id="faa41-113">registered</span></span>|<span data-ttu-id="faa41-114">2</span><span class="sxs-lookup"><span data-stu-id="faa41-114">2</span></span>|<span data-ttu-id="faa41-115">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="faa41-115">The device is registered.</span></span>|
|<span data-ttu-id="faa41-116">失効</span><span class="sxs-lookup"><span data-stu-id="faa41-116">revoked</span></span>|<span data-ttu-id="faa41-117">3</span><span class="sxs-lookup"><span data-stu-id="faa41-117">3</span></span>|<span data-ttu-id="faa41-118">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="faa41-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="faa41-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="faa41-119">keyConflict</span></span>|<span data-ttu-id="faa41-120">4</span><span class="sxs-lookup"><span data-stu-id="faa41-120">4</span></span>|<span data-ttu-id="faa41-121">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="faa41-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="faa41-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="faa41-122">approvalPending</span></span>|<span data-ttu-id="faa41-123">5</span><span class="sxs-lookup"><span data-stu-id="faa41-123">5</span></span>|<span data-ttu-id="faa41-124">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="faa41-124">The device is pending approval.</span></span>|
|<span data-ttu-id="faa41-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="faa41-125">certificateReset</span></span>|<span data-ttu-id="faa41-126">6</span><span class="sxs-lookup"><span data-stu-id="faa41-126">6</span></span>|<span data-ttu-id="faa41-127">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="faa41-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="faa41-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="faa41-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="faa41-129">7</span><span class="sxs-lookup"><span data-stu-id="faa41-129">7</span></span>|<span data-ttu-id="faa41-130">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="faa41-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="faa41-131">不明</span><span class="sxs-lookup"><span data-stu-id="faa41-131">unknown</span></span>|<span data-ttu-id="faa41-132">8</span><span class="sxs-lookup"><span data-stu-id="faa41-132">8</span></span>|<span data-ttu-id="faa41-133">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="faa41-133">The device registration status is unknown.</span></span>|



