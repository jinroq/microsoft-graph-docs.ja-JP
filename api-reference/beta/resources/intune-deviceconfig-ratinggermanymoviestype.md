---
title: ratingGermanyMoviesType 列挙型
description: 映画のドイツのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 170dbf4614b34f8dacfa55f7d635146e06d56ea4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874691"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="42ed4-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="42ed4-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="42ed4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42ed4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42ed4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42ed4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42ed4-107">映画のドイツのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="42ed4-107">Movies rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="42ed4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="42ed4-108">Members</span></span>
|<span data-ttu-id="42ed4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="42ed4-109">Member</span></span>|<span data-ttu-id="42ed4-110">値</span><span class="sxs-lookup"><span data-stu-id="42ed4-110">Value</span></span>|<span data-ttu-id="42ed4-111">説明</span><span class="sxs-lookup"><span data-stu-id="42ed4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ed4-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="42ed4-112">allAllowed</span></span>|<span data-ttu-id="42ed4-113">0</span><span class="sxs-lookup"><span data-stu-id="42ed4-113">0</span></span>|<span data-ttu-id="42ed4-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="42ed4-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="42ed4-115">allBlocked</span></span>|<span data-ttu-id="42ed4-116">1</span><span class="sxs-lookup"><span data-stu-id="42ed4-116">1</span></span>|<span data-ttu-id="42ed4-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="42ed4-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="42ed4-118">全般</span><span class="sxs-lookup"><span data-stu-id="42ed4-118">general</span></span>|<span data-ttu-id="42ed4-119">2</span><span class="sxs-lookup"><span data-stu-id="42ed4-119">2</span></span>|<span data-ttu-id="42ed4-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="42ed4-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="42ed4-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="42ed4-121">agesAbove6</span></span>|<span data-ttu-id="42ed4-122">3</span><span class="sxs-lookup"><span data-stu-id="42ed4-122">3</span></span>|<span data-ttu-id="42ed4-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="42ed4-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="42ed4-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="42ed4-124">agesAbove12</span></span>|<span data-ttu-id="42ed4-125">4</span><span class="sxs-lookup"><span data-stu-id="42ed4-125">4</span></span>|<span data-ttu-id="42ed4-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="42ed4-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="42ed4-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="42ed4-127">agesAbove16</span></span>|<span data-ttu-id="42ed4-128">5</span><span class="sxs-lookup"><span data-stu-id="42ed4-128">5</span></span>|<span data-ttu-id="42ed4-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="42ed4-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="42ed4-130">大人</span><span class="sxs-lookup"><span data-stu-id="42ed4-130">adults</span></span>|<span data-ttu-id="42ed4-131">6</span><span class="sxs-lookup"><span data-stu-id="42ed4-131">6</span></span>|<span data-ttu-id="42ed4-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="42ed4-132">Ab 18 Jahren, adults only</span></span>|





