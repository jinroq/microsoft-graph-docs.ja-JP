---
title: emailSyncDuration 列挙型
description: 電子メールに使用できる値は、時間を同期します。
ms.openlocfilehash: 93b15c3fd8f20e8285fd8f4f78da79234e24ebc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069353"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="47bb4-103">emailSyncDuration 列挙型</span><span class="sxs-lookup"><span data-stu-id="47bb4-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="47bb4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47bb4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47bb4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47bb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47bb4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47bb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47bb4-107">電子メールに使用できる値は、時間を同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="47bb4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="47bb4-108">Members</span></span>
|<span data-ttu-id="47bb4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="47bb4-109">Member</span></span>|<span data-ttu-id="47bb4-110">値</span><span class="sxs-lookup"><span data-stu-id="47bb4-110">Value</span></span>|<span data-ttu-id="47bb4-111">説明</span><span class="sxs-lookup"><span data-stu-id="47bb4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47bb4-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="47bb4-112">userDefined</span></span>|<span data-ttu-id="47bb4-113">0</span><span class="sxs-lookup"><span data-stu-id="47bb4-113">0</span></span>|<span data-ttu-id="47bb4-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="47bb4-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="47bb4-115">直後</span><span class="sxs-lookup"><span data-stu-id="47bb4-115">oneDay</span></span>|<span data-ttu-id="47bb4-116">1</span><span class="sxs-lookup"><span data-stu-id="47bb4-116">1</span></span>|<span data-ttu-id="47bb4-117">1 日分の電子メールを同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-117">Sync one day of email.</span></span>|
|<span data-ttu-id="47bb4-118">3 日</span><span class="sxs-lookup"><span data-stu-id="47bb4-118">threeDays</span></span>|<span data-ttu-id="47bb4-119">2</span><span class="sxs-lookup"><span data-stu-id="47bb4-119">2</span></span>|<span data-ttu-id="47bb4-120">3 日間の電子メールを同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-120">Sync three days of email.</span></span>|
|<span data-ttu-id="47bb4-121">1 週間</span><span class="sxs-lookup"><span data-stu-id="47bb4-121">oneWeek</span></span>|<span data-ttu-id="47bb4-122">3</span><span class="sxs-lookup"><span data-stu-id="47bb4-122">3</span></span>|<span data-ttu-id="47bb4-123">1 週間分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-123">Sync one week of email.</span></span>|
|<span data-ttu-id="47bb4-124">2 週間</span><span class="sxs-lookup"><span data-stu-id="47bb4-124">twoWeeks</span></span>|<span data-ttu-id="47bb4-125">4</span><span class="sxs-lookup"><span data-stu-id="47bb4-125">4</span></span>|<span data-ttu-id="47bb4-126">2 週間分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="47bb4-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="47bb4-127">oneMonth</span></span>|<span data-ttu-id="47bb4-128">5</span><span class="sxs-lookup"><span data-stu-id="47bb4-128">5</span></span>|<span data-ttu-id="47bb4-129">電子メールの 1 か月を同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-129">Sync one month of email.</span></span>|
|<span data-ttu-id="47bb4-130">無制限</span><span class="sxs-lookup"><span data-stu-id="47bb4-130">unlimited</span></span>|<span data-ttu-id="47bb4-131">6</span><span class="sxs-lookup"><span data-stu-id="47bb4-131">6</span></span>|<span data-ttu-id="47bb4-132">電子メールの無制限の時間を同期します。</span><span class="sxs-lookup"><span data-stu-id="47bb4-132">Sync an unlimited duration of email.</span></span>|





