---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94ff2a645b9ea3862cee50ca086284deea02da09
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942018"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="36c99-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="36c99-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="36c99-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36c99-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36c99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36c99-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="36c99-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="36c99-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="36c99-107">Members</span></span>
|<span data-ttu-id="36c99-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="36c99-108">Member</span></span>|<span data-ttu-id="36c99-109">値</span><span class="sxs-lookup"><span data-stu-id="36c99-109">Value</span></span>|<span data-ttu-id="36c99-110">説明</span><span class="sxs-lookup"><span data-stu-id="36c99-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36c99-111">notRegistered 済み</span><span class="sxs-lookup"><span data-stu-id="36c99-111">notRegistered</span></span>|<span data-ttu-id="36c99-112">.0</span><span class="sxs-lookup"><span data-stu-id="36c99-112">0</span></span>|<span data-ttu-id="36c99-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="36c99-113">The device is not registered.</span></span>|
|<span data-ttu-id="36c99-114">い</span><span class="sxs-lookup"><span data-stu-id="36c99-114">registered</span></span>|<span data-ttu-id="36c99-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="36c99-115">2</span></span>|<span data-ttu-id="36c99-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="36c99-116">The device is registered.</span></span>|
|<span data-ttu-id="36c99-117">破棄</span><span class="sxs-lookup"><span data-stu-id="36c99-117">revoked</span></span>|<span data-ttu-id="36c99-118">1/3</span><span class="sxs-lookup"><span data-stu-id="36c99-118">3</span></span>|<span data-ttu-id="36c99-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="36c99-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="36c99-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="36c99-120">keyConflict</span></span>|<span data-ttu-id="36c99-121">2/4</span><span class="sxs-lookup"><span data-stu-id="36c99-121">4</span></span>|<span data-ttu-id="36c99-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="36c99-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="36c99-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="36c99-123">approvalPending</span></span>|<span data-ttu-id="36c99-124">5</span><span class="sxs-lookup"><span data-stu-id="36c99-124">5</span></span>|<span data-ttu-id="36c99-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="36c99-125">The device is pending approval.</span></span>|
|<span data-ttu-id="36c99-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="36c99-126">certificateReset</span></span>|<span data-ttu-id="36c99-127">シックス</span><span class="sxs-lookup"><span data-stu-id="36c99-127">6</span></span>|<span data-ttu-id="36c99-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="36c99-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="36c99-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="36c99-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="36c99-130">7</span><span class="sxs-lookup"><span data-stu-id="36c99-130">7</span></span>|<span data-ttu-id="36c99-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="36c99-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="36c99-132">不明</span><span class="sxs-lookup"><span data-stu-id="36c99-132">unknown</span></span>|<span data-ttu-id="36c99-133">8 </span><span class="sxs-lookup"><span data-stu-id="36c99-133">8</span></span>|<span data-ttu-id="36c99-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="36c99-134">The device registration status is unknown.</span></span>|




