---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 265b02e5bc0ce09edbc12345fca01ccbe0b0343b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944535"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="1f570-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="1f570-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="1f570-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f570-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f570-106">週単位のスケジュールに使用できる値。</span><span class="sxs-lookup"><span data-stu-id="1f570-106">Possible values for a weekly schedule.</span></span>

## <a name="members"></a><span data-ttu-id="1f570-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1f570-107">Members</span></span>
|<span data-ttu-id="1f570-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1f570-108">Member</span></span>|<span data-ttu-id="1f570-109">値</span><span class="sxs-lookup"><span data-stu-id="1f570-109">Value</span></span>|<span data-ttu-id="1f570-110">説明</span><span class="sxs-lookup"><span data-stu-id="1f570-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f570-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="1f570-111">userDefined</span></span>|<span data-ttu-id="1f570-112">.0</span><span class="sxs-lookup"><span data-stu-id="1f570-112">0</span></span>|<span data-ttu-id="1f570-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="1f570-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1f570-114">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="1f570-114">everyday</span></span>|<span data-ttu-id="1f570-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1f570-115">1</span></span>|<span data-ttu-id="1f570-116">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="1f570-116">Everyday.</span></span>|
|<span data-ttu-id="1f570-117">n</span><span class="sxs-lookup"><span data-stu-id="1f570-117">sunday</span></span>|<span data-ttu-id="1f570-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="1f570-118">2</span></span>|<span data-ttu-id="1f570-119">日曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-119">Sunday.</span></span>|
|<span data-ttu-id="1f570-120">曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-120">monday</span></span>|<span data-ttu-id="1f570-121">1/3</span><span class="sxs-lookup"><span data-stu-id="1f570-121">3</span></span>|<span data-ttu-id="1f570-122">月曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-122">Monday.</span></span>|
|<span data-ttu-id="1f570-123">毎週</span><span class="sxs-lookup"><span data-stu-id="1f570-123">tuesday</span></span>|<span data-ttu-id="1f570-124">2/4</span><span class="sxs-lookup"><span data-stu-id="1f570-124">4</span></span>|<span data-ttu-id="1f570-125">火曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-125">Tuesday.</span></span>|
|<span data-ttu-id="1f570-126">毎週</span><span class="sxs-lookup"><span data-stu-id="1f570-126">wednesday</span></span>|<span data-ttu-id="1f570-127">5</span><span class="sxs-lookup"><span data-stu-id="1f570-127">5</span></span>|<span data-ttu-id="1f570-128">水曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-128">Wednesday.</span></span>|
|<span data-ttu-id="1f570-129">火曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-129">thursday</span></span>|<span data-ttu-id="1f570-130">シックス</span><span class="sxs-lookup"><span data-stu-id="1f570-130">6</span></span>|<span data-ttu-id="1f570-131">木曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-131">Thursday.</span></span>|
|<span data-ttu-id="1f570-132">金曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-132">friday</span></span>|<span data-ttu-id="1f570-133">7</span><span class="sxs-lookup"><span data-stu-id="1f570-133">7</span></span>|<span data-ttu-id="1f570-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-134">Friday.</span></span>|
|<span data-ttu-id="1f570-135">土日</span><span class="sxs-lookup"><span data-stu-id="1f570-135">saturday</span></span>|<span data-ttu-id="1f570-136">8 </span><span class="sxs-lookup"><span data-stu-id="1f570-136">8</span></span>|<span data-ttu-id="1f570-137">土曜日</span><span class="sxs-lookup"><span data-stu-id="1f570-137">Saturday.</span></span>|




