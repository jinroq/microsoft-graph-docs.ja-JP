---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580975"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="42682-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="42682-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="42682-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42682-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42682-105">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="42682-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="42682-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="42682-106">Members</span></span>
|<span data-ttu-id="42682-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="42682-107">Member</span></span>|<span data-ttu-id="42682-108">値</span><span class="sxs-lookup"><span data-stu-id="42682-108">Value</span></span>|<span data-ttu-id="42682-109">説明</span><span class="sxs-lookup"><span data-stu-id="42682-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42682-110">notregistered 済み</span><span class="sxs-lookup"><span data-stu-id="42682-110">notRegistered</span></span>|<span data-ttu-id="42682-111">.0</span><span class="sxs-lookup"><span data-stu-id="42682-111">0</span></span>|<span data-ttu-id="42682-112">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="42682-112">The device is not registered.</span></span>|
|<span data-ttu-id="42682-113">い</span><span class="sxs-lookup"><span data-stu-id="42682-113">registered</span></span>|<span data-ttu-id="42682-114">2 </span><span class="sxs-lookup"><span data-stu-id="42682-114">2</span></span>|<span data-ttu-id="42682-115">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="42682-115">The device is registered.</span></span>|
|<span data-ttu-id="42682-116">破棄</span><span class="sxs-lookup"><span data-stu-id="42682-116">revoked</span></span>|<span data-ttu-id="42682-117">3 </span><span class="sxs-lookup"><span data-stu-id="42682-117">3</span></span>|<span data-ttu-id="42682-118">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="42682-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="42682-119">keyconflict</span><span class="sxs-lookup"><span data-stu-id="42682-119">keyConflict</span></span>|<span data-ttu-id="42682-120">4 </span><span class="sxs-lookup"><span data-stu-id="42682-120">4</span></span>|<span data-ttu-id="42682-121">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="42682-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="42682-122">approvalpending</span><span class="sxs-lookup"><span data-stu-id="42682-122">approvalPending</span></span>|<span data-ttu-id="42682-123">5 </span><span class="sxs-lookup"><span data-stu-id="42682-123">5</span></span>|<span data-ttu-id="42682-124">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="42682-124">The device is pending approval.</span></span>|
|<span data-ttu-id="42682-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="42682-125">certificateReset</span></span>|<span data-ttu-id="42682-126">6 </span><span class="sxs-lookup"><span data-stu-id="42682-126">6</span></span>|<span data-ttu-id="42682-127">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="42682-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="42682-128">notregisteredpendingenrollment</span><span class="sxs-lookup"><span data-stu-id="42682-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="42682-129">7 </span><span class="sxs-lookup"><span data-stu-id="42682-129">7</span></span>|<span data-ttu-id="42682-130">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="42682-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="42682-131">不明</span><span class="sxs-lookup"><span data-stu-id="42682-131">unknown</span></span>|<span data-ttu-id="42682-132">8 </span><span class="sxs-lookup"><span data-stu-id="42682-132">8</span></span>|<span data-ttu-id="42682-133">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="42682-133">The device registration status is unknown.</span></span>|



