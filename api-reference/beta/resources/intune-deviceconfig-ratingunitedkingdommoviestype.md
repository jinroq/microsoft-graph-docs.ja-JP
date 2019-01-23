---
title: ratingUnitedKingdomMoviesType 列挙型
description: 映画は英国でのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62194038006b011fdc8a70c4b399beef5e8c742b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412535"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="01858-103">ratingUnitedKingdomMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="01858-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="01858-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01858-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01858-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01858-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01858-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="01858-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01858-107">映画は英国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="01858-107">Movies rating labels in United Kingdom</span></span>

## <a name="members"></a><span data-ttu-id="01858-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="01858-108">Members</span></span>
|<span data-ttu-id="01858-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="01858-109">Member</span></span>|<span data-ttu-id="01858-110">値</span><span class="sxs-lookup"><span data-stu-id="01858-110">Value</span></span>|<span data-ttu-id="01858-111">説明</span><span class="sxs-lookup"><span data-stu-id="01858-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01858-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="01858-112">allAllowed</span></span>|<span data-ttu-id="01858-113">0</span><span class="sxs-lookup"><span data-stu-id="01858-113">0</span></span>|<span data-ttu-id="01858-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="01858-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="01858-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="01858-115">allBlocked</span></span>|<span data-ttu-id="01858-116">1</span><span class="sxs-lookup"><span data-stu-id="01858-116">1</span></span>|<span data-ttu-id="01858-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="01858-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="01858-118">全般</span><span class="sxs-lookup"><span data-stu-id="01858-118">general</span></span>|<span data-ttu-id="01858-119">2</span><span class="sxs-lookup"><span data-stu-id="01858-119">2</span></span>|<span data-ttu-id="01858-120">U のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="01858-120">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="01858-121">universalChildren</span><span class="sxs-lookup"><span data-stu-id="01858-121">universalChildren</span></span>|<span data-ttu-id="01858-122">3</span><span class="sxs-lookup"><span data-stu-id="01858-122">3</span></span>|<span data-ttu-id="01858-123">UC のクラス分けが前の学校の子、以前の規制ラベルに適しています。</span><span class="sxs-lookup"><span data-stu-id="01858-123">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="01858-124">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="01858-124">parentalGuidance</span></span>|<span data-ttu-id="01858-125">4</span><span class="sxs-lookup"><span data-stu-id="01858-125">4</span></span>|<span data-ttu-id="01858-126">PG の分類が適切で完成度の高い</span><span class="sxs-lookup"><span data-stu-id="01858-126">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="01858-127">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="01858-127">agesAbove12Video</span></span>|<span data-ttu-id="01858-128">5</span><span class="sxs-lookup"><span data-stu-id="01858-128">5</span></span>|<span data-ttu-id="01858-129">12 年間、12、ビデオを適切なリリースします。</span><span class="sxs-lookup"><span data-stu-id="01858-129">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="01858-130">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="01858-130">agesAbove12Cinema</span></span>|<span data-ttu-id="01858-131">6</span><span class="sxs-lookup"><span data-stu-id="01858-131">6</span></span>|<span data-ttu-id="01858-132">12 a、映画のリリースが 12 年間、適切です</span><span class="sxs-lookup"><span data-stu-id="01858-132">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="01858-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="01858-133">agesAbove15</span></span>|<span data-ttu-id="01858-134">7</span><span class="sxs-lookup"><span data-stu-id="01858-134">7</span></span>|<span data-ttu-id="01858-135">15、15 年間にのみ適していると古い</span><span class="sxs-lookup"><span data-stu-id="01858-135">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="01858-136">大人</span><span class="sxs-lookup"><span data-stu-id="01858-136">adults</span></span>|<span data-ttu-id="01858-137">8</span><span class="sxs-lookup"><span data-stu-id="01858-137">8</span></span>|<span data-ttu-id="01858-138">大人にのみ適して</span><span class="sxs-lookup"><span data-stu-id="01858-138">Suitable only for adults</span></span>|




