---
title: weeklySchedule 列挙型
description: 週単位のスケジュールに使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b35be5a180324ca6dfe6fccd7cc8aaf01ae47a0c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151108"
---
# <a name="weeklyschedule-enum-type"></a><span data-ttu-id="f0c72-103">weeklySchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="f0c72-103">weeklySchedule enum type</span></span>

> <span data-ttu-id="f0c72-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0c72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0c72-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0c72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0c72-106">週単位のスケジュールに使用できる値。</span><span class="sxs-lookup"><span data-stu-id="f0c72-106">Possible values for a weekly schedule.</span></span>

## <a name="members"></a><span data-ttu-id="f0c72-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0c72-107">Members</span></span>
|<span data-ttu-id="f0c72-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0c72-108">Member</span></span>|<span data-ttu-id="f0c72-109">値</span><span class="sxs-lookup"><span data-stu-id="f0c72-109">Value</span></span>|<span data-ttu-id="f0c72-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0c72-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0c72-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="f0c72-111">userDefined</span></span>|<span data-ttu-id="f0c72-112">.0</span><span class="sxs-lookup"><span data-stu-id="f0c72-112">0</span></span>|<span data-ttu-id="f0c72-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f0c72-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f0c72-114">毎日毎日</span><span class="sxs-lookup"><span data-stu-id="f0c72-114">everyday</span></span>|<span data-ttu-id="f0c72-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f0c72-115">1</span></span>|<span data-ttu-id="f0c72-116">毎日毎日。</span><span class="sxs-lookup"><span data-stu-id="f0c72-116">Everyday.</span></span>|
|<span data-ttu-id="f0c72-117">n</span><span class="sxs-lookup"><span data-stu-id="f0c72-117">sunday</span></span>|<span data-ttu-id="f0c72-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f0c72-118">2</span></span>|<span data-ttu-id="f0c72-119">日曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-119">Sunday.</span></span>|
|<span data-ttu-id="f0c72-120">曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-120">monday</span></span>|<span data-ttu-id="f0c72-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f0c72-121">3</span></span>|<span data-ttu-id="f0c72-122">月曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-122">Monday.</span></span>|
|<span data-ttu-id="f0c72-123">毎週</span><span class="sxs-lookup"><span data-stu-id="f0c72-123">tuesday</span></span>|<span data-ttu-id="f0c72-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f0c72-124">4</span></span>|<span data-ttu-id="f0c72-125">火曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-125">Tuesday.</span></span>|
|<span data-ttu-id="f0c72-126">毎週</span><span class="sxs-lookup"><span data-stu-id="f0c72-126">wednesday</span></span>|<span data-ttu-id="f0c72-127">5</span><span class="sxs-lookup"><span data-stu-id="f0c72-127">5</span></span>|<span data-ttu-id="f0c72-128">水曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-128">Wednesday.</span></span>|
|<span data-ttu-id="f0c72-129">火曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-129">thursday</span></span>|<span data-ttu-id="f0c72-130">シックス</span><span class="sxs-lookup"><span data-stu-id="f0c72-130">6</span></span>|<span data-ttu-id="f0c72-131">木曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-131">Thursday.</span></span>|
|<span data-ttu-id="f0c72-132">金曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-132">friday</span></span>|<span data-ttu-id="f0c72-133">7</span><span class="sxs-lookup"><span data-stu-id="f0c72-133">7</span></span>|<span data-ttu-id="f0c72-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-134">Friday.</span></span>|
|<span data-ttu-id="f0c72-135">土日</span><span class="sxs-lookup"><span data-stu-id="f0c72-135">saturday</span></span>|<span data-ttu-id="f0c72-136">~</span><span class="sxs-lookup"><span data-stu-id="f0c72-136">8</span></span>|<span data-ttu-id="f0c72-137">土曜日</span><span class="sxs-lookup"><span data-stu-id="f0c72-137">Saturday.</span></span>|




