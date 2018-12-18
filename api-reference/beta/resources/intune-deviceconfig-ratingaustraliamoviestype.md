---
title: ratingAustraliaMoviesType 列挙型
description: 映画のオーストラリアのラベルの評価
author: tfitzmac
ms.openlocfilehash: d282b4c0e58fb0fb5141068d3d59a10052c83490
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307099"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="25bc4-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="25bc4-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="25bc4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25bc4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25bc4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25bc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25bc4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25bc4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25bc4-107">映画のオーストラリアのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="25bc4-107">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="25bc4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="25bc4-108">Members</span></span>
|<span data-ttu-id="25bc4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="25bc4-109">Member</span></span>|<span data-ttu-id="25bc4-110">値</span><span class="sxs-lookup"><span data-stu-id="25bc4-110">Value</span></span>|<span data-ttu-id="25bc4-111">説明</span><span class="sxs-lookup"><span data-stu-id="25bc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25bc4-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="25bc4-112">allAllowed</span></span>|<span data-ttu-id="25bc4-113">0</span><span class="sxs-lookup"><span data-stu-id="25bc4-113">0</span></span>|<span data-ttu-id="25bc4-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="25bc4-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="25bc4-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="25bc4-115">allBlocked</span></span>|<span data-ttu-id="25bc4-116">1</span><span class="sxs-lookup"><span data-stu-id="25bc4-116">1</span></span>|<span data-ttu-id="25bc4-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="25bc4-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="25bc4-118">全般</span><span class="sxs-lookup"><span data-stu-id="25bc4-118">general</span></span>|<span data-ttu-id="25bc4-119">2</span><span class="sxs-lookup"><span data-stu-id="25bc4-119">2</span></span>|<span data-ttu-id="25bc4-120">G のクラス分けは、すべてのユーザーに対して適切です</span><span class="sxs-lookup"><span data-stu-id="25bc4-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="25bc4-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="25bc4-121">parentalGuidance</span></span>|<span data-ttu-id="25bc4-122">3</span><span class="sxs-lookup"><span data-stu-id="25bc4-122">3</span></span>|<span data-ttu-id="25bc4-123">PG が視聴者の親または保護者からのガイドに目をお勧め</span><span class="sxs-lookup"><span data-stu-id="25bc4-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="25bc4-124">成熟</span><span class="sxs-lookup"><span data-stu-id="25bc4-124">mature</span></span>|<span data-ttu-id="25bc4-125">4</span><span class="sxs-lookup"><span data-stu-id="25bc4-125">4</span></span>|<span data-ttu-id="25bc4-126">ビューアーで 15 M のクラス分けは推奨されません。</span><span class="sxs-lookup"><span data-stu-id="25bc4-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="25bc4-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="25bc4-127">agesAbove15</span></span>|<span data-ttu-id="25bc4-128">5</span><span class="sxs-lookup"><span data-stu-id="25bc4-128">5</span></span>|<span data-ttu-id="25bc4-129">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="25bc4-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="25bc4-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="25bc4-130">agesAbove18</span></span>|<span data-ttu-id="25bc4-131">6</span><span class="sxs-lookup"><span data-stu-id="25bc4-131">6</span></span>|<span data-ttu-id="25bc4-132">R18 + の分類は 18 才未満の閲覧者には適していません。</span><span class="sxs-lookup"><span data-stu-id="25bc4-132">The R18+ classification is not suitable for viewers under 18</span></span>|





