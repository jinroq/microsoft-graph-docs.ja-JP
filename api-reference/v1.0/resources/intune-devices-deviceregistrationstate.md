---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264135"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="6deb3-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="6deb3-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="6deb3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6deb3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6deb3-105">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="6deb3-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="6deb3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6deb3-106">Members</span></span>
|<span data-ttu-id="6deb3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6deb3-107">Member</span></span>|<span data-ttu-id="6deb3-108">値</span><span class="sxs-lookup"><span data-stu-id="6deb3-108">Value</span></span>|<span data-ttu-id="6deb3-109">説明</span><span class="sxs-lookup"><span data-stu-id="6deb3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6deb3-110">notregistered 済み</span><span class="sxs-lookup"><span data-stu-id="6deb3-110">notRegistered</span></span>|<span data-ttu-id="6deb3-111">.0</span><span class="sxs-lookup"><span data-stu-id="6deb3-111">0</span></span>|<span data-ttu-id="6deb3-112">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="6deb3-112">The device is not registered.</span></span>|
|<span data-ttu-id="6deb3-113">い</span><span class="sxs-lookup"><span data-stu-id="6deb3-113">registered</span></span>|<span data-ttu-id="6deb3-114">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6deb3-114">2</span></span>|<span data-ttu-id="6deb3-115">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="6deb3-115">The device is registered.</span></span>|
|<span data-ttu-id="6deb3-116">破棄</span><span class="sxs-lookup"><span data-stu-id="6deb3-116">revoked</span></span>|<span data-ttu-id="6deb3-117">1/3</span><span class="sxs-lookup"><span data-stu-id="6deb3-117">3</span></span>|<span data-ttu-id="6deb3-118">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="6deb3-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="6deb3-119">keyconflict</span><span class="sxs-lookup"><span data-stu-id="6deb3-119">keyConflict</span></span>|<span data-ttu-id="6deb3-120">2/4</span><span class="sxs-lookup"><span data-stu-id="6deb3-120">4</span></span>|<span data-ttu-id="6deb3-121">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="6deb3-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="6deb3-122">approvalpending</span><span class="sxs-lookup"><span data-stu-id="6deb3-122">approvalPending</span></span>|<span data-ttu-id="6deb3-123">5</span><span class="sxs-lookup"><span data-stu-id="6deb3-123">5</span></span>|<span data-ttu-id="6deb3-124">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="6deb3-124">The device is pending approval.</span></span>|
|<span data-ttu-id="6deb3-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="6deb3-125">certificateReset</span></span>|<span data-ttu-id="6deb3-126">シックス</span><span class="sxs-lookup"><span data-stu-id="6deb3-126">6</span></span>|<span data-ttu-id="6deb3-127">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="6deb3-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="6deb3-128">notregisteredpendingenrollment</span><span class="sxs-lookup"><span data-stu-id="6deb3-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="6deb3-129">7</span><span class="sxs-lookup"><span data-stu-id="6deb3-129">7</span></span>|<span data-ttu-id="6deb3-130">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="6deb3-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="6deb3-131">不明</span><span class="sxs-lookup"><span data-stu-id="6deb3-131">unknown</span></span>|<span data-ttu-id="6deb3-132">~</span><span class="sxs-lookup"><span data-stu-id="6deb3-132">8</span></span>|<span data-ttu-id="6deb3-133">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="6deb3-133">The device registration status is unknown.</span></span>|



