---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac2380b38c88c6f5cd35b333cdfcded3c4ee11fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928431"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="f87fb-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="f87fb-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="f87fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f87fb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f87fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f87fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f87fb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f87fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f87fb-107">週単位のスケジュールに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="f87fb-107">Possible values for a weekly schedule.</span></span>
## <a name="members"></a><span data-ttu-id="f87fb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f87fb-108">Members</span></span>
|<span data-ttu-id="f87fb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f87fb-109">Member</span></span>|<span data-ttu-id="f87fb-110">値</span><span class="sxs-lookup"><span data-stu-id="f87fb-110">Value</span></span>|<span data-ttu-id="f87fb-111">説明</span><span class="sxs-lookup"><span data-stu-id="f87fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f87fb-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="f87fb-112">userDefined</span></span>|<span data-ttu-id="f87fb-113">0</span><span class="sxs-lookup"><span data-stu-id="f87fb-113">0</span></span>|<span data-ttu-id="f87fb-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="f87fb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f87fb-115">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="f87fb-115">everyday</span></span>|<span data-ttu-id="f87fb-116">1</span><span class="sxs-lookup"><span data-stu-id="f87fb-116">1</span></span>|<span data-ttu-id="f87fb-117">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="f87fb-117">Everyday.</span></span>|
|<span data-ttu-id="f87fb-118">日曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-118">sunday</span></span>|<span data-ttu-id="f87fb-119">2</span><span class="sxs-lookup"><span data-stu-id="f87fb-119">2</span></span>|<span data-ttu-id="f87fb-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-120">Sunday.</span></span>|
|<span data-ttu-id="f87fb-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-121">monday</span></span>|<span data-ttu-id="f87fb-122">3</span><span class="sxs-lookup"><span data-stu-id="f87fb-122">3</span></span>|<span data-ttu-id="f87fb-123">月曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-123">Monday.</span></span>|
|<span data-ttu-id="f87fb-124">火曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-124">tuesday</span></span>|<span data-ttu-id="f87fb-125">4</span><span class="sxs-lookup"><span data-stu-id="f87fb-125">4</span></span>|<span data-ttu-id="f87fb-126">火曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-126">Tuesday.</span></span>|
|<span data-ttu-id="f87fb-127">(水)</span><span class="sxs-lookup"><span data-stu-id="f87fb-127">wednesday</span></span>|<span data-ttu-id="f87fb-128">5</span><span class="sxs-lookup"><span data-stu-id="f87fb-128">5</span></span>|<span data-ttu-id="f87fb-129">水曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-129">Wednesday.</span></span>|
|<span data-ttu-id="f87fb-130">(木)</span><span class="sxs-lookup"><span data-stu-id="f87fb-130">thursday</span></span>|<span data-ttu-id="f87fb-131">6</span><span class="sxs-lookup"><span data-stu-id="f87fb-131">6</span></span>|<span data-ttu-id="f87fb-132">木曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-132">Thursday.</span></span>|
|<span data-ttu-id="f87fb-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-133">friday</span></span>|<span data-ttu-id="f87fb-134">7</span><span class="sxs-lookup"><span data-stu-id="f87fb-134">7</span></span>|<span data-ttu-id="f87fb-135">金曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-135">Friday.</span></span>|
|<span data-ttu-id="f87fb-136">土曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-136">saturday</span></span>|<span data-ttu-id="f87fb-137">8</span><span class="sxs-lookup"><span data-stu-id="f87fb-137">8</span></span>|<span data-ttu-id="f87fb-138">土曜日</span><span class="sxs-lookup"><span data-stu-id="f87fb-138">Saturday.</span></span>|





