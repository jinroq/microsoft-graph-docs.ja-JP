---
title: emailSyncSchedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 14b73fc4cfbf9cf53bdab4c2841403cac4077fa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001426"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="19c89-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="19c89-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="19c89-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19c89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19c89-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19c89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c89-106">電子メール同期スケジュールに指定できる値。</span><span class="sxs-lookup"><span data-stu-id="19c89-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="19c89-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19c89-107">Members</span></span>
|<span data-ttu-id="19c89-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19c89-108">Member</span></span>|<span data-ttu-id="19c89-109">値</span><span class="sxs-lookup"><span data-stu-id="19c89-109">Value</span></span>|<span data-ttu-id="19c89-110">説明</span><span class="sxs-lookup"><span data-stu-id="19c89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c89-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="19c89-111">userDefined</span></span>|<span data-ttu-id="19c89-112">.0</span><span class="sxs-lookup"><span data-stu-id="19c89-112">0</span></span>|<span data-ttu-id="19c89-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="19c89-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="19c89-114">Asメッセージの受信</span><span class="sxs-lookup"><span data-stu-id="19c89-114">asMessagesArrive</span></span>|<span data-ttu-id="19c89-115">1-d</span><span class="sxs-lookup"><span data-stu-id="19c89-115">1</span></span>|<span data-ttu-id="19c89-116">メッセージが到着したときに同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="19c89-117">手動</span><span class="sxs-lookup"><span data-stu-id="19c89-117">manual</span></span>|<span data-ttu-id="19c89-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="19c89-118">2</span></span>|<span data-ttu-id="19c89-119">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-119">Sync manually.</span></span>|
|<span data-ttu-id="19c89-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="19c89-120">fifteenMinutes</span></span>|<span data-ttu-id="19c89-121">1/3</span><span class="sxs-lookup"><span data-stu-id="19c89-121">3</span></span>|<span data-ttu-id="19c89-122">15分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="19c89-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="19c89-123">thirtyMinutes</span></span>|<span data-ttu-id="19c89-124">2/4</span><span class="sxs-lookup"><span data-stu-id="19c89-124">4</span></span>|<span data-ttu-id="19c89-125">30分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="19c89-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="19c89-126">sixtyMinutes</span></span>|<span data-ttu-id="19c89-127">5</span><span class="sxs-lookup"><span data-stu-id="19c89-127">5</span></span>|<span data-ttu-id="19c89-128">60分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="19c89-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="19c89-129">basedOnMyUsage</span></span>|<span data-ttu-id="19c89-130">シックス</span><span class="sxs-lookup"><span data-stu-id="19c89-130">6</span></span>|<span data-ttu-id="19c89-131">自分の使用状況に基づいて同期します。</span><span class="sxs-lookup"><span data-stu-id="19c89-131">Sync based on my usage.</span></span>|





