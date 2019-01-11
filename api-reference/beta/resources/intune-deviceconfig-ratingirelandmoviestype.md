---
title: ratingIrelandMoviesType 列挙型
description: アイルランドのラベルを規制ムービー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f5af5fb771821096eb006c0727ef8efb5e45136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880872"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="10a7d-103">ratingIrelandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="10a7d-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="10a7d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10a7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10a7d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10a7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10a7d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="10a7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10a7d-107">アイルランドのラベルを規制ムービー</span><span class="sxs-lookup"><span data-stu-id="10a7d-107">Movies rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="10a7d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="10a7d-108">Members</span></span>
|<span data-ttu-id="10a7d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="10a7d-109">Member</span></span>|<span data-ttu-id="10a7d-110">値</span><span class="sxs-lookup"><span data-stu-id="10a7d-110">Value</span></span>|<span data-ttu-id="10a7d-111">説明</span><span class="sxs-lookup"><span data-stu-id="10a7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a7d-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="10a7d-112">allAllowed</span></span>|<span data-ttu-id="10a7d-113">0</span><span class="sxs-lookup"><span data-stu-id="10a7d-113">0</span></span>|<span data-ttu-id="10a7d-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="10a7d-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="10a7d-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="10a7d-115">allBlocked</span></span>|<span data-ttu-id="10a7d-116">1</span><span class="sxs-lookup"><span data-stu-id="10a7d-116">1</span></span>|<span data-ttu-id="10a7d-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="10a7d-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="10a7d-118">全般</span><span class="sxs-lookup"><span data-stu-id="10a7d-118">general</span></span>|<span data-ttu-id="10a7d-119">2</span><span class="sxs-lookup"><span data-stu-id="10a7d-119">2</span></span>|<span data-ttu-id="10a7d-120">時代のこと、学校の子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="10a7d-120">Suitable for children of school going age</span></span>|
|<span data-ttu-id="10a7d-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="10a7d-121">parentalGuidance</span></span>|<span data-ttu-id="10a7d-122">3</span><span class="sxs-lookup"><span data-stu-id="10a7d-122">3</span></span>|<span data-ttu-id="10a7d-123">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="10a7d-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="10a7d-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="10a7d-124">agesAbove12</span></span>|<span data-ttu-id="10a7d-125">4</span><span class="sxs-lookup"><span data-stu-id="10a7d-125">4</span></span>|<span data-ttu-id="10a7d-126">12 a のクラス分けは、12 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="10a7d-126">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="10a7d-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="10a7d-127">agesAbove15</span></span>|<span data-ttu-id="10a7d-128">5</span><span class="sxs-lookup"><span data-stu-id="10a7d-128">5</span></span>|<span data-ttu-id="10a7d-129">15 a のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="10a7d-129">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="10a7d-130">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="10a7d-130">agesAbove16</span></span>|<span data-ttu-id="10a7d-131">6</span><span class="sxs-lookup"><span data-stu-id="10a7d-131">6</span></span>|<span data-ttu-id="10a7d-132">16 のクラス分けは、16 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="10a7d-132">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="10a7d-133">大人</span><span class="sxs-lookup"><span data-stu-id="10a7d-133">adults</span></span>|<span data-ttu-id="10a7d-134">7</span><span class="sxs-lookup"><span data-stu-id="10a7d-134">7</span></span>|<span data-ttu-id="10a7d-135">大人にのみ適しての 18 の分類</span><span class="sxs-lookup"><span data-stu-id="10a7d-135">The 18 classification, suitable only for adults</span></span>|





