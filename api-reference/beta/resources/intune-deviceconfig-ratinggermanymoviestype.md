---
title: ratingGermanyMoviesType 列挙型
description: 映画のドイツのラベルの評価
author: tfitzmac
ms.openlocfilehash: 2dc78b1de99c193ab575b28ef3658ddd2b5f6df2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312342"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="8efd6-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8efd6-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="8efd6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8efd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8efd6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8efd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8efd6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8efd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8efd6-107">映画のドイツのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="8efd6-107">Movies rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="8efd6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8efd6-108">Members</span></span>
|<span data-ttu-id="8efd6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8efd6-109">Member</span></span>|<span data-ttu-id="8efd6-110">値</span><span class="sxs-lookup"><span data-stu-id="8efd6-110">Value</span></span>|<span data-ttu-id="8efd6-111">説明</span><span class="sxs-lookup"><span data-stu-id="8efd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8efd6-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="8efd6-112">allAllowed</span></span>|<span data-ttu-id="8efd6-113">0</span><span class="sxs-lookup"><span data-stu-id="8efd6-113">0</span></span>|<span data-ttu-id="8efd6-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="8efd6-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="8efd6-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="8efd6-115">allBlocked</span></span>|<span data-ttu-id="8efd6-116">1</span><span class="sxs-lookup"><span data-stu-id="8efd6-116">1</span></span>|<span data-ttu-id="8efd6-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="8efd6-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="8efd6-118">全般</span><span class="sxs-lookup"><span data-stu-id="8efd6-118">general</span></span>|<span data-ttu-id="8efd6-119">2</span><span class="sxs-lookup"><span data-stu-id="8efd6-119">2</span></span>|<span data-ttu-id="8efd6-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="8efd6-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="8efd6-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="8efd6-121">agesAbove6</span></span>|<span data-ttu-id="8efd6-122">3</span><span class="sxs-lookup"><span data-stu-id="8efd6-122">3</span></span>|<span data-ttu-id="8efd6-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="8efd6-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="8efd6-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="8efd6-124">agesAbove12</span></span>|<span data-ttu-id="8efd6-125">4</span><span class="sxs-lookup"><span data-stu-id="8efd6-125">4</span></span>|<span data-ttu-id="8efd6-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="8efd6-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="8efd6-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="8efd6-127">agesAbove16</span></span>|<span data-ttu-id="8efd6-128">5</span><span class="sxs-lookup"><span data-stu-id="8efd6-128">5</span></span>|<span data-ttu-id="8efd6-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="8efd6-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="8efd6-130">大人</span><span class="sxs-lookup"><span data-stu-id="8efd6-130">adults</span></span>|<span data-ttu-id="8efd6-131">6</span><span class="sxs-lookup"><span data-stu-id="8efd6-131">6</span></span>|<span data-ttu-id="8efd6-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="8efd6-132">Ab 18 Jahren, adults only</span></span>|





