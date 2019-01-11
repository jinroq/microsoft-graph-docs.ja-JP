---
title: ratingCanadaMoviesType 列挙型
description: 映画がカナダでのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c9443a673ab9e97ef6cb4967018f35bcb8b3b932
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826489"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="ee86c-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ee86c-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="ee86c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee86c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee86c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee86c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee86c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee86c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee86c-107">映画がカナダでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="ee86c-107">Movies rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="ee86c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee86c-108">Members</span></span>
|<span data-ttu-id="ee86c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee86c-109">Member</span></span>|<span data-ttu-id="ee86c-110">値</span><span class="sxs-lookup"><span data-stu-id="ee86c-110">Value</span></span>|<span data-ttu-id="ee86c-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee86c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee86c-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ee86c-112">allAllowed</span></span>|<span data-ttu-id="ee86c-113">0</span><span class="sxs-lookup"><span data-stu-id="ee86c-113">0</span></span>|<span data-ttu-id="ee86c-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="ee86c-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="ee86c-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ee86c-115">allBlocked</span></span>|<span data-ttu-id="ee86c-116">1</span><span class="sxs-lookup"><span data-stu-id="ee86c-116">1</span></span>|<span data-ttu-id="ee86c-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="ee86c-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="ee86c-118">全般</span><span class="sxs-lookup"><span data-stu-id="ee86c-118">general</span></span>|<span data-ttu-id="ee86c-119">2</span><span class="sxs-lookup"><span data-stu-id="ee86c-119">2</span></span>|<span data-ttu-id="ee86c-120">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="ee86c-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="ee86c-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="ee86c-121">parentalGuidance</span></span>|<span data-ttu-id="ee86c-122">3</span><span class="sxs-lookup"><span data-stu-id="ee86c-122">3</span></span>|<span data-ttu-id="ee86c-123">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="ee86c-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="ee86c-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="ee86c-124">agesAbove14</span></span>|<span data-ttu-id="ee86c-125">4</span><span class="sxs-lookup"><span data-stu-id="ee86c-125">4</span></span>|<span data-ttu-id="ee86c-126">14A 分類が 14 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="ee86c-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="ee86c-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="ee86c-127">agesAbove18</span></span>|<span data-ttu-id="ee86c-128">5</span><span class="sxs-lookup"><span data-stu-id="ee86c-128">5</span></span>|<span data-ttu-id="ee86c-129">18A 分類が 18 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="ee86c-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="ee86c-130">制限</span><span class="sxs-lookup"><span data-stu-id="ee86c-130">restricted</span></span>|<span data-ttu-id="ee86c-131">6</span><span class="sxs-lookup"><span data-stu-id="ee86c-131">6</span></span>|<span data-ttu-id="ee86c-132">R のクラス分けは、18 年間に限定され、古い</span><span class="sxs-lookup"><span data-stu-id="ee86c-132">The R classification is restricted to 18 years and older</span></span>|





