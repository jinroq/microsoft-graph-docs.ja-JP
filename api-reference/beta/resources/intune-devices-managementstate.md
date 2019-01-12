---
title: managementState 列挙型
description: Microsoft Intune でのデバイスの状態を管理します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d9d083c56df366b9f896432328d51c295f62190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961947"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="3f182-103">managementState 列挙型</span><span class="sxs-lookup"><span data-stu-id="3f182-103">managementState enum type</span></span>

> <span data-ttu-id="3f182-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f182-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f182-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f182-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f182-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3f182-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f182-107">Microsoft Intune でのデバイスの状態を管理します。</span><span class="sxs-lookup"><span data-stu-id="3f182-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="3f182-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3f182-108">Members</span></span>
|<span data-ttu-id="3f182-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3f182-109">Member</span></span>|<span data-ttu-id="3f182-110">値</span><span class="sxs-lookup"><span data-stu-id="3f182-110">Value</span></span>|<span data-ttu-id="3f182-111">説明</span><span class="sxs-lookup"><span data-stu-id="3f182-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f182-112">管理</span><span class="sxs-lookup"><span data-stu-id="3f182-112">managed</span></span>|<span data-ttu-id="3f182-113">0</span><span class="sxs-lookup"><span data-stu-id="3f182-113">0</span></span>|<span data-ttu-id="3f182-114">管理対象デバイスは、します。</span><span class="sxs-lookup"><span data-stu-id="3f182-114">The device is under management</span></span>|
|<span data-ttu-id="3f182-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="3f182-115">retirePending</span></span>|<span data-ttu-id="3f182-116">1</span><span class="sxs-lookup"><span data-stu-id="3f182-116">1</span></span>|<span data-ttu-id="3f182-117">削除コマンドは、デバイスと管理から unenrolling の処理中に発生しています。</span><span class="sxs-lookup"><span data-stu-id="3f182-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3f182-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="3f182-118">retireFailed</span></span>|<span data-ttu-id="3f182-119">2</span><span class="sxs-lookup"><span data-stu-id="3f182-119">2</span></span>|<span data-ttu-id="3f182-120">破棄コマンドがデバイスに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="3f182-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="3f182-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="3f182-121">wipePending</span></span>|<span data-ttu-id="3f182-122">3</span><span class="sxs-lookup"><span data-stu-id="3f182-122">3</span></span>|<span data-ttu-id="3f182-123">ワイプ コマンドは、デバイスと管理から unenrolling の処理中に発生しています。</span><span class="sxs-lookup"><span data-stu-id="3f182-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3f182-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="3f182-124">wipeFailed</span></span>|<span data-ttu-id="3f182-125">4</span><span class="sxs-lookup"><span data-stu-id="3f182-125">4</span></span>|<span data-ttu-id="3f182-126">デバイス ワイプ コマンドが失敗しました。</span><span class="sxs-lookup"><span data-stu-id="3f182-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="3f182-127">問題があります。</span><span class="sxs-lookup"><span data-stu-id="3f182-127">unhealthy</span></span>|<span data-ttu-id="3f182-128">5</span><span class="sxs-lookup"><span data-stu-id="3f182-128">5</span></span>|<span data-ttu-id="3f182-129">デバイスが正常な状態ではありません。</span><span class="sxs-lookup"><span data-stu-id="3f182-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="3f182-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="3f182-130">deletePending</span></span>|<span data-ttu-id="3f182-131">6</span><span class="sxs-lookup"><span data-stu-id="3f182-131">6</span></span>|<span data-ttu-id="3f182-132">削除コマンドは、デバイスで発生しています。</span><span class="sxs-lookup"><span data-stu-id="3f182-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="3f182-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="3f182-133">retireIssued</span></span>|<span data-ttu-id="3f182-134">7</span><span class="sxs-lookup"><span data-stu-id="3f182-134">7</span></span>|<span data-ttu-id="3f182-135">デバイスの削除コマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="3f182-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="3f182-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="3f182-136">wipeIssued</span></span>|<span data-ttu-id="3f182-137">8</span><span class="sxs-lookup"><span data-stu-id="3f182-137">8</span></span>|<span data-ttu-id="3f182-138">デバイス ワイプ コマンドがに対して発行されました</span><span class="sxs-lookup"><span data-stu-id="3f182-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="3f182-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="3f182-139">wipeCanceled</span></span>|<span data-ttu-id="3f182-140">9</span><span class="sxs-lookup"><span data-stu-id="3f182-140">9</span></span>|<span data-ttu-id="3f182-141">このデバイスのワイプ コマンドがキャンセルされました</span><span class="sxs-lookup"><span data-stu-id="3f182-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="3f182-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="3f182-142">retireCanceled</span></span>|<span data-ttu-id="3f182-143">10</span><span class="sxs-lookup"><span data-stu-id="3f182-143">10</span></span>|<span data-ttu-id="3f182-144">このデバイスの削除コマンドがキャンセルされました</span><span class="sxs-lookup"><span data-stu-id="3f182-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="3f182-145">発見</span><span class="sxs-lookup"><span data-stu-id="3f182-145">discovered</span></span>|<span data-ttu-id="3f182-146">11</span><span class="sxs-lookup"><span data-stu-id="3f182-146">11</span></span>|<span data-ttu-id="3f182-147">デバイスが検出されたが、完全に登録されています。</span><span class="sxs-lookup"><span data-stu-id="3f182-147">The device is discovered but not fully enrolled.</span></span>|





