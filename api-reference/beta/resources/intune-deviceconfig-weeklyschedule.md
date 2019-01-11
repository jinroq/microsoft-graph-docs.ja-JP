---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b01c71399016fcee2a5320c04dd20073f7d8673a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816248"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="a35ea-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="a35ea-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="a35ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a35ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a35ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a35ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a35ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a35ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a35ea-107">週単位のスケジュールに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="a35ea-107">Possible values for a weekly schedule.</span></span>
## <a name="members"></a><span data-ttu-id="a35ea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a35ea-108">Members</span></span>
|<span data-ttu-id="a35ea-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a35ea-109">Member</span></span>|<span data-ttu-id="a35ea-110">値</span><span class="sxs-lookup"><span data-stu-id="a35ea-110">Value</span></span>|<span data-ttu-id="a35ea-111">説明</span><span class="sxs-lookup"><span data-stu-id="a35ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35ea-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="a35ea-112">userDefined</span></span>|<span data-ttu-id="a35ea-113">0</span><span class="sxs-lookup"><span data-stu-id="a35ea-113">0</span></span>|<span data-ttu-id="a35ea-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="a35ea-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a35ea-115">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="a35ea-115">everyday</span></span>|<span data-ttu-id="a35ea-116">1</span><span class="sxs-lookup"><span data-stu-id="a35ea-116">1</span></span>|<span data-ttu-id="a35ea-117">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="a35ea-117">Everyday.</span></span>|
|<span data-ttu-id="a35ea-118">日曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-118">sunday</span></span>|<span data-ttu-id="a35ea-119">2</span><span class="sxs-lookup"><span data-stu-id="a35ea-119">2</span></span>|<span data-ttu-id="a35ea-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-120">Sunday.</span></span>|
|<span data-ttu-id="a35ea-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-121">monday</span></span>|<span data-ttu-id="a35ea-122">3</span><span class="sxs-lookup"><span data-stu-id="a35ea-122">3</span></span>|<span data-ttu-id="a35ea-123">月曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-123">Monday.</span></span>|
|<span data-ttu-id="a35ea-124">火曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-124">tuesday</span></span>|<span data-ttu-id="a35ea-125">4</span><span class="sxs-lookup"><span data-stu-id="a35ea-125">4</span></span>|<span data-ttu-id="a35ea-126">火曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-126">Tuesday.</span></span>|
|<span data-ttu-id="a35ea-127">(水)</span><span class="sxs-lookup"><span data-stu-id="a35ea-127">wednesday</span></span>|<span data-ttu-id="a35ea-128">5</span><span class="sxs-lookup"><span data-stu-id="a35ea-128">5</span></span>|<span data-ttu-id="a35ea-129">水曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-129">Wednesday.</span></span>|
|<span data-ttu-id="a35ea-130">(木)</span><span class="sxs-lookup"><span data-stu-id="a35ea-130">thursday</span></span>|<span data-ttu-id="a35ea-131">6</span><span class="sxs-lookup"><span data-stu-id="a35ea-131">6</span></span>|<span data-ttu-id="a35ea-132">木曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-132">Thursday.</span></span>|
|<span data-ttu-id="a35ea-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-133">friday</span></span>|<span data-ttu-id="a35ea-134">7</span><span class="sxs-lookup"><span data-stu-id="a35ea-134">7</span></span>|<span data-ttu-id="a35ea-135">金曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-135">Friday.</span></span>|
|<span data-ttu-id="a35ea-136">土曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-136">saturday</span></span>|<span data-ttu-id="a35ea-137">8</span><span class="sxs-lookup"><span data-stu-id="a35ea-137">8</span></span>|<span data-ttu-id="a35ea-138">土曜日</span><span class="sxs-lookup"><span data-stu-id="a35ea-138">Saturday.</span></span>|





