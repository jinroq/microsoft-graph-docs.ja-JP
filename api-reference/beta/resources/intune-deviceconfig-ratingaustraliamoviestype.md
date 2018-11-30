---
title: ratingAustraliaMoviesType 列挙型
description: 映画のオーストラリアのラベルの評価
ms.openlocfilehash: 68eef0de18ad74c8fed76c4218bad0ae18a070f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072691"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="0d519-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0d519-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="0d519-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d519-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d519-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d519-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d519-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d519-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d519-107">映画のオーストラリアのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="0d519-107">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="0d519-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d519-108">Members</span></span>
|<span data-ttu-id="0d519-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d519-109">Member</span></span>|<span data-ttu-id="0d519-110">値</span><span class="sxs-lookup"><span data-stu-id="0d519-110">Value</span></span>|<span data-ttu-id="0d519-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d519-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d519-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="0d519-112">allAllowed</span></span>|<span data-ttu-id="0d519-113">0</span><span class="sxs-lookup"><span data-stu-id="0d519-113">0</span></span>|<span data-ttu-id="0d519-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="0d519-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="0d519-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="0d519-115">allBlocked</span></span>|<span data-ttu-id="0d519-116">1</span><span class="sxs-lookup"><span data-stu-id="0d519-116">1</span></span>|<span data-ttu-id="0d519-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="0d519-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="0d519-118">全般</span><span class="sxs-lookup"><span data-stu-id="0d519-118">general</span></span>|<span data-ttu-id="0d519-119">2</span><span class="sxs-lookup"><span data-stu-id="0d519-119">2</span></span>|<span data-ttu-id="0d519-120">G のクラス分けは、すべてのユーザーに対して適切です</span><span class="sxs-lookup"><span data-stu-id="0d519-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="0d519-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="0d519-121">parentalGuidance</span></span>|<span data-ttu-id="0d519-122">3</span><span class="sxs-lookup"><span data-stu-id="0d519-122">3</span></span>|<span data-ttu-id="0d519-123">PG が視聴者の親または保護者からのガイドに目をお勧め</span><span class="sxs-lookup"><span data-stu-id="0d519-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="0d519-124">成熟</span><span class="sxs-lookup"><span data-stu-id="0d519-124">mature</span></span>|<span data-ttu-id="0d519-125">4</span><span class="sxs-lookup"><span data-stu-id="0d519-125">4</span></span>|<span data-ttu-id="0d519-126">ビューアーで 15 M のクラス分けは推奨されません。</span><span class="sxs-lookup"><span data-stu-id="0d519-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="0d519-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="0d519-127">agesAbove15</span></span>|<span data-ttu-id="0d519-128">5</span><span class="sxs-lookup"><span data-stu-id="0d519-128">5</span></span>|<span data-ttu-id="0d519-129">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="0d519-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="0d519-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="0d519-130">agesAbove18</span></span>|<span data-ttu-id="0d519-131">6</span><span class="sxs-lookup"><span data-stu-id="0d519-131">6</span></span>|<span data-ttu-id="0d519-132">R18 + の分類は 18 才未満の閲覧者には適していません。</span><span class="sxs-lookup"><span data-stu-id="0d519-132">The R18+ classification is not suitable for viewers under 18</span></span>|





