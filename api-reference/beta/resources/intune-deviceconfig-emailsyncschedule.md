---
title: emailSyncSchedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4d3645ea2c0eaa7f8f1cf8138f1c0727cfa0d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325632"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="980b3-103">emailSyncSchedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="980b3-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="980b3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="980b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="980b3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="980b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="980b3-106">電子メール同期スケジュールに指定できる値。</span><span class="sxs-lookup"><span data-stu-id="980b3-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="980b3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="980b3-107">Members</span></span>
|<span data-ttu-id="980b3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="980b3-108">Member</span></span>|<span data-ttu-id="980b3-109">値</span><span class="sxs-lookup"><span data-stu-id="980b3-109">Value</span></span>|<span data-ttu-id="980b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="980b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="980b3-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="980b3-111">userDefined</span></span>|<span data-ttu-id="980b3-112">.0</span><span class="sxs-lookup"><span data-stu-id="980b3-112">0</span></span>|<span data-ttu-id="980b3-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="980b3-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="980b3-114">Asメッセージの受信</span><span class="sxs-lookup"><span data-stu-id="980b3-114">asMessagesArrive</span></span>|<span data-ttu-id="980b3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="980b3-115">1</span></span>|<span data-ttu-id="980b3-116">メッセージが到着したときに同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="980b3-117">手動</span><span class="sxs-lookup"><span data-stu-id="980b3-117">manual</span></span>|<span data-ttu-id="980b3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="980b3-118">2</span></span>|<span data-ttu-id="980b3-119">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-119">Sync manually.</span></span>|
|<span data-ttu-id="980b3-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="980b3-120">fifteenMinutes</span></span>|<span data-ttu-id="980b3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="980b3-121">3</span></span>|<span data-ttu-id="980b3-122">15分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="980b3-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="980b3-123">thirtyMinutes</span></span>|<span data-ttu-id="980b3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="980b3-124">4</span></span>|<span data-ttu-id="980b3-125">30分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="980b3-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="980b3-126">sixtyMinutes</span></span>|<span data-ttu-id="980b3-127">5</span><span class="sxs-lookup"><span data-stu-id="980b3-127">5</span></span>|<span data-ttu-id="980b3-128">60分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="980b3-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="980b3-129">basedOnMyUsage</span></span>|<span data-ttu-id="980b3-130">シックス</span><span class="sxs-lookup"><span data-stu-id="980b3-130">6</span></span>|<span data-ttu-id="980b3-131">自分の使用状況に基づいて同期します。</span><span class="sxs-lookup"><span data-stu-id="980b3-131">Sync based on my usage.</span></span>|



