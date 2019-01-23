---
title: emailSyncSchedule 列挙型
description: 電子メールの同期スケジュールの可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425184"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="0263d-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="0263d-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="0263d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0263d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0263d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0263d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0263d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0263d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0263d-107">電子メールの同期スケジュールの可能な値です。</span><span class="sxs-lookup"><span data-stu-id="0263d-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="0263d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0263d-108">Members</span></span>
|<span data-ttu-id="0263d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0263d-109">Member</span></span>|<span data-ttu-id="0263d-110">値</span><span class="sxs-lookup"><span data-stu-id="0263d-110">Value</span></span>|<span data-ttu-id="0263d-111">説明</span><span class="sxs-lookup"><span data-stu-id="0263d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0263d-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="0263d-112">userDefined</span></span>|<span data-ttu-id="0263d-113">0</span><span class="sxs-lookup"><span data-stu-id="0263d-113">0</span></span>|<span data-ttu-id="0263d-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="0263d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="0263d-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="0263d-115">asMessagesArrive</span></span>|<span data-ttu-id="0263d-116">1</span><span class="sxs-lookup"><span data-stu-id="0263d-116">1</span></span>|<span data-ttu-id="0263d-117">メッセージの受信時に同期します。</span><span class="sxs-lookup"><span data-stu-id="0263d-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="0263d-118">手動</span><span class="sxs-lookup"><span data-stu-id="0263d-118">manual</span></span>|<span data-ttu-id="0263d-119">2</span><span class="sxs-lookup"><span data-stu-id="0263d-119">2</span></span>|<span data-ttu-id="0263d-120">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="0263d-120">Sync manually.</span></span>|
|<span data-ttu-id="0263d-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="0263d-121">fifteenMinutes</span></span>|<span data-ttu-id="0263d-122">3</span><span class="sxs-lookup"><span data-stu-id="0263d-122">3</span></span>|<span data-ttu-id="0263d-123">15 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="0263d-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="0263d-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="0263d-124">thirtyMinutes</span></span>|<span data-ttu-id="0263d-125">4</span><span class="sxs-lookup"><span data-stu-id="0263d-125">4</span></span>|<span data-ttu-id="0263d-126">30 分ごとの同期します。</span><span class="sxs-lookup"><span data-stu-id="0263d-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="0263d-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="0263d-127">sixtyMinutes</span></span>|<span data-ttu-id="0263d-128">5</span><span class="sxs-lookup"><span data-stu-id="0263d-128">5</span></span>|<span data-ttu-id="0263d-129">同期は 60 分ごと。</span><span class="sxs-lookup"><span data-stu-id="0263d-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="0263d-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="0263d-130">basedOnMyUsage</span></span>|<span data-ttu-id="0263d-131">6</span><span class="sxs-lookup"><span data-stu-id="0263d-131">6</span></span>|<span data-ttu-id="0263d-132">私の使用率に基づく同期。</span><span class="sxs-lookup"><span data-stu-id="0263d-132">Sync based on my usage.</span></span>|




