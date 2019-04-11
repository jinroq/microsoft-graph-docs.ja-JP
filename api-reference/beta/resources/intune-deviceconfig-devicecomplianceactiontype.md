---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772945"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="d6f18-103">devicecomplianceactiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6f18-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="d6f18-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6f18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6f18-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6f18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6f18-106">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="d6f18-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="d6f18-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6f18-107">Members</span></span>
|<span data-ttu-id="d6f18-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6f18-108">Member</span></span>|<span data-ttu-id="d6f18-109">値</span><span class="sxs-lookup"><span data-stu-id="d6f18-109">Value</span></span>|<span data-ttu-id="d6f18-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6f18-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6f18-111">noAction</span><span class="sxs-lookup"><span data-stu-id="d6f18-111">noAction</span></span>|<span data-ttu-id="d6f18-112">.0</span><span class="sxs-lookup"><span data-stu-id="d6f18-112">0</span></span>|<span data-ttu-id="d6f18-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="d6f18-113">No Action</span></span>|
|<span data-ttu-id="d6f18-114">お知らせ</span><span class="sxs-lookup"><span data-stu-id="d6f18-114">notification</span></span>|<span data-ttu-id="d6f18-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d6f18-115">1</span></span>|<span data-ttu-id="d6f18-116">通知の送信</span><span class="sxs-lookup"><span data-stu-id="d6f18-116">Send Notification</span></span>|
|<span data-ttu-id="d6f18-117">拒否</span><span class="sxs-lookup"><span data-stu-id="d6f18-117">block</span></span>|<span data-ttu-id="d6f18-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d6f18-118">2</span></span>|<span data-ttu-id="d6f18-119">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="d6f18-119">Block the device in AAD</span></span>|
|<span data-ttu-id="d6f18-120">削除</span><span class="sxs-lookup"><span data-stu-id="d6f18-120">retire</span></span>|<span data-ttu-id="d6f18-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d6f18-121">3</span></span>|<span data-ttu-id="d6f18-122">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="d6f18-122">Retire the device</span></span>|
|<span data-ttu-id="d6f18-123">ふき</span><span class="sxs-lookup"><span data-stu-id="d6f18-123">wipe</span></span>|<span data-ttu-id="d6f18-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d6f18-124">4</span></span>|<span data-ttu-id="d6f18-125">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="d6f18-125">Wipe the device</span></span>|
|<span data-ttu-id="d6f18-126">removeresourceaccessprofiles</span><span class="sxs-lookup"><span data-stu-id="d6f18-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="d6f18-127">5</span><span class="sxs-lookup"><span data-stu-id="d6f18-127">5</span></span>|<span data-ttu-id="d6f18-128">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="d6f18-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="d6f18-129">pushnotification</span><span class="sxs-lookup"><span data-stu-id="d6f18-129">pushNotification</span></span>|<span data-ttu-id="d6f18-130">i-9</span><span class="sxs-lookup"><span data-stu-id="d6f18-130">9</span></span>|<span data-ttu-id="d6f18-131">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="d6f18-131">Send push notification to device</span></span>|
|<span data-ttu-id="d6f18-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="d6f18-132">remoteLock</span></span>|<span data-ttu-id="d6f18-133">個</span><span class="sxs-lookup"><span data-stu-id="d6f18-133">10</span></span>|<span data-ttu-id="d6f18-134">デバイスをリモートでロックする</span><span class="sxs-lookup"><span data-stu-id="d6f18-134">Remotely lock the device</span></span>|





