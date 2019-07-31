---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e153ac5c1bfbd09540fd55b5df23eab095e2a002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968387"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="978e3-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="978e3-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="978e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="978e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="978e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="978e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978e3-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="978e3-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="978e3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="978e3-107">Members</span></span>
|<span data-ttu-id="978e3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="978e3-108">Member</span></span>|<span data-ttu-id="978e3-109">値</span><span class="sxs-lookup"><span data-stu-id="978e3-109">Value</span></span>|<span data-ttu-id="978e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="978e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978e3-111">notRegistered 済み</span><span class="sxs-lookup"><span data-stu-id="978e3-111">notRegistered</span></span>|<span data-ttu-id="978e3-112">.0</span><span class="sxs-lookup"><span data-stu-id="978e3-112">0</span></span>|<span data-ttu-id="978e3-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="978e3-113">The device is not registered.</span></span>|
|<span data-ttu-id="978e3-114">い</span><span class="sxs-lookup"><span data-stu-id="978e3-114">registered</span></span>|<span data-ttu-id="978e3-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="978e3-115">2</span></span>|<span data-ttu-id="978e3-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="978e3-116">The device is registered.</span></span>|
|<span data-ttu-id="978e3-117">破棄</span><span class="sxs-lookup"><span data-stu-id="978e3-117">revoked</span></span>|<span data-ttu-id="978e3-118">1/3</span><span class="sxs-lookup"><span data-stu-id="978e3-118">3</span></span>|<span data-ttu-id="978e3-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="978e3-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="978e3-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="978e3-120">keyConflict</span></span>|<span data-ttu-id="978e3-121">2/4</span><span class="sxs-lookup"><span data-stu-id="978e3-121">4</span></span>|<span data-ttu-id="978e3-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="978e3-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="978e3-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="978e3-123">approvalPending</span></span>|<span data-ttu-id="978e3-124">5</span><span class="sxs-lookup"><span data-stu-id="978e3-124">5</span></span>|<span data-ttu-id="978e3-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="978e3-125">The device is pending approval.</span></span>|
|<span data-ttu-id="978e3-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="978e3-126">certificateReset</span></span>|<span data-ttu-id="978e3-127">シックス</span><span class="sxs-lookup"><span data-stu-id="978e3-127">6</span></span>|<span data-ttu-id="978e3-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="978e3-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="978e3-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="978e3-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="978e3-130">7</span><span class="sxs-lookup"><span data-stu-id="978e3-130">7</span></span>|<span data-ttu-id="978e3-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="978e3-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="978e3-132">不明</span><span class="sxs-lookup"><span data-stu-id="978e3-132">unknown</span></span>|<span data-ttu-id="978e3-133">8 </span><span class="sxs-lookup"><span data-stu-id="978e3-133">8</span></span>|<span data-ttu-id="978e3-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="978e3-134">The device registration status is unknown.</span></span>|





