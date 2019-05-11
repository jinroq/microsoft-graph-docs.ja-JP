---
title: emailSyncDuration 列挙型
description: 電子メール同期の期間として指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c6296178a8cd9bb987965944ba02c96aa44a534
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946777"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="e8334-103">emailSyncDuration 列挙型</span><span class="sxs-lookup"><span data-stu-id="e8334-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="e8334-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8334-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8334-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8334-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8334-106">電子メール同期の期間として指定できる値。</span><span class="sxs-lookup"><span data-stu-id="e8334-106">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="e8334-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8334-107">Members</span></span>
|<span data-ttu-id="e8334-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8334-108">Member</span></span>|<span data-ttu-id="e8334-109">値</span><span class="sxs-lookup"><span data-stu-id="e8334-109">Value</span></span>|<span data-ttu-id="e8334-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8334-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8334-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e8334-111">userDefined</span></span>|<span data-ttu-id="e8334-112">.0</span><span class="sxs-lookup"><span data-stu-id="e8334-112">0</span></span>|<span data-ttu-id="e8334-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e8334-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e8334-114">oneDay</span><span class="sxs-lookup"><span data-stu-id="e8334-114">oneDay</span></span>|<span data-ttu-id="e8334-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e8334-115">1</span></span>|<span data-ttu-id="e8334-116">1日分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-116">Sync one day of email.</span></span>|
|<span data-ttu-id="e8334-117">threeDays</span><span class="sxs-lookup"><span data-stu-id="e8334-117">threeDays</span></span>|<span data-ttu-id="e8334-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e8334-118">2</span></span>|<span data-ttu-id="e8334-119">3日間のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-119">Sync three days of email.</span></span>|
|<span data-ttu-id="e8334-120">oneWeek</span><span class="sxs-lookup"><span data-stu-id="e8334-120">oneWeek</span></span>|<span data-ttu-id="e8334-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e8334-121">3</span></span>|<span data-ttu-id="e8334-122">電子メールの1週間を同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-122">Sync one week of email.</span></span>|
|<span data-ttu-id="e8334-123">2週間</span><span class="sxs-lookup"><span data-stu-id="e8334-123">twoWeeks</span></span>|<span data-ttu-id="e8334-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e8334-124">4</span></span>|<span data-ttu-id="e8334-125">2週間のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-125">Sync two weeks of email.</span></span>|
|<span data-ttu-id="e8334-126">オンライン</span><span class="sxs-lookup"><span data-stu-id="e8334-126">oneMonth</span></span>|<span data-ttu-id="e8334-127">5</span><span class="sxs-lookup"><span data-stu-id="e8334-127">5</span></span>|<span data-ttu-id="e8334-128">1か月分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-128">Sync one month of email.</span></span>|
|<span data-ttu-id="e8334-129">無制限</span><span class="sxs-lookup"><span data-stu-id="e8334-129">unlimited</span></span>|<span data-ttu-id="e8334-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e8334-130">6</span></span>|<span data-ttu-id="e8334-131">電子メールの期間を無制限に同期します。</span><span class="sxs-lookup"><span data-stu-id="e8334-131">Sync an unlimited duration of email.</span></span>|




