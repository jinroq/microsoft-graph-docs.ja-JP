---
title: deviceComplianceActionType 列挙型
description: スケジュールされたアクションの種類列挙
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05f9df39c563a47fa571a4badcf789ea4ddb08b1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979530"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="e3a7e-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3a7e-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="e3a7e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3a7e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3a7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3a7e-106">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="e3a7e-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="e3a7e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3a7e-107">Members</span></span>
|<span data-ttu-id="e3a7e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3a7e-108">Member</span></span>|<span data-ttu-id="e3a7e-109">値</span><span class="sxs-lookup"><span data-stu-id="e3a7e-109">Value</span></span>|<span data-ttu-id="e3a7e-110">説明</span><span class="sxs-lookup"><span data-stu-id="e3a7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a7e-111">noAction</span><span class="sxs-lookup"><span data-stu-id="e3a7e-111">noAction</span></span>|<span data-ttu-id="e3a7e-112">.0</span><span class="sxs-lookup"><span data-stu-id="e3a7e-112">0</span></span>|<span data-ttu-id="e3a7e-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="e3a7e-113">No Action</span></span>|
|<span data-ttu-id="e3a7e-114">お知らせ</span><span class="sxs-lookup"><span data-stu-id="e3a7e-114">notification</span></span>|<span data-ttu-id="e3a7e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e3a7e-115">1</span></span>|<span data-ttu-id="e3a7e-116">通知の送信</span><span class="sxs-lookup"><span data-stu-id="e3a7e-116">Send Notification</span></span>|
|<span data-ttu-id="e3a7e-117">拒否</span><span class="sxs-lookup"><span data-stu-id="e3a7e-117">block</span></span>|<span data-ttu-id="e3a7e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e3a7e-118">2</span></span>|<span data-ttu-id="e3a7e-119">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="e3a7e-119">Block the device in AAD</span></span>|
|<span data-ttu-id="e3a7e-120">削除</span><span class="sxs-lookup"><span data-stu-id="e3a7e-120">retire</span></span>|<span data-ttu-id="e3a7e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e3a7e-121">3</span></span>|<span data-ttu-id="e3a7e-122">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="e3a7e-122">Retire the device</span></span>|
|<span data-ttu-id="e3a7e-123">ふき</span><span class="sxs-lookup"><span data-stu-id="e3a7e-123">wipe</span></span>|<span data-ttu-id="e3a7e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e3a7e-124">4</span></span>|<span data-ttu-id="e3a7e-125">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="e3a7e-125">Wipe the device</span></span>|
|<span data-ttu-id="e3a7e-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="e3a7e-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="e3a7e-127">5</span><span class="sxs-lookup"><span data-stu-id="e3a7e-127">5</span></span>|<span data-ttu-id="e3a7e-128">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="e3a7e-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="e3a7e-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="e3a7e-129">pushNotification</span></span>|<span data-ttu-id="e3a7e-130">9 </span><span class="sxs-lookup"><span data-stu-id="e3a7e-130">9</span></span>|<span data-ttu-id="e3a7e-131">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="e3a7e-131">Send push notification to device</span></span>|
|<span data-ttu-id="e3a7e-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="e3a7e-132">remoteLock</span></span>|<span data-ttu-id="e3a7e-133">10 </span><span class="sxs-lookup"><span data-stu-id="e3a7e-133">10</span></span>|<span data-ttu-id="e3a7e-134">デバイスをリモートでロックする</span><span class="sxs-lookup"><span data-stu-id="e3a7e-134">Remotely lock the device</span></span>|





