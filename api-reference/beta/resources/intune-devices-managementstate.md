---
title: managementstate 列挙型
description: Microsoft Intune でのデバイスの管理状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a53b07f89ee551d3e559a42bbe23c5fba808f20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174145"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="0c802-103">managementstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="0c802-103">managementState enum type</span></span>

> <span data-ttu-id="0c802-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c802-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c802-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c802-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c802-106">Microsoft Intune でのデバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="0c802-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="0c802-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c802-107">Members</span></span>
|<span data-ttu-id="0c802-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c802-108">Member</span></span>|<span data-ttu-id="0c802-109">値</span><span class="sxs-lookup"><span data-stu-id="0c802-109">Value</span></span>|<span data-ttu-id="0c802-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c802-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c802-111">対象</span><span class="sxs-lookup"><span data-stu-id="0c802-111">managed</span></span>|<span data-ttu-id="0c802-112">.0</span><span class="sxs-lookup"><span data-stu-id="0c802-112">0</span></span>|<span data-ttu-id="0c802-113">デバイスが管理下にある</span><span class="sxs-lookup"><span data-stu-id="0c802-113">The device is under management</span></span>|
|<span data-ttu-id="0c802-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="0c802-114">retirePending</span></span>|<span data-ttu-id="0c802-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0c802-115">1</span></span>|<span data-ttu-id="0c802-116">廃棄コマンドは、デバイス上および管理からの登録取り消しプロセス中に発生します。</span><span class="sxs-lookup"><span data-stu-id="0c802-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0c802-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="0c802-117">retireFailed</span></span>|<span data-ttu-id="0c802-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0c802-118">2</span></span>|<span data-ttu-id="0c802-119">デバイスでのリタイアコマンドが失敗しました</span><span class="sxs-lookup"><span data-stu-id="0c802-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="0c802-120">wipepending</span><span class="sxs-lookup"><span data-stu-id="0c802-120">wipePending</span></span>|<span data-ttu-id="0c802-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0c802-121">3</span></span>|<span data-ttu-id="0c802-122">ワイプコマンドがデバイス上で発生していて、管理からの登録取り消しプロセスである</span><span class="sxs-lookup"><span data-stu-id="0c802-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0c802-123">wipefailed</span><span class="sxs-lookup"><span data-stu-id="0c802-123">wipeFailed</span></span>|<span data-ttu-id="0c802-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0c802-124">4</span></span>|<span data-ttu-id="0c802-125">デバイスでワイプコマンドが失敗しました</span><span class="sxs-lookup"><span data-stu-id="0c802-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="0c802-126">正常</span><span class="sxs-lookup"><span data-stu-id="0c802-126">unhealthy</span></span>|<span data-ttu-id="0c802-127">5</span><span class="sxs-lookup"><span data-stu-id="0c802-127">5</span></span>|<span data-ttu-id="0c802-128">デバイスに問題があります。</span><span class="sxs-lookup"><span data-stu-id="0c802-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="0c802-129">deletepending</span><span class="sxs-lookup"><span data-stu-id="0c802-129">deletePending</span></span>|<span data-ttu-id="0c802-130">シックス</span><span class="sxs-lookup"><span data-stu-id="0c802-130">6</span></span>|<span data-ttu-id="0c802-131">デバイスで削除コマンドが発生しています</span><span class="sxs-lookup"><span data-stu-id="0c802-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="0c802-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="0c802-132">retireIssued</span></span>|<span data-ttu-id="0c802-133">7</span><span class="sxs-lookup"><span data-stu-id="0c802-133">7</span></span>|<span data-ttu-id="0c802-134">デバイスに対して、廃棄コマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="0c802-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="0c802-135">wipeissued 済み</span><span class="sxs-lookup"><span data-stu-id="0c802-135">wipeIssued</span></span>|<span data-ttu-id="0c802-136">~</span><span class="sxs-lookup"><span data-stu-id="0c802-136">8</span></span>|<span data-ttu-id="0c802-137">デバイスに対してワイプコマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="0c802-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="0c802-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="0c802-138">wipeCanceled</span></span>|<span data-ttu-id="0c802-139">i-9</span><span class="sxs-lookup"><span data-stu-id="0c802-139">9</span></span>|<span data-ttu-id="0c802-140">このデバイスのワイプコマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="0c802-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="0c802-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="0c802-141">retireCanceled</span></span>|<span data-ttu-id="0c802-142">個</span><span class="sxs-lookup"><span data-stu-id="0c802-142">10</span></span>|<span data-ttu-id="0c802-143">このデバイスの廃棄コマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="0c802-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="0c802-144">た</span><span class="sxs-lookup"><span data-stu-id="0c802-144">discovered</span></span>|<span data-ttu-id="0c802-145">#</span><span class="sxs-lookup"><span data-stu-id="0c802-145">11</span></span>|<span data-ttu-id="0c802-146">デバイスが検出されますが、完全に登録されていません。</span><span class="sxs-lookup"><span data-stu-id="0c802-146">The device is discovered but not fully enrolled.</span></span>|




