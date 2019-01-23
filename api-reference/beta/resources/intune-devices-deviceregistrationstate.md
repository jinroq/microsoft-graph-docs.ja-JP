---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396757"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="f3aa9-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f3aa9-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="f3aa9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3aa9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3aa9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3aa9-107">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="f3aa9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3aa9-108">Members</span></span>
|<span data-ttu-id="f3aa9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3aa9-109">Member</span></span>|<span data-ttu-id="f3aa9-110">値</span><span class="sxs-lookup"><span data-stu-id="f3aa9-110">Value</span></span>|<span data-ttu-id="f3aa9-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3aa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3aa9-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="f3aa9-112">notRegistered</span></span>|<span data-ttu-id="f3aa9-113">0</span><span class="sxs-lookup"><span data-stu-id="f3aa9-113">0</span></span>|<span data-ttu-id="f3aa9-114">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-114">The device is not registered.</span></span>|
|<span data-ttu-id="f3aa9-115">登録</span><span class="sxs-lookup"><span data-stu-id="f3aa9-115">registered</span></span>|<span data-ttu-id="f3aa9-116">2</span><span class="sxs-lookup"><span data-stu-id="f3aa9-116">2</span></span>|<span data-ttu-id="f3aa9-117">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-117">The device is registered.</span></span>|
|<span data-ttu-id="f3aa9-118">失効</span><span class="sxs-lookup"><span data-stu-id="f3aa9-118">revoked</span></span>|<span data-ttu-id="f3aa9-119">3</span><span class="sxs-lookup"><span data-stu-id="f3aa9-119">3</span></span>|<span data-ttu-id="f3aa9-120">デバイスがブロックされている、消去した廃止します。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="f3aa9-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="f3aa9-121">keyConflict</span></span>|<span data-ttu-id="f3aa9-122">4</span><span class="sxs-lookup"><span data-stu-id="f3aa9-122">4</span></span>|<span data-ttu-id="f3aa9-123">デバイスには、キーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="f3aa9-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="f3aa9-124">approvalPending</span></span>|<span data-ttu-id="f3aa9-125">5</span><span class="sxs-lookup"><span data-stu-id="f3aa9-125">5</span></span>|<span data-ttu-id="f3aa9-126">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-126">The device is pending approval.</span></span>|
|<span data-ttu-id="f3aa9-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="f3aa9-127">certificateReset</span></span>|<span data-ttu-id="f3aa9-128">6</span><span class="sxs-lookup"><span data-stu-id="f3aa9-128">6</span></span>|<span data-ttu-id="f3aa9-129">デバイスの証明書をリセットするとします。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="f3aa9-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="f3aa9-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="f3aa9-131">7</span><span class="sxs-lookup"><span data-stu-id="f3aa9-131">7</span></span>|<span data-ttu-id="f3aa9-132">デバイスが登録されていないと登録を保留中です。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="f3aa9-133">不明</span><span class="sxs-lookup"><span data-stu-id="f3aa9-133">unknown</span></span>|<span data-ttu-id="f3aa9-134">8</span><span class="sxs-lookup"><span data-stu-id="f3aa9-134">8</span></span>|<span data-ttu-id="f3aa9-135">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="f3aa9-135">The device registration status is unknown.</span></span>|




