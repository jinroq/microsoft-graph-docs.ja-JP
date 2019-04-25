---
title: managementstate 列挙型
description: Microsoft Intune でのデバイスの管理状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521293"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="9ff74-103">managementstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="9ff74-103">managementState enum type</span></span>

> <span data-ttu-id="9ff74-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ff74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff74-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ff74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff74-106">Microsoft Intune でのデバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="9ff74-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="9ff74-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ff74-107">Members</span></span>
|<span data-ttu-id="9ff74-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ff74-108">Member</span></span>|<span data-ttu-id="9ff74-109">値</span><span class="sxs-lookup"><span data-stu-id="9ff74-109">Value</span></span>|<span data-ttu-id="9ff74-110">説明</span><span class="sxs-lookup"><span data-stu-id="9ff74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff74-111">対象</span><span class="sxs-lookup"><span data-stu-id="9ff74-111">managed</span></span>|<span data-ttu-id="9ff74-112">.0</span><span class="sxs-lookup"><span data-stu-id="9ff74-112">0</span></span>|<span data-ttu-id="9ff74-113">デバイスが管理下にある</span><span class="sxs-lookup"><span data-stu-id="9ff74-113">The device is under management</span></span>|
|<span data-ttu-id="9ff74-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="9ff74-114">retirePending</span></span>|<span data-ttu-id="9ff74-115">1 </span><span class="sxs-lookup"><span data-stu-id="9ff74-115">1</span></span>|<span data-ttu-id="9ff74-116">廃棄コマンドは、デバイス上および管理からの登録取り消しプロセス中に発生します。</span><span class="sxs-lookup"><span data-stu-id="9ff74-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="9ff74-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="9ff74-117">retireFailed</span></span>|<span data-ttu-id="9ff74-118">2 </span><span class="sxs-lookup"><span data-stu-id="9ff74-118">2</span></span>|<span data-ttu-id="9ff74-119">デバイスでのリタイアコマンドが失敗しました</span><span class="sxs-lookup"><span data-stu-id="9ff74-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="9ff74-120">wipepending</span><span class="sxs-lookup"><span data-stu-id="9ff74-120">wipePending</span></span>|<span data-ttu-id="9ff74-121">3 </span><span class="sxs-lookup"><span data-stu-id="9ff74-121">3</span></span>|<span data-ttu-id="9ff74-122">ワイプコマンドがデバイス上で発生していて、管理からの登録取り消しプロセスである</span><span class="sxs-lookup"><span data-stu-id="9ff74-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="9ff74-123">wipefailed</span><span class="sxs-lookup"><span data-stu-id="9ff74-123">wipeFailed</span></span>|<span data-ttu-id="9ff74-124">4 </span><span class="sxs-lookup"><span data-stu-id="9ff74-124">4</span></span>|<span data-ttu-id="9ff74-125">デバイスでワイプコマンドが失敗しました</span><span class="sxs-lookup"><span data-stu-id="9ff74-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="9ff74-126">正常</span><span class="sxs-lookup"><span data-stu-id="9ff74-126">unhealthy</span></span>|<span data-ttu-id="9ff74-127">5 </span><span class="sxs-lookup"><span data-stu-id="9ff74-127">5</span></span>|<span data-ttu-id="9ff74-128">デバイスに問題があります。</span><span class="sxs-lookup"><span data-stu-id="9ff74-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="9ff74-129">deletepending</span><span class="sxs-lookup"><span data-stu-id="9ff74-129">deletePending</span></span>|<span data-ttu-id="9ff74-130">6 </span><span class="sxs-lookup"><span data-stu-id="9ff74-130">6</span></span>|<span data-ttu-id="9ff74-131">デバイスで削除コマンドが発生しています</span><span class="sxs-lookup"><span data-stu-id="9ff74-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="9ff74-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="9ff74-132">retireIssued</span></span>|<span data-ttu-id="9ff74-133">7 </span><span class="sxs-lookup"><span data-stu-id="9ff74-133">7</span></span>|<span data-ttu-id="9ff74-134">デバイスに対して、廃棄コマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="9ff74-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="9ff74-135">wipeissued 済み</span><span class="sxs-lookup"><span data-stu-id="9ff74-135">wipeIssued</span></span>|<span data-ttu-id="9ff74-136">8 </span><span class="sxs-lookup"><span data-stu-id="9ff74-136">8</span></span>|<span data-ttu-id="9ff74-137">デバイスに対してワイプコマンドが発行されました</span><span class="sxs-lookup"><span data-stu-id="9ff74-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="9ff74-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="9ff74-138">wipeCanceled</span></span>|<span data-ttu-id="9ff74-139">9 </span><span class="sxs-lookup"><span data-stu-id="9ff74-139">9</span></span>|<span data-ttu-id="9ff74-140">このデバイスのワイプコマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="9ff74-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="9ff74-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="9ff74-141">retireCanceled</span></span>|<span data-ttu-id="9ff74-142">10  </span><span class="sxs-lookup"><span data-stu-id="9ff74-142">10</span></span>|<span data-ttu-id="9ff74-143">このデバイスの廃棄コマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="9ff74-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="9ff74-144">た</span><span class="sxs-lookup"><span data-stu-id="9ff74-144">discovered</span></span>|<span data-ttu-id="9ff74-145">11 </span><span class="sxs-lookup"><span data-stu-id="9ff74-145">11</span></span>|<span data-ttu-id="9ff74-146">デバイスが検出されますが、完全に登録されていません。</span><span class="sxs-lookup"><span data-stu-id="9ff74-146">The device is discovered but not fully enrolled.</span></span>|





