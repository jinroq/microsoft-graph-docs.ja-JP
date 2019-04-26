---
title: emailsyncschedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1da569d7050e88dd5eb41640bc2d8eaa602bb2b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556222"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="02b0a-103">emailsyncschedule 列挙型</span><span class="sxs-lookup"><span data-stu-id="02b0a-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="02b0a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02b0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02b0a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02b0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b0a-106">電子メール同期スケジュールに指定できる値。</span><span class="sxs-lookup"><span data-stu-id="02b0a-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="02b0a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="02b0a-107">Members</span></span>
|<span data-ttu-id="02b0a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="02b0a-108">Member</span></span>|<span data-ttu-id="02b0a-109">値</span><span class="sxs-lookup"><span data-stu-id="02b0a-109">Value</span></span>|<span data-ttu-id="02b0a-110">説明</span><span class="sxs-lookup"><span data-stu-id="02b0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b0a-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="02b0a-111">userDefined</span></span>|<span data-ttu-id="02b0a-112">.0</span><span class="sxs-lookup"><span data-stu-id="02b0a-112">0</span></span>|<span data-ttu-id="02b0a-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="02b0a-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="02b0a-114">asメッセージの受信</span><span class="sxs-lookup"><span data-stu-id="02b0a-114">asMessagesArrive</span></span>|<span data-ttu-id="02b0a-115">1 </span><span class="sxs-lookup"><span data-stu-id="02b0a-115">1</span></span>|<span data-ttu-id="02b0a-116">メッセージが到着したときに同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="02b0a-117">手動</span><span class="sxs-lookup"><span data-stu-id="02b0a-117">manual</span></span>|<span data-ttu-id="02b0a-118">2 </span><span class="sxs-lookup"><span data-stu-id="02b0a-118">2</span></span>|<span data-ttu-id="02b0a-119">手動で同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-119">Sync manually.</span></span>|
|<span data-ttu-id="02b0a-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="02b0a-120">fifteenMinutes</span></span>|<span data-ttu-id="02b0a-121">3 </span><span class="sxs-lookup"><span data-stu-id="02b0a-121">3</span></span>|<span data-ttu-id="02b0a-122">15分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="02b0a-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="02b0a-123">thirtyMinutes</span></span>|<span data-ttu-id="02b0a-124">4 </span><span class="sxs-lookup"><span data-stu-id="02b0a-124">4</span></span>|<span data-ttu-id="02b0a-125">30分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="02b0a-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="02b0a-126">sixtyMinutes</span></span>|<span data-ttu-id="02b0a-127">5 </span><span class="sxs-lookup"><span data-stu-id="02b0a-127">5</span></span>|<span data-ttu-id="02b0a-128">60分ごとに同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="02b0a-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="02b0a-129">basedOnMyUsage</span></span>|<span data-ttu-id="02b0a-130">6 </span><span class="sxs-lookup"><span data-stu-id="02b0a-130">6</span></span>|<span data-ttu-id="02b0a-131">自分の使用状況に基づいて同期します。</span><span class="sxs-lookup"><span data-stu-id="02b0a-131">Sync based on my usage.</span></span>|





