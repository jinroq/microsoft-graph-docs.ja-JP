---
title: emailSyncSchedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f84c9a5cdb5d9608a34553c2a3a6f05a989b78a8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995064"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="eb73d-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="eb73d-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="eb73d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb73d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb73d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb73d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb73d-106">電子メール同期スケジュールに指定できる値。</span><span class="sxs-lookup"><span data-stu-id="eb73d-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="eb73d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb73d-107">Members</span></span>
|<span data-ttu-id="eb73d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb73d-108">Member</span></span>|<span data-ttu-id="eb73d-109">値</span><span class="sxs-lookup"><span data-stu-id="eb73d-109">Value</span></span>|<span data-ttu-id="eb73d-110">説明</span><span class="sxs-lookup"><span data-stu-id="eb73d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb73d-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="eb73d-111">userDefined</span></span>|<span data-ttu-id="eb73d-112">.0</span><span class="sxs-lookup"><span data-stu-id="eb73d-112">0</span></span>|<span data-ttu-id="eb73d-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="eb73d-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="eb73d-114">Asメッセージの受信</span><span class="sxs-lookup"><span data-stu-id="eb73d-114">asMessagesArrive</span></span>|<span data-ttu-id="eb73d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="eb73d-115">1</span></span>|<span data-ttu-id="eb73d-116">メッセージが到着したときに同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="eb73d-117">手動</span><span class="sxs-lookup"><span data-stu-id="eb73d-117">manual</span></span>|<span data-ttu-id="eb73d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="eb73d-118">2</span></span>|<span data-ttu-id="eb73d-119">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-119">Sync manually.</span></span>|
|<span data-ttu-id="eb73d-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="eb73d-120">fifteenMinutes</span></span>|<span data-ttu-id="eb73d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="eb73d-121">3</span></span>|<span data-ttu-id="eb73d-122">15分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="eb73d-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="eb73d-123">thirtyMinutes</span></span>|<span data-ttu-id="eb73d-124">2/4</span><span class="sxs-lookup"><span data-stu-id="eb73d-124">4</span></span>|<span data-ttu-id="eb73d-125">30分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="eb73d-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="eb73d-126">sixtyMinutes</span></span>|<span data-ttu-id="eb73d-127">5</span><span class="sxs-lookup"><span data-stu-id="eb73d-127">5</span></span>|<span data-ttu-id="eb73d-128">60分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="eb73d-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="eb73d-129">basedOnMyUsage</span></span>|<span data-ttu-id="eb73d-130">シックス</span><span class="sxs-lookup"><span data-stu-id="eb73d-130">6</span></span>|<span data-ttu-id="eb73d-131">自分の使用状況に基づいて同期します。</span><span class="sxs-lookup"><span data-stu-id="eb73d-131">Sync based on my usage.</span></span>|





