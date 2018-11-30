---
title: ratingUnitedStatesMoviesType 列挙型
description: 映画が米国でのラベルの評価
ms.openlocfilehash: a281f9c2d50a4f2b960e98422501e73c256fc6ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067844"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="d73e3-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d73e3-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="d73e3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d73e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d73e3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d73e3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d73e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d73e3-107">映画が米国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="d73e3-107">Movies rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="d73e3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d73e3-108">Members</span></span>
|<span data-ttu-id="d73e3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d73e3-109">Member</span></span>|<span data-ttu-id="d73e3-110">値</span><span class="sxs-lookup"><span data-stu-id="d73e3-110">Value</span></span>|<span data-ttu-id="d73e3-111">説明</span><span class="sxs-lookup"><span data-stu-id="d73e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d73e3-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d73e3-112">allAllowed</span></span>|<span data-ttu-id="d73e3-113">0</span><span class="sxs-lookup"><span data-stu-id="d73e3-113">0</span></span>|<span data-ttu-id="d73e3-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="d73e3-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="d73e3-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d73e3-115">allBlocked</span></span>|<span data-ttu-id="d73e3-116">1</span><span class="sxs-lookup"><span data-stu-id="d73e3-116">1</span></span>|<span data-ttu-id="d73e3-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="d73e3-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="d73e3-118">全般</span><span class="sxs-lookup"><span data-stu-id="d73e3-118">general</span></span>|<span data-ttu-id="d73e3-119">2</span><span class="sxs-lookup"><span data-stu-id="d73e3-119">2</span></span>|<span data-ttu-id="d73e3-120">G、すべての年代の参加を許可</span><span class="sxs-lookup"><span data-stu-id="d73e3-120">G, all ages admitted</span></span>|
|<span data-ttu-id="d73e3-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d73e3-121">parentalGuidance</span></span>|<span data-ttu-id="d73e3-122">3</span><span class="sxs-lookup"><span data-stu-id="d73e3-122">3</span></span>|<span data-ttu-id="d73e3-123">PG、可能性がありますだと内容が子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="d73e3-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="d73e3-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="d73e3-124">parentalGuidance13</span></span>|<span data-ttu-id="d73e3-125">4</span><span class="sxs-lookup"><span data-stu-id="d73e3-125">4</span></span>|<span data-ttu-id="d73e3-126">PG13、いくつかの材料があります 13 才未満の子供に適切です</span><span class="sxs-lookup"><span data-stu-id="d73e3-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="d73e3-127">制限</span><span class="sxs-lookup"><span data-stu-id="d73e3-127">restricted</span></span>|<span data-ttu-id="d73e3-128">5</span><span class="sxs-lookup"><span data-stu-id="d73e3-128">5</span></span>|<span data-ttu-id="d73e3-129">親または大人の同伴に付属する R、17 歳未満の閲覧者が必要な</span><span class="sxs-lookup"><span data-stu-id="d73e3-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="d73e3-130">大人</span><span class="sxs-lookup"><span data-stu-id="d73e3-130">adults</span></span>|<span data-ttu-id="d73e3-131">6</span><span class="sxs-lookup"><span data-stu-id="d73e3-131">6</span></span>|<span data-ttu-id="d73e3-132">NC17、成人のみ</span><span class="sxs-lookup"><span data-stu-id="d73e3-132">NC17, adults only</span></span>|





