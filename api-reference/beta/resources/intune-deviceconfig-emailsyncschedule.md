---
title: emailSyncSchedule 列挙型
description: 電子メールの同期スケジュールの可能な値です。
ms.openlocfilehash: 48c5d433815d5f27d018d97ac479641146754669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066634"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="04356-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="04356-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="04356-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04356-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04356-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04356-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04356-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04356-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04356-107">電子メールの同期スケジュールの可能な値です。</span><span class="sxs-lookup"><span data-stu-id="04356-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="04356-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="04356-108">Members</span></span>
|<span data-ttu-id="04356-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="04356-109">Member</span></span>|<span data-ttu-id="04356-110">値</span><span class="sxs-lookup"><span data-stu-id="04356-110">Value</span></span>|<span data-ttu-id="04356-111">説明</span><span class="sxs-lookup"><span data-stu-id="04356-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04356-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="04356-112">userDefined</span></span>|<span data-ttu-id="04356-113">0</span><span class="sxs-lookup"><span data-stu-id="04356-113">0</span></span>|<span data-ttu-id="04356-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="04356-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="04356-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="04356-115">asMessagesArrive</span></span>|<span data-ttu-id="04356-116">1</span><span class="sxs-lookup"><span data-stu-id="04356-116">1</span></span>|<span data-ttu-id="04356-117">メッセージの受信時に同期します。</span><span class="sxs-lookup"><span data-stu-id="04356-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="04356-118">手動</span><span class="sxs-lookup"><span data-stu-id="04356-118">manual</span></span>|<span data-ttu-id="04356-119">2</span><span class="sxs-lookup"><span data-stu-id="04356-119">2</span></span>|<span data-ttu-id="04356-120">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="04356-120">Sync manually.</span></span>|
|<span data-ttu-id="04356-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="04356-121">fifteenMinutes</span></span>|<span data-ttu-id="04356-122">3</span><span class="sxs-lookup"><span data-stu-id="04356-122">3</span></span>|<span data-ttu-id="04356-123">15 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="04356-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="04356-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="04356-124">thirtyMinutes</span></span>|<span data-ttu-id="04356-125">4</span><span class="sxs-lookup"><span data-stu-id="04356-125">4</span></span>|<span data-ttu-id="04356-126">30 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="04356-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="04356-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="04356-127">sixtyMinutes</span></span>|<span data-ttu-id="04356-128">5</span><span class="sxs-lookup"><span data-stu-id="04356-128">5</span></span>|<span data-ttu-id="04356-129">同期は 60 分ごと。</span><span class="sxs-lookup"><span data-stu-id="04356-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="04356-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="04356-130">basedOnMyUsage</span></span>|<span data-ttu-id="04356-131">6</span><span class="sxs-lookup"><span data-stu-id="04356-131">6</span></span>|<span data-ttu-id="04356-132">私の使用率に基づく同期。</span><span class="sxs-lookup"><span data-stu-id="04356-132">Sync based on my usage.</span></span>|





