---
title: ratingGermanyMoviesType 列挙型
description: 映画のドイツのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8806461969b5bea7957d5be75722181654de9097
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922005"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="00327-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="00327-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="00327-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00327-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00327-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00327-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00327-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00327-107">映画のドイツのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="00327-107">Movies rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="00327-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="00327-108">Members</span></span>
|<span data-ttu-id="00327-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="00327-109">Member</span></span>|<span data-ttu-id="00327-110">値</span><span class="sxs-lookup"><span data-stu-id="00327-110">Value</span></span>|<span data-ttu-id="00327-111">説明</span><span class="sxs-lookup"><span data-stu-id="00327-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00327-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="00327-112">allAllowed</span></span>|<span data-ttu-id="00327-113">0</span><span class="sxs-lookup"><span data-stu-id="00327-113">0</span></span>|<span data-ttu-id="00327-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="00327-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="00327-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="00327-115">allBlocked</span></span>|<span data-ttu-id="00327-116">1</span><span class="sxs-lookup"><span data-stu-id="00327-116">1</span></span>|<span data-ttu-id="00327-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="00327-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="00327-118">全般</span><span class="sxs-lookup"><span data-stu-id="00327-118">general</span></span>|<span data-ttu-id="00327-119">2</span><span class="sxs-lookup"><span data-stu-id="00327-119">2</span></span>|<span data-ttu-id="00327-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="00327-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="00327-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="00327-121">agesAbove6</span></span>|<span data-ttu-id="00327-122">3</span><span class="sxs-lookup"><span data-stu-id="00327-122">3</span></span>|<span data-ttu-id="00327-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="00327-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="00327-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="00327-124">agesAbove12</span></span>|<span data-ttu-id="00327-125">4</span><span class="sxs-lookup"><span data-stu-id="00327-125">4</span></span>|<span data-ttu-id="00327-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="00327-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="00327-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="00327-127">agesAbove16</span></span>|<span data-ttu-id="00327-128">5</span><span class="sxs-lookup"><span data-stu-id="00327-128">5</span></span>|<span data-ttu-id="00327-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="00327-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="00327-130">大人</span><span class="sxs-lookup"><span data-stu-id="00327-130">adults</span></span>|<span data-ttu-id="00327-131">6</span><span class="sxs-lookup"><span data-stu-id="00327-131">6</span></span>|<span data-ttu-id="00327-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="00327-132">Ab 18 Jahren, adults only</span></span>|





