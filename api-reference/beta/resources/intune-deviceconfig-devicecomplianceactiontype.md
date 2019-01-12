---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973210"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="4e9cd-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4e9cd-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="4e9cd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e9cd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e9cd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e9cd-107">列挙型の操作をスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="4e9cd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4e9cd-108">Members</span></span>
|<span data-ttu-id="4e9cd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4e9cd-109">Member</span></span>|<span data-ttu-id="4e9cd-110">値</span><span class="sxs-lookup"><span data-stu-id="4e9cd-110">Value</span></span>|<span data-ttu-id="4e9cd-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e9cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9cd-112">noAction</span><span class="sxs-lookup"><span data-stu-id="4e9cd-112">noAction</span></span>|<span data-ttu-id="4e9cd-113">0</span><span class="sxs-lookup"><span data-stu-id="4e9cd-113">0</span></span>|<span data-ttu-id="4e9cd-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-114">No Action</span></span>|
|<span data-ttu-id="4e9cd-115">通知</span><span class="sxs-lookup"><span data-stu-id="4e9cd-115">notification</span></span>|<span data-ttu-id="4e9cd-116">1</span><span class="sxs-lookup"><span data-stu-id="4e9cd-116">1</span></span>|<span data-ttu-id="4e9cd-117">通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-117">Send Notification</span></span>|
|<span data-ttu-id="4e9cd-118">ブロック</span><span class="sxs-lookup"><span data-stu-id="4e9cd-118">block</span></span>|<span data-ttu-id="4e9cd-119">2</span><span class="sxs-lookup"><span data-stu-id="4e9cd-119">2</span></span>|<span data-ttu-id="4e9cd-120">AAD でデバイスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-120">Block the device in AAD</span></span>|
|<span data-ttu-id="4e9cd-121">退職</span><span class="sxs-lookup"><span data-stu-id="4e9cd-121">retire</span></span>|<span data-ttu-id="4e9cd-122">3</span><span class="sxs-lookup"><span data-stu-id="4e9cd-122">3</span></span>|<span data-ttu-id="4e9cd-123">デバイスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-123">Retire the device</span></span>|
|<span data-ttu-id="4e9cd-124">ワイプ</span><span class="sxs-lookup"><span data-stu-id="4e9cd-124">wipe</span></span>|<span data-ttu-id="4e9cd-125">4</span><span class="sxs-lookup"><span data-stu-id="4e9cd-125">4</span></span>|<span data-ttu-id="4e9cd-126">デバイスをワイプします。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-126">Wipe the device</span></span>|
|<span data-ttu-id="4e9cd-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="4e9cd-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="4e9cd-128">5</span><span class="sxs-lookup"><span data-stu-id="4e9cd-128">5</span></span>|<span data-ttu-id="4e9cd-129">デバイスからリソースのアクセス ・ プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="4e9cd-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="4e9cd-130">pushNotification</span></span>|<span data-ttu-id="4e9cd-131">9</span><span class="sxs-lookup"><span data-stu-id="4e9cd-131">9</span></span>|<span data-ttu-id="4e9cd-132">デバイスにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-132">Send push notification to device</span></span>|
|<span data-ttu-id="4e9cd-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="4e9cd-133">remoteLock</span></span>|<span data-ttu-id="4e9cd-134">10</span><span class="sxs-lookup"><span data-stu-id="4e9cd-134">10</span></span>|<span data-ttu-id="4e9cd-135">リモートでデバイスをロックします。</span><span class="sxs-lookup"><span data-stu-id="4e9cd-135">Remotely lock the device</span></span>|





