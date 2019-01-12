---
title: ratingUnitedKingdomMoviesType 列挙型
description: 映画は英国でのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b80ad9cfb9f1b2f449e9758699bd677150903332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962185"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="b1712-103">ratingUnitedKingdomMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b1712-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="b1712-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1712-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1712-105">映画は英国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="b1712-105">Movies rating labels in United Kingdom</span></span>
## <a name="members"></a><span data-ttu-id="b1712-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1712-106">Members</span></span>
|<span data-ttu-id="b1712-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1712-107">Member</span></span>|<span data-ttu-id="b1712-108">値</span><span class="sxs-lookup"><span data-stu-id="b1712-108">Value</span></span>|<span data-ttu-id="b1712-109">説明</span><span class="sxs-lookup"><span data-stu-id="b1712-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1712-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b1712-110">allAllowed</span></span>|<span data-ttu-id="b1712-111">0</span><span class="sxs-lookup"><span data-stu-id="b1712-111">0</span></span>|<span data-ttu-id="b1712-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="b1712-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="b1712-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b1712-113">allBlocked</span></span>|<span data-ttu-id="b1712-114">1</span><span class="sxs-lookup"><span data-stu-id="b1712-114">1</span></span>|<span data-ttu-id="b1712-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="b1712-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="b1712-116">全般</span><span class="sxs-lookup"><span data-stu-id="b1712-116">general</span></span>|<span data-ttu-id="b1712-117">2</span><span class="sxs-lookup"><span data-stu-id="b1712-117">2</span></span>|<span data-ttu-id="b1712-118">U のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="b1712-118">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="b1712-119">universalChildren</span><span class="sxs-lookup"><span data-stu-id="b1712-119">universalChildren</span></span>|<span data-ttu-id="b1712-120">3</span><span class="sxs-lookup"><span data-stu-id="b1712-120">3</span></span>|<span data-ttu-id="b1712-121">UC のクラス分けが前の学校の子、以前の規制ラベルに適しています。</span><span class="sxs-lookup"><span data-stu-id="b1712-121">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="b1712-122">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b1712-122">parentalGuidance</span></span>|<span data-ttu-id="b1712-123">4</span><span class="sxs-lookup"><span data-stu-id="b1712-123">4</span></span>|<span data-ttu-id="b1712-124">PG の分類が適切で完成度の高い</span><span class="sxs-lookup"><span data-stu-id="b1712-124">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="b1712-125">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="b1712-125">agesAbove12Video</span></span>|<span data-ttu-id="b1712-126">5</span><span class="sxs-lookup"><span data-stu-id="b1712-126">5</span></span>|<span data-ttu-id="b1712-127">12 年間、12、ビデオを適切なリリースします。</span><span class="sxs-lookup"><span data-stu-id="b1712-127">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="b1712-128">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="b1712-128">agesAbove12Cinema</span></span>|<span data-ttu-id="b1712-129">6</span><span class="sxs-lookup"><span data-stu-id="b1712-129">6</span></span>|<span data-ttu-id="b1712-130">12 a、映画のリリースが 12 年間、適切です</span><span class="sxs-lookup"><span data-stu-id="b1712-130">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="b1712-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="b1712-131">agesAbove15</span></span>|<span data-ttu-id="b1712-132">7</span><span class="sxs-lookup"><span data-stu-id="b1712-132">7</span></span>|<span data-ttu-id="b1712-133">15、15 年間にのみ適していると古い</span><span class="sxs-lookup"><span data-stu-id="b1712-133">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="b1712-134">大人</span><span class="sxs-lookup"><span data-stu-id="b1712-134">adults</span></span>|<span data-ttu-id="b1712-135">8</span><span class="sxs-lookup"><span data-stu-id="b1712-135">8</span></span>|<span data-ttu-id="b1712-136">大人にのみ適して</span><span class="sxs-lookup"><span data-stu-id="b1712-136">Suitable only for adults</span></span>|



