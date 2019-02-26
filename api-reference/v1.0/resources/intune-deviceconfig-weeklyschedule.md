---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04773d2c23dde1d103e2865e6cc8d731337e38a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263022"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="e99b7-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="e99b7-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="e99b7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e99b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e99b7-105">週単位のスケジュールに使用できる値。</span><span class="sxs-lookup"><span data-stu-id="e99b7-105">Possible values for a weekly schedule.</span></span>

## <a name="members"></a><span data-ttu-id="e99b7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e99b7-106">Members</span></span>
|<span data-ttu-id="e99b7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e99b7-107">Member</span></span>|<span data-ttu-id="e99b7-108">値</span><span class="sxs-lookup"><span data-stu-id="e99b7-108">Value</span></span>|<span data-ttu-id="e99b7-109">説明</span><span class="sxs-lookup"><span data-stu-id="e99b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e99b7-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e99b7-110">userDefined</span></span>|<span data-ttu-id="e99b7-111">.0</span><span class="sxs-lookup"><span data-stu-id="e99b7-111">0</span></span>|<span data-ttu-id="e99b7-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e99b7-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e99b7-113">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="e99b7-113">everyday</span></span>|<span data-ttu-id="e99b7-114">1-d</span><span class="sxs-lookup"><span data-stu-id="e99b7-114">1</span></span>|<span data-ttu-id="e99b7-115">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="e99b7-115">Everyday.</span></span>|
|<span data-ttu-id="e99b7-116">n</span><span class="sxs-lookup"><span data-stu-id="e99b7-116">sunday</span></span>|<span data-ttu-id="e99b7-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e99b7-117">2</span></span>|<span data-ttu-id="e99b7-118">日曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-118">Sunday.</span></span>|
|<span data-ttu-id="e99b7-119">曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-119">monday</span></span>|<span data-ttu-id="e99b7-120">1/3</span><span class="sxs-lookup"><span data-stu-id="e99b7-120">3</span></span>|<span data-ttu-id="e99b7-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-121">Monday.</span></span>|
|<span data-ttu-id="e99b7-122">毎週</span><span class="sxs-lookup"><span data-stu-id="e99b7-122">tuesday</span></span>|<span data-ttu-id="e99b7-123">2/4</span><span class="sxs-lookup"><span data-stu-id="e99b7-123">4</span></span>|<span data-ttu-id="e99b7-124">火曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-124">Tuesday.</span></span>|
|<span data-ttu-id="e99b7-125">毎週</span><span class="sxs-lookup"><span data-stu-id="e99b7-125">wednesday</span></span>|<span data-ttu-id="e99b7-126">5</span><span class="sxs-lookup"><span data-stu-id="e99b7-126">5</span></span>|<span data-ttu-id="e99b7-127">水曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-127">Wednesday.</span></span>|
|<span data-ttu-id="e99b7-128">火曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-128">thursday</span></span>|<span data-ttu-id="e99b7-129">シックス</span><span class="sxs-lookup"><span data-stu-id="e99b7-129">6</span></span>|<span data-ttu-id="e99b7-130">木曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-130">Thursday.</span></span>|
|<span data-ttu-id="e99b7-131">金曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-131">friday</span></span>|<span data-ttu-id="e99b7-132">7</span><span class="sxs-lookup"><span data-stu-id="e99b7-132">7</span></span>|<span data-ttu-id="e99b7-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-133">Friday.</span></span>|
|<span data-ttu-id="e99b7-134">土日</span><span class="sxs-lookup"><span data-stu-id="e99b7-134">saturday</span></span>|<span data-ttu-id="e99b7-135">~</span><span class="sxs-lookup"><span data-stu-id="e99b7-135">8</span></span>|<span data-ttu-id="e99b7-136">土曜日</span><span class="sxs-lookup"><span data-stu-id="e99b7-136">Saturday.</span></span>|



