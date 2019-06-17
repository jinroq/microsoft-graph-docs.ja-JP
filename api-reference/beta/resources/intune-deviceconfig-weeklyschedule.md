---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af637a0a09bacec8771321f586c887e7573e82eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991605"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="2bdc6-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="2bdc6-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="2bdc6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bdc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bdc6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bdc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdc6-106">週単位のスケジュールに使用できる値。</span><span class="sxs-lookup"><span data-stu-id="2bdc6-106">Possible values for a weekly schedule.</span></span>

## <a name="members"></a><span data-ttu-id="2bdc6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2bdc6-107">Members</span></span>
|<span data-ttu-id="2bdc6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2bdc6-108">Member</span></span>|<span data-ttu-id="2bdc6-109">値</span><span class="sxs-lookup"><span data-stu-id="2bdc6-109">Value</span></span>|<span data-ttu-id="2bdc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="2bdc6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdc6-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="2bdc6-111">userDefined</span></span>|<span data-ttu-id="2bdc6-112">.0</span><span class="sxs-lookup"><span data-stu-id="2bdc6-112">0</span></span>|<span data-ttu-id="2bdc6-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="2bdc6-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2bdc6-114">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-114">everyday</span></span>|<span data-ttu-id="2bdc6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="2bdc6-115">1</span></span>|<span data-ttu-id="2bdc6-116">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="2bdc6-116">Everyday.</span></span>|
|<span data-ttu-id="2bdc6-117">n</span><span class="sxs-lookup"><span data-stu-id="2bdc6-117">sunday</span></span>|<span data-ttu-id="2bdc6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="2bdc6-118">2</span></span>|<span data-ttu-id="2bdc6-119">日曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-119">Sunday.</span></span>|
|<span data-ttu-id="2bdc6-120">曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-120">monday</span></span>|<span data-ttu-id="2bdc6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="2bdc6-121">3</span></span>|<span data-ttu-id="2bdc6-122">月曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-122">Monday.</span></span>|
|<span data-ttu-id="2bdc6-123">毎週</span><span class="sxs-lookup"><span data-stu-id="2bdc6-123">tuesday</span></span>|<span data-ttu-id="2bdc6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="2bdc6-124">4</span></span>|<span data-ttu-id="2bdc6-125">火曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-125">Tuesday.</span></span>|
|<span data-ttu-id="2bdc6-126">毎週</span><span class="sxs-lookup"><span data-stu-id="2bdc6-126">wednesday</span></span>|<span data-ttu-id="2bdc6-127">5</span><span class="sxs-lookup"><span data-stu-id="2bdc6-127">5</span></span>|<span data-ttu-id="2bdc6-128">水曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-128">Wednesday.</span></span>|
|<span data-ttu-id="2bdc6-129">火曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-129">thursday</span></span>|<span data-ttu-id="2bdc6-130">シックス</span><span class="sxs-lookup"><span data-stu-id="2bdc6-130">6</span></span>|<span data-ttu-id="2bdc6-131">木曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-131">Thursday.</span></span>|
|<span data-ttu-id="2bdc6-132">金曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-132">friday</span></span>|<span data-ttu-id="2bdc6-133">7</span><span class="sxs-lookup"><span data-stu-id="2bdc6-133">7</span></span>|<span data-ttu-id="2bdc6-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-134">Friday.</span></span>|
|<span data-ttu-id="2bdc6-135">土日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-135">saturday</span></span>|<span data-ttu-id="2bdc6-136">8 </span><span class="sxs-lookup"><span data-stu-id="2bdc6-136">8</span></span>|<span data-ttu-id="2bdc6-137">土曜日</span><span class="sxs-lookup"><span data-stu-id="2bdc6-137">Saturday.</span></span>|





