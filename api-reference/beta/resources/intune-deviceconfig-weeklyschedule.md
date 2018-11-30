---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに指定できる値です。
ms.openlocfilehash: 67534cbe21782b64e995d9bf48d9abbde778f142
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069654"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="db012-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="db012-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="db012-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db012-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db012-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db012-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db012-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db012-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db012-107">週単位のスケジュールに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="db012-107">Possible values for a weekly schedule.</span></span>
## <a name="members"></a><span data-ttu-id="db012-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="db012-108">Members</span></span>
|<span data-ttu-id="db012-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="db012-109">Member</span></span>|<span data-ttu-id="db012-110">値</span><span class="sxs-lookup"><span data-stu-id="db012-110">Value</span></span>|<span data-ttu-id="db012-111">説明</span><span class="sxs-lookup"><span data-stu-id="db012-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db012-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="db012-112">userDefined</span></span>|<span data-ttu-id="db012-113">0</span><span class="sxs-lookup"><span data-stu-id="db012-113">0</span></span>|<span data-ttu-id="db012-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="db012-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="db012-115">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="db012-115">everyday</span></span>|<span data-ttu-id="db012-116">1</span><span class="sxs-lookup"><span data-stu-id="db012-116">1</span></span>|<span data-ttu-id="db012-117">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="db012-117">Everyday.</span></span>|
|<span data-ttu-id="db012-118">日曜日</span><span class="sxs-lookup"><span data-stu-id="db012-118">sunday</span></span>|<span data-ttu-id="db012-119">2</span><span class="sxs-lookup"><span data-stu-id="db012-119">2</span></span>|<span data-ttu-id="db012-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="db012-120">Sunday.</span></span>|
|<span data-ttu-id="db012-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="db012-121">monday</span></span>|<span data-ttu-id="db012-122">3</span><span class="sxs-lookup"><span data-stu-id="db012-122">3</span></span>|<span data-ttu-id="db012-123">月曜日</span><span class="sxs-lookup"><span data-stu-id="db012-123">Monday.</span></span>|
|<span data-ttu-id="db012-124">火曜日</span><span class="sxs-lookup"><span data-stu-id="db012-124">tuesday</span></span>|<span data-ttu-id="db012-125">4</span><span class="sxs-lookup"><span data-stu-id="db012-125">4</span></span>|<span data-ttu-id="db012-126">火曜日</span><span class="sxs-lookup"><span data-stu-id="db012-126">Tuesday.</span></span>|
|<span data-ttu-id="db012-127">(水)</span><span class="sxs-lookup"><span data-stu-id="db012-127">wednesday</span></span>|<span data-ttu-id="db012-128">5</span><span class="sxs-lookup"><span data-stu-id="db012-128">5</span></span>|<span data-ttu-id="db012-129">水曜日</span><span class="sxs-lookup"><span data-stu-id="db012-129">Wednesday.</span></span>|
|<span data-ttu-id="db012-130">(木)</span><span class="sxs-lookup"><span data-stu-id="db012-130">thursday</span></span>|<span data-ttu-id="db012-131">6</span><span class="sxs-lookup"><span data-stu-id="db012-131">6</span></span>|<span data-ttu-id="db012-132">木曜日</span><span class="sxs-lookup"><span data-stu-id="db012-132">Thursday.</span></span>|
|<span data-ttu-id="db012-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="db012-133">friday</span></span>|<span data-ttu-id="db012-134">7</span><span class="sxs-lookup"><span data-stu-id="db012-134">7</span></span>|<span data-ttu-id="db012-135">金曜日</span><span class="sxs-lookup"><span data-stu-id="db012-135">Friday.</span></span>|
|<span data-ttu-id="db012-136">土曜日</span><span class="sxs-lookup"><span data-stu-id="db012-136">saturday</span></span>|<span data-ttu-id="db012-137">8</span><span class="sxs-lookup"><span data-stu-id="db012-137">8</span></span>|<span data-ttu-id="db012-138">土曜日</span><span class="sxs-lookup"><span data-stu-id="db012-138">Saturday.</span></span>|





