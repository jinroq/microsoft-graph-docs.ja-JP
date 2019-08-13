---
title: deviceComplianceActionType 列挙型
description: スケジュールされたアクションの種類列挙
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab26d2b6cda774f3d2cf3284f92d1901cc4bdf82
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333213"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="3fd5a-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3fd5a-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="3fd5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fd5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fd5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fd5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd5a-106">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="3fd5a-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="3fd5a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fd5a-107">Members</span></span>
|<span data-ttu-id="3fd5a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fd5a-108">Member</span></span>|<span data-ttu-id="3fd5a-109">値</span><span class="sxs-lookup"><span data-stu-id="3fd5a-109">Value</span></span>|<span data-ttu-id="3fd5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="3fd5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd5a-111">noAction</span><span class="sxs-lookup"><span data-stu-id="3fd5a-111">noAction</span></span>|<span data-ttu-id="3fd5a-112">.0</span><span class="sxs-lookup"><span data-stu-id="3fd5a-112">0</span></span>|<span data-ttu-id="3fd5a-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="3fd5a-113">No Action</span></span>|
|<span data-ttu-id="3fd5a-114">お知らせ</span><span class="sxs-lookup"><span data-stu-id="3fd5a-114">notification</span></span>|<span data-ttu-id="3fd5a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3fd5a-115">1</span></span>|<span data-ttu-id="3fd5a-116">通知の送信</span><span class="sxs-lookup"><span data-stu-id="3fd5a-116">Send Notification</span></span>|
|<span data-ttu-id="3fd5a-117">拒否</span><span class="sxs-lookup"><span data-stu-id="3fd5a-117">block</span></span>|<span data-ttu-id="3fd5a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3fd5a-118">2</span></span>|<span data-ttu-id="3fd5a-119">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="3fd5a-119">Block the device in AAD</span></span>|
|<span data-ttu-id="3fd5a-120">削除</span><span class="sxs-lookup"><span data-stu-id="3fd5a-120">retire</span></span>|<span data-ttu-id="3fd5a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3fd5a-121">3</span></span>|<span data-ttu-id="3fd5a-122">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="3fd5a-122">Retire the device</span></span>|
|<span data-ttu-id="3fd5a-123">ふき</span><span class="sxs-lookup"><span data-stu-id="3fd5a-123">wipe</span></span>|<span data-ttu-id="3fd5a-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3fd5a-124">4</span></span>|<span data-ttu-id="3fd5a-125">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="3fd5a-125">Wipe the device</span></span>|
|<span data-ttu-id="3fd5a-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="3fd5a-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="3fd5a-127">5</span><span class="sxs-lookup"><span data-stu-id="3fd5a-127">5</span></span>|<span data-ttu-id="3fd5a-128">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="3fd5a-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="3fd5a-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="3fd5a-129">pushNotification</span></span>|<span data-ttu-id="3fd5a-130">9 </span><span class="sxs-lookup"><span data-stu-id="3fd5a-130">9</span></span>|<span data-ttu-id="3fd5a-131">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="3fd5a-131">Send push notification to device</span></span>|
|<span data-ttu-id="3fd5a-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="3fd5a-132">remoteLock</span></span>|<span data-ttu-id="3fd5a-133">10 </span><span class="sxs-lookup"><span data-stu-id="3fd5a-133">10</span></span>|<span data-ttu-id="3fd5a-134">デバイスをリモートでロックする</span><span class="sxs-lookup"><span data-stu-id="3fd5a-134">Remotely lock the device</span></span>|



