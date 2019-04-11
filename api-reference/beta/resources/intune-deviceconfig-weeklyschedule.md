---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8899696ace2011440b641ae83849a179dbfd6438
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802836"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="e6481-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="e6481-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="e6481-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6481-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6481-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e6481-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6481-106">週単位のスケジュールに使用できる値。</span><span class="sxs-lookup"><span data-stu-id="e6481-106">Possible values for a weekly schedule.</span></span>

## <a name="members"></a><span data-ttu-id="e6481-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6481-107">Members</span></span>
|<span data-ttu-id="e6481-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6481-108">Member</span></span>|<span data-ttu-id="e6481-109">値</span><span class="sxs-lookup"><span data-stu-id="e6481-109">Value</span></span>|<span data-ttu-id="e6481-110">説明</span><span class="sxs-lookup"><span data-stu-id="e6481-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6481-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e6481-111">userDefined</span></span>|<span data-ttu-id="e6481-112">.0</span><span class="sxs-lookup"><span data-stu-id="e6481-112">0</span></span>|<span data-ttu-id="e6481-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e6481-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e6481-114">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="e6481-114">everyday</span></span>|<span data-ttu-id="e6481-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e6481-115">1</span></span>|<span data-ttu-id="e6481-116">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="e6481-116">Everyday.</span></span>|
|<span data-ttu-id="e6481-117">n</span><span class="sxs-lookup"><span data-stu-id="e6481-117">sunday</span></span>|<span data-ttu-id="e6481-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e6481-118">2</span></span>|<span data-ttu-id="e6481-119">日曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-119">Sunday.</span></span>|
|<span data-ttu-id="e6481-120">曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-120">monday</span></span>|<span data-ttu-id="e6481-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e6481-121">3</span></span>|<span data-ttu-id="e6481-122">月曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-122">Monday.</span></span>|
|<span data-ttu-id="e6481-123">毎週</span><span class="sxs-lookup"><span data-stu-id="e6481-123">tuesday</span></span>|<span data-ttu-id="e6481-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e6481-124">4</span></span>|<span data-ttu-id="e6481-125">火曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-125">Tuesday.</span></span>|
|<span data-ttu-id="e6481-126">毎週</span><span class="sxs-lookup"><span data-stu-id="e6481-126">wednesday</span></span>|<span data-ttu-id="e6481-127">5</span><span class="sxs-lookup"><span data-stu-id="e6481-127">5</span></span>|<span data-ttu-id="e6481-128">水曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-128">Wednesday.</span></span>|
|<span data-ttu-id="e6481-129">火曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-129">thursday</span></span>|<span data-ttu-id="e6481-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e6481-130">6</span></span>|<span data-ttu-id="e6481-131">木曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-131">Thursday.</span></span>|
|<span data-ttu-id="e6481-132">金曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-132">friday</span></span>|<span data-ttu-id="e6481-133">7</span><span class="sxs-lookup"><span data-stu-id="e6481-133">7</span></span>|<span data-ttu-id="e6481-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-134">Friday.</span></span>|
|<span data-ttu-id="e6481-135">土日</span><span class="sxs-lookup"><span data-stu-id="e6481-135">saturday</span></span>|<span data-ttu-id="e6481-136">~</span><span class="sxs-lookup"><span data-stu-id="e6481-136">8</span></span>|<span data-ttu-id="e6481-137">土曜日</span><span class="sxs-lookup"><span data-stu-id="e6481-137">Saturday.</span></span>|





