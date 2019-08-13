---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 92171fb3e9fc50e516ed4568cceea03c5e0ba1cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369935"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="4a2af-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a2af-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="4a2af-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a2af-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a2af-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="4a2af-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="4a2af-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a2af-107">Members</span></span>
|<span data-ttu-id="4a2af-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a2af-108">Member</span></span>|<span data-ttu-id="4a2af-109">値</span><span class="sxs-lookup"><span data-stu-id="4a2af-109">Value</span></span>|<span data-ttu-id="4a2af-110">説明</span><span class="sxs-lookup"><span data-stu-id="4a2af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a2af-111">notRegistered 済み</span><span class="sxs-lookup"><span data-stu-id="4a2af-111">notRegistered</span></span>|<span data-ttu-id="4a2af-112">.0</span><span class="sxs-lookup"><span data-stu-id="4a2af-112">0</span></span>|<span data-ttu-id="4a2af-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="4a2af-113">The device is not registered.</span></span>|
|<span data-ttu-id="4a2af-114">い</span><span class="sxs-lookup"><span data-stu-id="4a2af-114">registered</span></span>|<span data-ttu-id="4a2af-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4a2af-115">2</span></span>|<span data-ttu-id="4a2af-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="4a2af-116">The device is registered.</span></span>|
|<span data-ttu-id="4a2af-117">破棄</span><span class="sxs-lookup"><span data-stu-id="4a2af-117">revoked</span></span>|<span data-ttu-id="4a2af-118">1/3</span><span class="sxs-lookup"><span data-stu-id="4a2af-118">3</span></span>|<span data-ttu-id="4a2af-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="4a2af-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="4a2af-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="4a2af-120">keyConflict</span></span>|<span data-ttu-id="4a2af-121">2/4</span><span class="sxs-lookup"><span data-stu-id="4a2af-121">4</span></span>|<span data-ttu-id="4a2af-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="4a2af-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="4a2af-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="4a2af-123">approvalPending</span></span>|<span data-ttu-id="4a2af-124">5</span><span class="sxs-lookup"><span data-stu-id="4a2af-124">5</span></span>|<span data-ttu-id="4a2af-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="4a2af-125">The device is pending approval.</span></span>|
|<span data-ttu-id="4a2af-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="4a2af-126">certificateReset</span></span>|<span data-ttu-id="4a2af-127">シックス</span><span class="sxs-lookup"><span data-stu-id="4a2af-127">6</span></span>|<span data-ttu-id="4a2af-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="4a2af-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="4a2af-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="4a2af-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="4a2af-130">7</span><span class="sxs-lookup"><span data-stu-id="4a2af-130">7</span></span>|<span data-ttu-id="4a2af-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="4a2af-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="4a2af-132">不明</span><span class="sxs-lookup"><span data-stu-id="4a2af-132">unknown</span></span>|<span data-ttu-id="4a2af-133">8 </span><span class="sxs-lookup"><span data-stu-id="4a2af-133">8</span></span>|<span data-ttu-id="4a2af-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="4a2af-134">The device registration status is unknown.</span></span>|



