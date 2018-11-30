---
title: ratingJapanMoviesType 列挙型
description: 映画の日本でのラベルの評価
ms.openlocfilehash: 1e58c7bbb54bc477ac725e2007f83a806f7152f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073228"
---
# <a name="ratingjapanmoviestype-enum-type"></a><span data-ttu-id="e8ea5-103">ratingJapanMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e8ea5-103">ratingJapanMoviesType enum type</span></span>

> <span data-ttu-id="e8ea5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8ea5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8ea5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8ea5-107">映画の日本でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="e8ea5-107">Movies rating labels in Japan</span></span>
## <a name="members"></a><span data-ttu-id="e8ea5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8ea5-108">Members</span></span>
|<span data-ttu-id="e8ea5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8ea5-109">Member</span></span>|<span data-ttu-id="e8ea5-110">値</span><span class="sxs-lookup"><span data-stu-id="e8ea5-110">Value</span></span>|<span data-ttu-id="e8ea5-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8ea5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ea5-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e8ea5-112">allAllowed</span></span>|<span data-ttu-id="e8ea5-113">0</span><span class="sxs-lookup"><span data-stu-id="e8ea5-113">0</span></span>|<span data-ttu-id="e8ea5-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="e8ea5-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e8ea5-115">allBlocked</span></span>|<span data-ttu-id="e8ea5-116">1</span><span class="sxs-lookup"><span data-stu-id="e8ea5-116">1</span></span>|<span data-ttu-id="e8ea5-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="e8ea5-118">全般</span><span class="sxs-lookup"><span data-stu-id="e8ea5-118">general</span></span>|<span data-ttu-id="e8ea5-119">2</span><span class="sxs-lookup"><span data-stu-id="e8ea5-119">2</span></span>|<span data-ttu-id="e8ea5-120">一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="e8ea5-120">Suitable for all ages</span></span>|
|<span data-ttu-id="e8ea5-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e8ea5-121">parentalGuidance</span></span>|<span data-ttu-id="e8ea5-122">3</span><span class="sxs-lookup"><span data-stu-id="e8ea5-122">3</span></span>|<span data-ttu-id="e8ea5-123">PG 12 分類若い人で 12 の保護者による制限を要求します。</span><span class="sxs-lookup"><span data-stu-id="e8ea5-123">The PG-12 classification requests parental guidance for young people under 12</span></span>|
|<span data-ttu-id="e8ea5-124">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="e8ea5-124">agesAbove15</span></span>|<span data-ttu-id="e8ea5-125">4</span><span class="sxs-lookup"><span data-stu-id="e8ea5-125">4</span></span>|<span data-ttu-id="e8ea5-126">R15 の各 + のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="e8ea5-126">The R15+ classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="e8ea5-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="e8ea5-127">agesAbove18</span></span>|<span data-ttu-id="e8ea5-128">5</span><span class="sxs-lookup"><span data-stu-id="e8ea5-128">5</span></span>|<span data-ttu-id="e8ea5-129">R18 + の分類は、18 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="e8ea5-129">The R18+ classification is suitable for viewers of 18 or older</span></span>|





