---
title: ratingUnitedStatesMoviesType 列挙型
description: 映画が米国でのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5aeb2279d2f8379a4adb17277adf0da278e1c7ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952238"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="6e8d4-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6e8d4-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="6e8d4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e8d4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e8d4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e8d4-107">映画が米国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="6e8d4-107">Movies rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="6e8d4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6e8d4-108">Members</span></span>
|<span data-ttu-id="6e8d4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6e8d4-109">Member</span></span>|<span data-ttu-id="6e8d4-110">値</span><span class="sxs-lookup"><span data-stu-id="6e8d4-110">Value</span></span>|<span data-ttu-id="6e8d4-111">説明</span><span class="sxs-lookup"><span data-stu-id="6e8d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e8d4-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="6e8d4-112">allAllowed</span></span>|<span data-ttu-id="6e8d4-113">0</span><span class="sxs-lookup"><span data-stu-id="6e8d4-113">0</span></span>|<span data-ttu-id="6e8d4-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="6e8d4-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="6e8d4-115">allBlocked</span></span>|<span data-ttu-id="6e8d4-116">1</span><span class="sxs-lookup"><span data-stu-id="6e8d4-116">1</span></span>|<span data-ttu-id="6e8d4-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="6e8d4-118">全般</span><span class="sxs-lookup"><span data-stu-id="6e8d4-118">general</span></span>|<span data-ttu-id="6e8d4-119">2</span><span class="sxs-lookup"><span data-stu-id="6e8d4-119">2</span></span>|<span data-ttu-id="6e8d4-120">G、すべての年代の参加を許可</span><span class="sxs-lookup"><span data-stu-id="6e8d4-120">G, all ages admitted</span></span>|
|<span data-ttu-id="6e8d4-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="6e8d4-121">parentalGuidance</span></span>|<span data-ttu-id="6e8d4-122">3</span><span class="sxs-lookup"><span data-stu-id="6e8d4-122">3</span></span>|<span data-ttu-id="6e8d4-123">PG、可能性がありますだと内容が子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="6e8d4-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="6e8d4-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="6e8d4-124">parentalGuidance13</span></span>|<span data-ttu-id="6e8d4-125">4</span><span class="sxs-lookup"><span data-stu-id="6e8d4-125">4</span></span>|<span data-ttu-id="6e8d4-126">PG13、いくつかの材料があります 13 才未満の子供に適切です</span><span class="sxs-lookup"><span data-stu-id="6e8d4-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="6e8d4-127">制限</span><span class="sxs-lookup"><span data-stu-id="6e8d4-127">restricted</span></span>|<span data-ttu-id="6e8d4-128">5</span><span class="sxs-lookup"><span data-stu-id="6e8d4-128">5</span></span>|<span data-ttu-id="6e8d4-129">親または大人の同伴に付属する R、17 歳未満の閲覧者が必要な</span><span class="sxs-lookup"><span data-stu-id="6e8d4-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="6e8d4-130">大人</span><span class="sxs-lookup"><span data-stu-id="6e8d4-130">adults</span></span>|<span data-ttu-id="6e8d4-131">6</span><span class="sxs-lookup"><span data-stu-id="6e8d4-131">6</span></span>|<span data-ttu-id="6e8d4-132">NC17、成人のみ</span><span class="sxs-lookup"><span data-stu-id="6e8d4-132">NC17, adults only</span></span>|





