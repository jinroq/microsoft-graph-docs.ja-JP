---
title: emailSyncDuration 列挙型
description: 電子メールに使用できる値は、時間を同期します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399410"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="4aae3-103">emailSyncDuration 列挙型</span><span class="sxs-lookup"><span data-stu-id="4aae3-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="4aae3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4aae3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4aae3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4aae3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4aae3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4aae3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aae3-107">電子メールに使用できる値は、時間を同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="4aae3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4aae3-108">Members</span></span>
|<span data-ttu-id="4aae3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4aae3-109">Member</span></span>|<span data-ttu-id="4aae3-110">値</span><span class="sxs-lookup"><span data-stu-id="4aae3-110">Value</span></span>|<span data-ttu-id="4aae3-111">説明</span><span class="sxs-lookup"><span data-stu-id="4aae3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aae3-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="4aae3-112">userDefined</span></span>|<span data-ttu-id="4aae3-113">0</span><span class="sxs-lookup"><span data-stu-id="4aae3-113">0</span></span>|<span data-ttu-id="4aae3-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="4aae3-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="4aae3-115">直後</span><span class="sxs-lookup"><span data-stu-id="4aae3-115">oneDay</span></span>|<span data-ttu-id="4aae3-116">1</span><span class="sxs-lookup"><span data-stu-id="4aae3-116">1</span></span>|<span data-ttu-id="4aae3-117">1 日分の電子メールを同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-117">Sync one day of email.</span></span>|
|<span data-ttu-id="4aae3-118">3 日</span><span class="sxs-lookup"><span data-stu-id="4aae3-118">threeDays</span></span>|<span data-ttu-id="4aae3-119">2</span><span class="sxs-lookup"><span data-stu-id="4aae3-119">2</span></span>|<span data-ttu-id="4aae3-120">3 日間の電子メールを同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-120">Sync three days of email.</span></span>|
|<span data-ttu-id="4aae3-121">1 週間</span><span class="sxs-lookup"><span data-stu-id="4aae3-121">oneWeek</span></span>|<span data-ttu-id="4aae3-122">3</span><span class="sxs-lookup"><span data-stu-id="4aae3-122">3</span></span>|<span data-ttu-id="4aae3-123">1 週間分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-123">Sync one week of email.</span></span>|
|<span data-ttu-id="4aae3-124">2 週間</span><span class="sxs-lookup"><span data-stu-id="4aae3-124">twoWeeks</span></span>|<span data-ttu-id="4aae3-125">4</span><span class="sxs-lookup"><span data-stu-id="4aae3-125">4</span></span>|<span data-ttu-id="4aae3-126">2 週間分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="4aae3-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="4aae3-127">oneMonth</span></span>|<span data-ttu-id="4aae3-128">5</span><span class="sxs-lookup"><span data-stu-id="4aae3-128">5</span></span>|<span data-ttu-id="4aae3-129">電子メールの 1 か月を同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-129">Sync one month of email.</span></span>|
|<span data-ttu-id="4aae3-130">無制限</span><span class="sxs-lookup"><span data-stu-id="4aae3-130">unlimited</span></span>|<span data-ttu-id="4aae3-131">6</span><span class="sxs-lookup"><span data-stu-id="4aae3-131">6</span></span>|<span data-ttu-id="4aae3-132">電子メールの無制限の時間を同期します。</span><span class="sxs-lookup"><span data-stu-id="4aae3-132">Sync an unlimited duration of email.</span></span>|




