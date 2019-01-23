---
title: managementState 列挙型
description: Microsoft Intune でのデバイスの状態を管理します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420018"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="a81a0-103">managementState 列挙型</span><span class="sxs-lookup"><span data-stu-id="a81a0-103">managementState enum type</span></span>

> <span data-ttu-id="a81a0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a81a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a81a0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a81a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a81a0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a81a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a81a0-107">Microsoft Intune でのデバイスの状態を管理します。</span><span class="sxs-lookup"><span data-stu-id="a81a0-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="a81a0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a81a0-108">Members</span></span>
|<span data-ttu-id="a81a0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a81a0-109">Member</span></span>|<span data-ttu-id="a81a0-110">値</span><span class="sxs-lookup"><span data-stu-id="a81a0-110">Value</span></span>|<span data-ttu-id="a81a0-111">説明</span><span class="sxs-lookup"><span data-stu-id="a81a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a81a0-112">管理</span><span class="sxs-lookup"><span data-stu-id="a81a0-112">managed</span></span>|<span data-ttu-id="a81a0-113">0</span><span class="sxs-lookup"><span data-stu-id="a81a0-113">0</span></span>|<span data-ttu-id="a81a0-114">管理対象デバイスは、します。</span><span class="sxs-lookup"><span data-stu-id="a81a0-114">The device is under management</span></span>|
|<span data-ttu-id="a81a0-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="a81a0-115">retirePending</span></span>|<span data-ttu-id="a81a0-116">1</span><span class="sxs-lookup"><span data-stu-id="a81a0-116">1</span></span>|<span data-ttu-id="a81a0-117">削除コマンドは、デバイスと管理から unenrolling の処理中に発生しています。</span><span class="sxs-lookup"><span data-stu-id="a81a0-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="a81a0-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="a81a0-118">retireFailed</span></span>|<span data-ttu-id="a81a0-119">2</span><span class="sxs-lookup"><span data-stu-id="a81a0-119">2</span></span>|<span data-ttu-id="a81a0-120">破棄コマンドがデバイスに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="a81a0-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="a81a0-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="a81a0-121">wipePending</span></span>|<span data-ttu-id="a81a0-122">3</span><span class="sxs-lookup"><span data-stu-id="a81a0-122">3</span></span>|<span data-ttu-id="a81a0-123">ワイプ コマンドは、デバイスと管理から unenrolling の処理中に発生しています。</span><span class="sxs-lookup"><span data-stu-id="a81a0-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="a81a0-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="a81a0-124">wipeFailed</span></span>|<span data-ttu-id="a81a0-125">4</span><span class="sxs-lookup"><span data-stu-id="a81a0-125">4</span></span>|<span data-ttu-id="a81a0-126">デバイス ワイプ コマンドが失敗しました。</span><span class="sxs-lookup"><span data-stu-id="a81a0-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="a81a0-127">問題があります。</span><span class="sxs-lookup"><span data-stu-id="a81a0-127">unhealthy</span></span>|<span data-ttu-id="a81a0-128">5</span><span class="sxs-lookup"><span data-stu-id="a81a0-128">5</span></span>|<span data-ttu-id="a81a0-129">デバイスが正常な状態ではありません。</span><span class="sxs-lookup"><span data-stu-id="a81a0-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="a81a0-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="a81a0-130">deletePending</span></span>|<span data-ttu-id="a81a0-131">6</span><span class="sxs-lookup"><span data-stu-id="a81a0-131">6</span></span>|<span data-ttu-id="a81a0-132">削除コマンドは、デバイスで発生しています。</span><span class="sxs-lookup"><span data-stu-id="a81a0-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="a81a0-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="a81a0-133">retireIssued</span></span>|<span data-ttu-id="a81a0-134">7</span><span class="sxs-lookup"><span data-stu-id="a81a0-134">7</span></span>|<span data-ttu-id="a81a0-135">デバイスの削除コマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="a81a0-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="a81a0-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="a81a0-136">wipeIssued</span></span>|<span data-ttu-id="a81a0-137">8</span><span class="sxs-lookup"><span data-stu-id="a81a0-137">8</span></span>|<span data-ttu-id="a81a0-138">デバイス ワイプ コマンドがに対して発行されました</span><span class="sxs-lookup"><span data-stu-id="a81a0-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="a81a0-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="a81a0-139">wipeCanceled</span></span>|<span data-ttu-id="a81a0-140">9</span><span class="sxs-lookup"><span data-stu-id="a81a0-140">9</span></span>|<span data-ttu-id="a81a0-141">このデバイスのワイプ コマンドがキャンセルされました</span><span class="sxs-lookup"><span data-stu-id="a81a0-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="a81a0-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="a81a0-142">retireCanceled</span></span>|<span data-ttu-id="a81a0-143">10</span><span class="sxs-lookup"><span data-stu-id="a81a0-143">10</span></span>|<span data-ttu-id="a81a0-144">このデバイスの削除コマンドがキャンセルされました</span><span class="sxs-lookup"><span data-stu-id="a81a0-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="a81a0-145">発見</span><span class="sxs-lookup"><span data-stu-id="a81a0-145">discovered</span></span>|<span data-ttu-id="a81a0-146">11</span><span class="sxs-lookup"><span data-stu-id="a81a0-146">11</span></span>|<span data-ttu-id="a81a0-147">デバイスが検出されたが、完全に登録されています。</span><span class="sxs-lookup"><span data-stu-id="a81a0-147">The device is discovered but not fully enrolled.</span></span>|




