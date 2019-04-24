---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522385"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="94614-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="94614-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="94614-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94614-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94614-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94614-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94614-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="94614-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="94614-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="94614-107">Members</span></span>
|<span data-ttu-id="94614-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="94614-108">Member</span></span>|<span data-ttu-id="94614-109">値</span><span class="sxs-lookup"><span data-stu-id="94614-109">Value</span></span>|<span data-ttu-id="94614-110">説明</span><span class="sxs-lookup"><span data-stu-id="94614-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94614-111">notregistered 済み</span><span class="sxs-lookup"><span data-stu-id="94614-111">notRegistered</span></span>|<span data-ttu-id="94614-112">.0</span><span class="sxs-lookup"><span data-stu-id="94614-112">0</span></span>|<span data-ttu-id="94614-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="94614-113">The device is not registered.</span></span>|
|<span data-ttu-id="94614-114">い</span><span class="sxs-lookup"><span data-stu-id="94614-114">registered</span></span>|<span data-ttu-id="94614-115">2 </span><span class="sxs-lookup"><span data-stu-id="94614-115">2</span></span>|<span data-ttu-id="94614-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="94614-116">The device is registered.</span></span>|
|<span data-ttu-id="94614-117">破棄</span><span class="sxs-lookup"><span data-stu-id="94614-117">revoked</span></span>|<span data-ttu-id="94614-118">3 </span><span class="sxs-lookup"><span data-stu-id="94614-118">3</span></span>|<span data-ttu-id="94614-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="94614-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="94614-120">keyconflict</span><span class="sxs-lookup"><span data-stu-id="94614-120">keyConflict</span></span>|<span data-ttu-id="94614-121">4 </span><span class="sxs-lookup"><span data-stu-id="94614-121">4</span></span>|<span data-ttu-id="94614-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="94614-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="94614-123">approvalpending</span><span class="sxs-lookup"><span data-stu-id="94614-123">approvalPending</span></span>|<span data-ttu-id="94614-124">5 </span><span class="sxs-lookup"><span data-stu-id="94614-124">5</span></span>|<span data-ttu-id="94614-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="94614-125">The device is pending approval.</span></span>|
|<span data-ttu-id="94614-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="94614-126">certificateReset</span></span>|<span data-ttu-id="94614-127">6 </span><span class="sxs-lookup"><span data-stu-id="94614-127">6</span></span>|<span data-ttu-id="94614-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="94614-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="94614-129">notregisteredpendingenrollment</span><span class="sxs-lookup"><span data-stu-id="94614-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="94614-130">7 </span><span class="sxs-lookup"><span data-stu-id="94614-130">7</span></span>|<span data-ttu-id="94614-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="94614-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="94614-132">不明</span><span class="sxs-lookup"><span data-stu-id="94614-132">unknown</span></span>|<span data-ttu-id="94614-133">8 </span><span class="sxs-lookup"><span data-stu-id="94614-133">8</span></span>|<span data-ttu-id="94614-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="94614-134">The device registration status is unknown.</span></span>|





