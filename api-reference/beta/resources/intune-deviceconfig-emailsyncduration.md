---
title: emailSyncDuration 列挙型
description: 電子メール同期の期間として指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fc05be47c2adc0764a2cdb1e69f7ec11413320cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357195"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="058ec-103">emailSyncDuration 列挙型</span><span class="sxs-lookup"><span data-stu-id="058ec-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="058ec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="058ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="058ec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="058ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="058ec-106">電子メール同期の期間として指定できる値。</span><span class="sxs-lookup"><span data-stu-id="058ec-106">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="058ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="058ec-107">Members</span></span>
|<span data-ttu-id="058ec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="058ec-108">Member</span></span>|<span data-ttu-id="058ec-109">値</span><span class="sxs-lookup"><span data-stu-id="058ec-109">Value</span></span>|<span data-ttu-id="058ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="058ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="058ec-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="058ec-111">userDefined</span></span>|<span data-ttu-id="058ec-112">.0</span><span class="sxs-lookup"><span data-stu-id="058ec-112">0</span></span>|<span data-ttu-id="058ec-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="058ec-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="058ec-114">oneDay</span><span class="sxs-lookup"><span data-stu-id="058ec-114">oneDay</span></span>|<span data-ttu-id="058ec-115">1-d</span><span class="sxs-lookup"><span data-stu-id="058ec-115">1</span></span>|<span data-ttu-id="058ec-116">1日分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-116">Sync one day of email.</span></span>|
|<span data-ttu-id="058ec-117">threeDays</span><span class="sxs-lookup"><span data-stu-id="058ec-117">threeDays</span></span>|<span data-ttu-id="058ec-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="058ec-118">2</span></span>|<span data-ttu-id="058ec-119">3日間のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-119">Sync three days of email.</span></span>|
|<span data-ttu-id="058ec-120">oneWeek</span><span class="sxs-lookup"><span data-stu-id="058ec-120">oneWeek</span></span>|<span data-ttu-id="058ec-121">1/3</span><span class="sxs-lookup"><span data-stu-id="058ec-121">3</span></span>|<span data-ttu-id="058ec-122">電子メールの1週間を同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-122">Sync one week of email.</span></span>|
|<span data-ttu-id="058ec-123">2週間</span><span class="sxs-lookup"><span data-stu-id="058ec-123">twoWeeks</span></span>|<span data-ttu-id="058ec-124">2/4</span><span class="sxs-lookup"><span data-stu-id="058ec-124">4</span></span>|<span data-ttu-id="058ec-125">2週間のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-125">Sync two weeks of email.</span></span>|
|<span data-ttu-id="058ec-126">オンライン</span><span class="sxs-lookup"><span data-stu-id="058ec-126">oneMonth</span></span>|<span data-ttu-id="058ec-127">5</span><span class="sxs-lookup"><span data-stu-id="058ec-127">5</span></span>|<span data-ttu-id="058ec-128">1か月分のメールを同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-128">Sync one month of email.</span></span>|
|<span data-ttu-id="058ec-129">無制限</span><span class="sxs-lookup"><span data-stu-id="058ec-129">unlimited</span></span>|<span data-ttu-id="058ec-130">シックス</span><span class="sxs-lookup"><span data-stu-id="058ec-130">6</span></span>|<span data-ttu-id="058ec-131">電子メールの期間を無制限に同期します。</span><span class="sxs-lookup"><span data-stu-id="058ec-131">Sync an unlimited duration of email.</span></span>|



