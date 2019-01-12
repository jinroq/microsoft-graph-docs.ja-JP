---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5af818245d4b71a038cdfa0cd3a4f3c188e76e60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911974"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="499ee-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="499ee-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="499ee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="499ee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="499ee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="499ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="499ee-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="499ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="499ee-107">オーストラリアのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="499ee-107">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="499ee-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="499ee-108">Members</span></span>
|<span data-ttu-id="499ee-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="499ee-109">Member</span></span>|<span data-ttu-id="499ee-110">値</span><span class="sxs-lookup"><span data-stu-id="499ee-110">Value</span></span>|<span data-ttu-id="499ee-111">説明</span><span class="sxs-lookup"><span data-stu-id="499ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499ee-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="499ee-112">allAllowed</span></span>|<span data-ttu-id="499ee-113">0</span><span class="sxs-lookup"><span data-stu-id="499ee-113">0</span></span>|<span data-ttu-id="499ee-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="499ee-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="499ee-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="499ee-115">allBlocked</span></span>|<span data-ttu-id="499ee-116">1</span><span class="sxs-lookup"><span data-stu-id="499ee-116">1</span></span>|<span data-ttu-id="499ee-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="499ee-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="499ee-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="499ee-118">preschoolers</span></span>|<span data-ttu-id="499ee-119">2</span><span class="sxs-lookup"><span data-stu-id="499ee-119">2</span></span>|<span data-ttu-id="499ee-120">P のクラス分けは、preschoolers</span><span class="sxs-lookup"><span data-stu-id="499ee-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="499ee-121">children</span><span class="sxs-lookup"><span data-stu-id="499ee-121">children</span></span>|<span data-ttu-id="499ee-122">3</span><span class="sxs-lookup"><span data-stu-id="499ee-122">3</span></span>|<span data-ttu-id="499ee-123">子で 14 C のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="499ee-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="499ee-124">全般</span><span class="sxs-lookup"><span data-stu-id="499ee-124">general</span></span>|<span data-ttu-id="499ee-125">4</span><span class="sxs-lookup"><span data-stu-id="499ee-125">4</span></span>|<span data-ttu-id="499ee-126">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="499ee-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="499ee-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="499ee-127">parentalGuidance</span></span>|<span data-ttu-id="499ee-128">5</span><span class="sxs-lookup"><span data-stu-id="499ee-128">5</span></span>|<span data-ttu-id="499ee-129">PG クラス分けが若い視聴者を推奨します。</span><span class="sxs-lookup"><span data-stu-id="499ee-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="499ee-130">成熟</span><span class="sxs-lookup"><span data-stu-id="499ee-130">mature</span></span>|<span data-ttu-id="499ee-131">6</span><span class="sxs-lookup"><span data-stu-id="499ee-131">6</span></span>|<span data-ttu-id="499ee-132">ビューアー 15 以上の M クラス分けをお勧め</span><span class="sxs-lookup"><span data-stu-id="499ee-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="499ee-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="499ee-133">agesAbove15</span></span>|<span data-ttu-id="499ee-134">7</span><span class="sxs-lookup"><span data-stu-id="499ee-134">7</span></span>|<span data-ttu-id="499ee-135">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="499ee-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="499ee-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="499ee-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="499ee-137">8</span><span class="sxs-lookup"><span data-stu-id="499ee-137">8</span></span>|<span data-ttu-id="499ee-138">AV15 + 分類が 15、成人向け暴力に固有であるユーザーに適していません。</span><span class="sxs-lookup"><span data-stu-id="499ee-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





