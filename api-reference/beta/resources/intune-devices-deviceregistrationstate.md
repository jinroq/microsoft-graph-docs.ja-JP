---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa2f009bc1a9fdafcabbbdbb4a5fbf5d2305b3a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995218"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="f145b-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f145b-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="f145b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f145b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f145b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f145b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f145b-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="f145b-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="f145b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f145b-107">Members</span></span>
|<span data-ttu-id="f145b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f145b-108">Member</span></span>|<span data-ttu-id="f145b-109">値</span><span class="sxs-lookup"><span data-stu-id="f145b-109">Value</span></span>|<span data-ttu-id="f145b-110">説明</span><span class="sxs-lookup"><span data-stu-id="f145b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f145b-111">notRegistered 済み</span><span class="sxs-lookup"><span data-stu-id="f145b-111">notRegistered</span></span>|<span data-ttu-id="f145b-112">.0</span><span class="sxs-lookup"><span data-stu-id="f145b-112">0</span></span>|<span data-ttu-id="f145b-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="f145b-113">The device is not registered.</span></span>|
|<span data-ttu-id="f145b-114">い</span><span class="sxs-lookup"><span data-stu-id="f145b-114">registered</span></span>|<span data-ttu-id="f145b-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f145b-115">2</span></span>|<span data-ttu-id="f145b-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="f145b-116">The device is registered.</span></span>|
|<span data-ttu-id="f145b-117">破棄</span><span class="sxs-lookup"><span data-stu-id="f145b-117">revoked</span></span>|<span data-ttu-id="f145b-118">1/3</span><span class="sxs-lookup"><span data-stu-id="f145b-118">3</span></span>|<span data-ttu-id="f145b-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="f145b-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="f145b-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="f145b-120">keyConflict</span></span>|<span data-ttu-id="f145b-121">2/4</span><span class="sxs-lookup"><span data-stu-id="f145b-121">4</span></span>|<span data-ttu-id="f145b-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="f145b-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="f145b-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="f145b-123">approvalPending</span></span>|<span data-ttu-id="f145b-124">5</span><span class="sxs-lookup"><span data-stu-id="f145b-124">5</span></span>|<span data-ttu-id="f145b-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="f145b-125">The device is pending approval.</span></span>|
|<span data-ttu-id="f145b-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="f145b-126">certificateReset</span></span>|<span data-ttu-id="f145b-127">シックス</span><span class="sxs-lookup"><span data-stu-id="f145b-127">6</span></span>|<span data-ttu-id="f145b-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="f145b-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="f145b-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="f145b-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="f145b-130">7</span><span class="sxs-lookup"><span data-stu-id="f145b-130">7</span></span>|<span data-ttu-id="f145b-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="f145b-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="f145b-132">不明</span><span class="sxs-lookup"><span data-stu-id="f145b-132">unknown</span></span>|<span data-ttu-id="f145b-133">8 </span><span class="sxs-lookup"><span data-stu-id="f145b-133">8</span></span>|<span data-ttu-id="f145b-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="f145b-134">The device registration status is unknown.</span></span>|





