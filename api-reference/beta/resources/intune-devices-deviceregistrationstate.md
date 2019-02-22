---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04d8c0fddb966504675e3b4c677dfd0bbabe64c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144626"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="d925c-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="d925c-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="d925c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d925c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d925c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d925c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d925c-106">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="d925c-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="d925c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d925c-107">Members</span></span>
|<span data-ttu-id="d925c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d925c-108">Member</span></span>|<span data-ttu-id="d925c-109">値</span><span class="sxs-lookup"><span data-stu-id="d925c-109">Value</span></span>|<span data-ttu-id="d925c-110">説明</span><span class="sxs-lookup"><span data-stu-id="d925c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d925c-111">notregistered 済み</span><span class="sxs-lookup"><span data-stu-id="d925c-111">notRegistered</span></span>|<span data-ttu-id="d925c-112">.0</span><span class="sxs-lookup"><span data-stu-id="d925c-112">0</span></span>|<span data-ttu-id="d925c-113">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="d925c-113">The device is not registered.</span></span>|
|<span data-ttu-id="d925c-114">い</span><span class="sxs-lookup"><span data-stu-id="d925c-114">registered</span></span>|<span data-ttu-id="d925c-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d925c-115">2</span></span>|<span data-ttu-id="d925c-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="d925c-116">The device is registered.</span></span>|
|<span data-ttu-id="d925c-117">破棄</span><span class="sxs-lookup"><span data-stu-id="d925c-117">revoked</span></span>|<span data-ttu-id="d925c-118">1/3</span><span class="sxs-lookup"><span data-stu-id="d925c-118">3</span></span>|<span data-ttu-id="d925c-119">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="d925c-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="d925c-120">keyconflict</span><span class="sxs-lookup"><span data-stu-id="d925c-120">keyConflict</span></span>|<span data-ttu-id="d925c-121">2/4</span><span class="sxs-lookup"><span data-stu-id="d925c-121">4</span></span>|<span data-ttu-id="d925c-122">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="d925c-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="d925c-123">approvalpending</span><span class="sxs-lookup"><span data-stu-id="d925c-123">approvalPending</span></span>|<span data-ttu-id="d925c-124">5</span><span class="sxs-lookup"><span data-stu-id="d925c-124">5</span></span>|<span data-ttu-id="d925c-125">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="d925c-125">The device is pending approval.</span></span>|
|<span data-ttu-id="d925c-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="d925c-126">certificateReset</span></span>|<span data-ttu-id="d925c-127">シックス</span><span class="sxs-lookup"><span data-stu-id="d925c-127">6</span></span>|<span data-ttu-id="d925c-128">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="d925c-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="d925c-129">notregisteredpendingenrollment</span><span class="sxs-lookup"><span data-stu-id="d925c-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="d925c-130">7</span><span class="sxs-lookup"><span data-stu-id="d925c-130">7</span></span>|<span data-ttu-id="d925c-131">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="d925c-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="d925c-132">不明</span><span class="sxs-lookup"><span data-stu-id="d925c-132">unknown</span></span>|<span data-ttu-id="d925c-133">~</span><span class="sxs-lookup"><span data-stu-id="d925c-133">8</span></span>|<span data-ttu-id="d925c-134">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="d925c-134">The device registration status is unknown.</span></span>|




