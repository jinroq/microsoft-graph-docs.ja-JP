---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 933ea7cf16421ecadd9bb23b4594d8ca0f5e767b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030731"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="105bd-103">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="105bd-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="105bd-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="105bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="105bd-105">デバイス登録の状態。</span><span class="sxs-lookup"><span data-stu-id="105bd-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="105bd-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="105bd-106">Members</span></span>
|<span data-ttu-id="105bd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="105bd-107">Member</span></span>|<span data-ttu-id="105bd-108">値</span><span class="sxs-lookup"><span data-stu-id="105bd-108">Value</span></span>|<span data-ttu-id="105bd-109">説明</span><span class="sxs-lookup"><span data-stu-id="105bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="105bd-110">notRegistered 済み</span><span class="sxs-lookup"><span data-stu-id="105bd-110">notRegistered</span></span>|<span data-ttu-id="105bd-111">.0</span><span class="sxs-lookup"><span data-stu-id="105bd-111">0</span></span>|<span data-ttu-id="105bd-112">デバイスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="105bd-112">The device is not registered.</span></span>|
|<span data-ttu-id="105bd-113">い</span><span class="sxs-lookup"><span data-stu-id="105bd-113">registered</span></span>|<span data-ttu-id="105bd-114">pbm-2</span><span class="sxs-lookup"><span data-stu-id="105bd-114">2</span></span>|<span data-ttu-id="105bd-115">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="105bd-115">The device is registered.</span></span>|
|<span data-ttu-id="105bd-116">破棄</span><span class="sxs-lookup"><span data-stu-id="105bd-116">revoked</span></span>|<span data-ttu-id="105bd-117">1/3</span><span class="sxs-lookup"><span data-stu-id="105bd-117">3</span></span>|<span data-ttu-id="105bd-118">デバイスがブロックされているか、ワイプされているか、破棄されています。</span><span class="sxs-lookup"><span data-stu-id="105bd-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="105bd-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="105bd-119">keyConflict</span></span>|<span data-ttu-id="105bd-120">2/4</span><span class="sxs-lookup"><span data-stu-id="105bd-120">4</span></span>|<span data-ttu-id="105bd-121">デバイスにキーの競合があります。</span><span class="sxs-lookup"><span data-stu-id="105bd-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="105bd-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="105bd-122">approvalPending</span></span>|<span data-ttu-id="105bd-123">5</span><span class="sxs-lookup"><span data-stu-id="105bd-123">5</span></span>|<span data-ttu-id="105bd-124">デバイスの承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="105bd-124">The device is pending approval.</span></span>|
|<span data-ttu-id="105bd-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="105bd-125">certificateReset</span></span>|<span data-ttu-id="105bd-126">シックス</span><span class="sxs-lookup"><span data-stu-id="105bd-126">6</span></span>|<span data-ttu-id="105bd-127">デバイス証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="105bd-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="105bd-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="105bd-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="105bd-129">7</span><span class="sxs-lookup"><span data-stu-id="105bd-129">7</span></span>|<span data-ttu-id="105bd-130">デバイスは登録されておらず、登録が保留されていません。</span><span class="sxs-lookup"><span data-stu-id="105bd-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="105bd-131">不明</span><span class="sxs-lookup"><span data-stu-id="105bd-131">unknown</span></span>|<span data-ttu-id="105bd-132">8 </span><span class="sxs-lookup"><span data-stu-id="105bd-132">8</span></span>|<span data-ttu-id="105bd-133">デバイス登録の状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="105bd-133">The device registration status is unknown.</span></span>|



