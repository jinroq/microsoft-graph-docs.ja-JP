---
title: ratingUnitedStatesMoviesType 列挙型
description: 映画が米国でのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 22861c0b05fc6a3dacbf520d03ee04b516dad3e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887844"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="4b685-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4b685-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="4b685-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b685-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b685-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b685-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b685-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b685-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b685-107">映画が米国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="4b685-107">Movies rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="4b685-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b685-108">Members</span></span>
|<span data-ttu-id="4b685-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b685-109">Member</span></span>|<span data-ttu-id="4b685-110">値</span><span class="sxs-lookup"><span data-stu-id="4b685-110">Value</span></span>|<span data-ttu-id="4b685-111">説明</span><span class="sxs-lookup"><span data-stu-id="4b685-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b685-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4b685-112">allAllowed</span></span>|<span data-ttu-id="4b685-113">0</span><span class="sxs-lookup"><span data-stu-id="4b685-113">0</span></span>|<span data-ttu-id="4b685-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="4b685-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="4b685-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4b685-115">allBlocked</span></span>|<span data-ttu-id="4b685-116">1</span><span class="sxs-lookup"><span data-stu-id="4b685-116">1</span></span>|<span data-ttu-id="4b685-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="4b685-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="4b685-118">全般</span><span class="sxs-lookup"><span data-stu-id="4b685-118">general</span></span>|<span data-ttu-id="4b685-119">2</span><span class="sxs-lookup"><span data-stu-id="4b685-119">2</span></span>|<span data-ttu-id="4b685-120">G、すべての年代の参加を許可</span><span class="sxs-lookup"><span data-stu-id="4b685-120">G, all ages admitted</span></span>|
|<span data-ttu-id="4b685-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="4b685-121">parentalGuidance</span></span>|<span data-ttu-id="4b685-122">3</span><span class="sxs-lookup"><span data-stu-id="4b685-122">3</span></span>|<span data-ttu-id="4b685-123">PG、可能性がありますだと内容が子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="4b685-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="4b685-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="4b685-124">parentalGuidance13</span></span>|<span data-ttu-id="4b685-125">4</span><span class="sxs-lookup"><span data-stu-id="4b685-125">4</span></span>|<span data-ttu-id="4b685-126">PG13、いくつかの材料があります 13 才未満の子供に適切です</span><span class="sxs-lookup"><span data-stu-id="4b685-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="4b685-127">制限</span><span class="sxs-lookup"><span data-stu-id="4b685-127">restricted</span></span>|<span data-ttu-id="4b685-128">5</span><span class="sxs-lookup"><span data-stu-id="4b685-128">5</span></span>|<span data-ttu-id="4b685-129">親または大人の同伴に付属する R、17 歳未満の閲覧者が必要な</span><span class="sxs-lookup"><span data-stu-id="4b685-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="4b685-130">大人</span><span class="sxs-lookup"><span data-stu-id="4b685-130">adults</span></span>|<span data-ttu-id="4b685-131">6</span><span class="sxs-lookup"><span data-stu-id="4b685-131">6</span></span>|<span data-ttu-id="4b685-132">NC17、成人のみ</span><span class="sxs-lookup"><span data-stu-id="4b685-132">NC17, adults only</span></span>|





