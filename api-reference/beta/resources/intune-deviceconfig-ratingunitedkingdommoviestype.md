---
title: ratingUnitedKingdomMoviesType 列挙型
description: 映画は英国でのラベルの評価
ms.openlocfilehash: 6d41c5c7ae8da1f1f27e4d9df4bfe9eb3a850597
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073165"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="967db-103">ratingUnitedKingdomMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="967db-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="967db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="967db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="967db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="967db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="967db-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="967db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="967db-107">映画は英国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="967db-107">Movies rating labels in United Kingdom</span></span>
## <a name="members"></a><span data-ttu-id="967db-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="967db-108">Members</span></span>
|<span data-ttu-id="967db-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="967db-109">Member</span></span>|<span data-ttu-id="967db-110">値</span><span class="sxs-lookup"><span data-stu-id="967db-110">Value</span></span>|<span data-ttu-id="967db-111">説明</span><span class="sxs-lookup"><span data-stu-id="967db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="967db-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="967db-112">allAllowed</span></span>|<span data-ttu-id="967db-113">0</span><span class="sxs-lookup"><span data-stu-id="967db-113">0</span></span>|<span data-ttu-id="967db-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="967db-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="967db-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="967db-115">allBlocked</span></span>|<span data-ttu-id="967db-116">1</span><span class="sxs-lookup"><span data-stu-id="967db-116">1</span></span>|<span data-ttu-id="967db-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="967db-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="967db-118">全般</span><span class="sxs-lookup"><span data-stu-id="967db-118">general</span></span>|<span data-ttu-id="967db-119">2</span><span class="sxs-lookup"><span data-stu-id="967db-119">2</span></span>|<span data-ttu-id="967db-120">U のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="967db-120">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="967db-121">universalChildren</span><span class="sxs-lookup"><span data-stu-id="967db-121">universalChildren</span></span>|<span data-ttu-id="967db-122">3</span><span class="sxs-lookup"><span data-stu-id="967db-122">3</span></span>|<span data-ttu-id="967db-123">UC のクラス分けが前の学校の子、以前の規制ラベルに適しています。</span><span class="sxs-lookup"><span data-stu-id="967db-123">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="967db-124">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="967db-124">parentalGuidance</span></span>|<span data-ttu-id="967db-125">4</span><span class="sxs-lookup"><span data-stu-id="967db-125">4</span></span>|<span data-ttu-id="967db-126">PG の分類が適切で完成度の高い</span><span class="sxs-lookup"><span data-stu-id="967db-126">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="967db-127">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="967db-127">agesAbove12Video</span></span>|<span data-ttu-id="967db-128">5</span><span class="sxs-lookup"><span data-stu-id="967db-128">5</span></span>|<span data-ttu-id="967db-129">12 年間、12、ビデオを適切なリリースします。</span><span class="sxs-lookup"><span data-stu-id="967db-129">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="967db-130">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="967db-130">agesAbove12Cinema</span></span>|<span data-ttu-id="967db-131">6</span><span class="sxs-lookup"><span data-stu-id="967db-131">6</span></span>|<span data-ttu-id="967db-132">12 a、映画のリリースが 12 年間、適切です</span><span class="sxs-lookup"><span data-stu-id="967db-132">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="967db-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="967db-133">agesAbove15</span></span>|<span data-ttu-id="967db-134">7</span><span class="sxs-lookup"><span data-stu-id="967db-134">7</span></span>|<span data-ttu-id="967db-135">15、15 年間にのみ適していると古い</span><span class="sxs-lookup"><span data-stu-id="967db-135">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="967db-136">大人</span><span class="sxs-lookup"><span data-stu-id="967db-136">adults</span></span>|<span data-ttu-id="967db-137">8</span><span class="sxs-lookup"><span data-stu-id="967db-137">8</span></span>|<span data-ttu-id="967db-138">大人にのみ適して</span><span class="sxs-lookup"><span data-stu-id="967db-138">Suitable only for adults</span></span>|





