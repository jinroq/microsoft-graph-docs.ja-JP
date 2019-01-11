---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 176e1d863fd2aa94ea48a2bf8aab515228ac31ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844689"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="bccc3-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bccc3-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="bccc3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bccc3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bccc3-105">オーストラリアのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="bccc3-105">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="bccc3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="bccc3-106">Members</span></span>
|<span data-ttu-id="bccc3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bccc3-107">Member</span></span>|<span data-ttu-id="bccc3-108">値</span><span class="sxs-lookup"><span data-stu-id="bccc3-108">Value</span></span>|<span data-ttu-id="bccc3-109">説明</span><span class="sxs-lookup"><span data-stu-id="bccc3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bccc3-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="bccc3-110">allAllowed</span></span>|<span data-ttu-id="bccc3-111">0</span><span class="sxs-lookup"><span data-stu-id="bccc3-111">0</span></span>|<span data-ttu-id="bccc3-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="bccc3-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="bccc3-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="bccc3-113">allBlocked</span></span>|<span data-ttu-id="bccc3-114">1</span><span class="sxs-lookup"><span data-stu-id="bccc3-114">1</span></span>|<span data-ttu-id="bccc3-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="bccc3-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="bccc3-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="bccc3-116">preschoolers</span></span>|<span data-ttu-id="bccc3-117">2</span><span class="sxs-lookup"><span data-stu-id="bccc3-117">2</span></span>|<span data-ttu-id="bccc3-118">P のクラス分けは、preschoolers</span><span class="sxs-lookup"><span data-stu-id="bccc3-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="bccc3-119">children</span><span class="sxs-lookup"><span data-stu-id="bccc3-119">children</span></span>|<span data-ttu-id="bccc3-120">3</span><span class="sxs-lookup"><span data-stu-id="bccc3-120">3</span></span>|<span data-ttu-id="bccc3-121">子で 14 C のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="bccc3-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="bccc3-122">全般</span><span class="sxs-lookup"><span data-stu-id="bccc3-122">general</span></span>|<span data-ttu-id="bccc3-123">4</span><span class="sxs-lookup"><span data-stu-id="bccc3-123">4</span></span>|<span data-ttu-id="bccc3-124">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="bccc3-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="bccc3-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="bccc3-125">parentalGuidance</span></span>|<span data-ttu-id="bccc3-126">5</span><span class="sxs-lookup"><span data-stu-id="bccc3-126">5</span></span>|<span data-ttu-id="bccc3-127">PG クラス分けが若い視聴者を推奨します。</span><span class="sxs-lookup"><span data-stu-id="bccc3-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="bccc3-128">成熟</span><span class="sxs-lookup"><span data-stu-id="bccc3-128">mature</span></span>|<span data-ttu-id="bccc3-129">6</span><span class="sxs-lookup"><span data-stu-id="bccc3-129">6</span></span>|<span data-ttu-id="bccc3-130">ビューアー 15 以上の M クラス分けをお勧め</span><span class="sxs-lookup"><span data-stu-id="bccc3-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="bccc3-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="bccc3-131">agesAbove15</span></span>|<span data-ttu-id="bccc3-132">7</span><span class="sxs-lookup"><span data-stu-id="bccc3-132">7</span></span>|<span data-ttu-id="bccc3-133">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="bccc3-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="bccc3-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="bccc3-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="bccc3-135">8</span><span class="sxs-lookup"><span data-stu-id="bccc3-135">8</span></span>|<span data-ttu-id="bccc3-136">AV15 + 分類が 15、成人向け暴力に固有であるユーザーに適していません。</span><span class="sxs-lookup"><span data-stu-id="bccc3-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



