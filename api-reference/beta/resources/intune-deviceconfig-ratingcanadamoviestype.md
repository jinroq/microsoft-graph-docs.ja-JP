---
title: ratingCanadaMoviesType 列挙型
description: 映画がカナダでのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 469bbf1b177df8bdf40dcdfea4ef6b0c4721cd3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918477"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="34c64-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="34c64-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="34c64-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34c64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34c64-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34c64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34c64-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="34c64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34c64-107">映画がカナダでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="34c64-107">Movies rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="34c64-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="34c64-108">Members</span></span>
|<span data-ttu-id="34c64-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="34c64-109">Member</span></span>|<span data-ttu-id="34c64-110">値</span><span class="sxs-lookup"><span data-stu-id="34c64-110">Value</span></span>|<span data-ttu-id="34c64-111">説明</span><span class="sxs-lookup"><span data-stu-id="34c64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c64-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="34c64-112">allAllowed</span></span>|<span data-ttu-id="34c64-113">0</span><span class="sxs-lookup"><span data-stu-id="34c64-113">0</span></span>|<span data-ttu-id="34c64-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="34c64-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="34c64-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="34c64-115">allBlocked</span></span>|<span data-ttu-id="34c64-116">1</span><span class="sxs-lookup"><span data-stu-id="34c64-116">1</span></span>|<span data-ttu-id="34c64-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="34c64-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="34c64-118">全般</span><span class="sxs-lookup"><span data-stu-id="34c64-118">general</span></span>|<span data-ttu-id="34c64-119">2</span><span class="sxs-lookup"><span data-stu-id="34c64-119">2</span></span>|<span data-ttu-id="34c64-120">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="34c64-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="34c64-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="34c64-121">parentalGuidance</span></span>|<span data-ttu-id="34c64-122">3</span><span class="sxs-lookup"><span data-stu-id="34c64-122">3</span></span>|<span data-ttu-id="34c64-123">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="34c64-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="34c64-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="34c64-124">agesAbove14</span></span>|<span data-ttu-id="34c64-125">4</span><span class="sxs-lookup"><span data-stu-id="34c64-125">4</span></span>|<span data-ttu-id="34c64-126">14A 分類が 14 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="34c64-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="34c64-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="34c64-127">agesAbove18</span></span>|<span data-ttu-id="34c64-128">5</span><span class="sxs-lookup"><span data-stu-id="34c64-128">5</span></span>|<span data-ttu-id="34c64-129">18A 分類が 18 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="34c64-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="34c64-130">制限</span><span class="sxs-lookup"><span data-stu-id="34c64-130">restricted</span></span>|<span data-ttu-id="34c64-131">6</span><span class="sxs-lookup"><span data-stu-id="34c64-131">6</span></span>|<span data-ttu-id="34c64-132">R のクラス分けは、18 年間に限定され、古い</span><span class="sxs-lookup"><span data-stu-id="34c64-132">The R classification is restricted to 18 years and older</span></span>|





