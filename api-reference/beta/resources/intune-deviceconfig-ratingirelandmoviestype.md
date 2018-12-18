---
title: ratingIrelandMoviesType 列挙型
description: アイルランドのラベルを規制ムービー
author: tfitzmac
ms.openlocfilehash: ddda08358bf00c62ba4ac6aed12ae871f9db0579
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359515"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="7549e-103">ratingIrelandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7549e-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="7549e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7549e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7549e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7549e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7549e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7549e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7549e-107">アイルランドのラベルを規制ムービー</span><span class="sxs-lookup"><span data-stu-id="7549e-107">Movies rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="7549e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7549e-108">Members</span></span>
|<span data-ttu-id="7549e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7549e-109">Member</span></span>|<span data-ttu-id="7549e-110">値</span><span class="sxs-lookup"><span data-stu-id="7549e-110">Value</span></span>|<span data-ttu-id="7549e-111">説明</span><span class="sxs-lookup"><span data-stu-id="7549e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7549e-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="7549e-112">allAllowed</span></span>|<span data-ttu-id="7549e-113">0</span><span class="sxs-lookup"><span data-stu-id="7549e-113">0</span></span>|<span data-ttu-id="7549e-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="7549e-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="7549e-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="7549e-115">allBlocked</span></span>|<span data-ttu-id="7549e-116">1</span><span class="sxs-lookup"><span data-stu-id="7549e-116">1</span></span>|<span data-ttu-id="7549e-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="7549e-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="7549e-118">全般</span><span class="sxs-lookup"><span data-stu-id="7549e-118">general</span></span>|<span data-ttu-id="7549e-119">2</span><span class="sxs-lookup"><span data-stu-id="7549e-119">2</span></span>|<span data-ttu-id="7549e-120">時代のこと、学校の子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="7549e-120">Suitable for children of school going age</span></span>|
|<span data-ttu-id="7549e-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="7549e-121">parentalGuidance</span></span>|<span data-ttu-id="7549e-122">3</span><span class="sxs-lookup"><span data-stu-id="7549e-122">3</span></span>|<span data-ttu-id="7549e-123">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="7549e-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="7549e-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="7549e-124">agesAbove12</span></span>|<span data-ttu-id="7549e-125">4</span><span class="sxs-lookup"><span data-stu-id="7549e-125">4</span></span>|<span data-ttu-id="7549e-126">12 a のクラス分けは、12 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="7549e-126">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="7549e-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="7549e-127">agesAbove15</span></span>|<span data-ttu-id="7549e-128">5</span><span class="sxs-lookup"><span data-stu-id="7549e-128">5</span></span>|<span data-ttu-id="7549e-129">15 a のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="7549e-129">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="7549e-130">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="7549e-130">agesAbove16</span></span>|<span data-ttu-id="7549e-131">6</span><span class="sxs-lookup"><span data-stu-id="7549e-131">6</span></span>|<span data-ttu-id="7549e-132">16 のクラス分けは、16 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="7549e-132">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="7549e-133">大人</span><span class="sxs-lookup"><span data-stu-id="7549e-133">adults</span></span>|<span data-ttu-id="7549e-134">7</span><span class="sxs-lookup"><span data-stu-id="7549e-134">7</span></span>|<span data-ttu-id="7549e-135">大人にのみ適しての 18 の分類</span><span class="sxs-lookup"><span data-stu-id="7549e-135">The 18 classification, suitable only for adults</span></span>|





