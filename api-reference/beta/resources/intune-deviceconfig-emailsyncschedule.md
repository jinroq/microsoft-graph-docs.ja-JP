---
title: emailSyncSchedule 列挙型
description: 電子メールの同期スケジュールの可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838396"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="74ab9-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="74ab9-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="74ab9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74ab9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74ab9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ab9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74ab9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74ab9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74ab9-107">電子メールの同期スケジュールの可能な値です。</span><span class="sxs-lookup"><span data-stu-id="74ab9-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="74ab9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="74ab9-108">Members</span></span>
|<span data-ttu-id="74ab9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="74ab9-109">Member</span></span>|<span data-ttu-id="74ab9-110">値</span><span class="sxs-lookup"><span data-stu-id="74ab9-110">Value</span></span>|<span data-ttu-id="74ab9-111">説明</span><span class="sxs-lookup"><span data-stu-id="74ab9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ab9-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="74ab9-112">userDefined</span></span>|<span data-ttu-id="74ab9-113">0</span><span class="sxs-lookup"><span data-stu-id="74ab9-113">0</span></span>|<span data-ttu-id="74ab9-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="74ab9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="74ab9-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="74ab9-115">asMessagesArrive</span></span>|<span data-ttu-id="74ab9-116">1</span><span class="sxs-lookup"><span data-stu-id="74ab9-116">1</span></span>|<span data-ttu-id="74ab9-117">メッセージの受信時に同期します。</span><span class="sxs-lookup"><span data-stu-id="74ab9-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="74ab9-118">手動</span><span class="sxs-lookup"><span data-stu-id="74ab9-118">manual</span></span>|<span data-ttu-id="74ab9-119">2</span><span class="sxs-lookup"><span data-stu-id="74ab9-119">2</span></span>|<span data-ttu-id="74ab9-120">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="74ab9-120">Sync manually.</span></span>|
|<span data-ttu-id="74ab9-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="74ab9-121">fifteenMinutes</span></span>|<span data-ttu-id="74ab9-122">3</span><span class="sxs-lookup"><span data-stu-id="74ab9-122">3</span></span>|<span data-ttu-id="74ab9-123">15 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="74ab9-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="74ab9-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="74ab9-124">thirtyMinutes</span></span>|<span data-ttu-id="74ab9-125">4</span><span class="sxs-lookup"><span data-stu-id="74ab9-125">4</span></span>|<span data-ttu-id="74ab9-126">30 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="74ab9-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="74ab9-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="74ab9-127">sixtyMinutes</span></span>|<span data-ttu-id="74ab9-128">5</span><span class="sxs-lookup"><span data-stu-id="74ab9-128">5</span></span>|<span data-ttu-id="74ab9-129">同期は 60 分ごと。</span><span class="sxs-lookup"><span data-stu-id="74ab9-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="74ab9-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="74ab9-130">basedOnMyUsage</span></span>|<span data-ttu-id="74ab9-131">6</span><span class="sxs-lookup"><span data-stu-id="74ab9-131">6</span></span>|<span data-ttu-id="74ab9-132">私の使用率に基づく同期。</span><span class="sxs-lookup"><span data-stu-id="74ab9-132">Sync based on my usage.</span></span>|





