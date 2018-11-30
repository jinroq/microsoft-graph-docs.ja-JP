---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアのテレビのコンテンツの規制ラベル
ms.openlocfilehash: 852d18b1cd7ae1486cf2826f0af169e4e89703d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021597"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="0d0ae-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0d0ae-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="0d0ae-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d0ae-105">オーストラリアのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="0d0ae-105">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="0d0ae-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d0ae-106">Members</span></span>
|<span data-ttu-id="0d0ae-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d0ae-107">Member</span></span>|<span data-ttu-id="0d0ae-108">値</span><span class="sxs-lookup"><span data-stu-id="0d0ae-108">Value</span></span>|<span data-ttu-id="0d0ae-109">説明</span><span class="sxs-lookup"><span data-stu-id="0d0ae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d0ae-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="0d0ae-110">allAllowed</span></span>|<span data-ttu-id="0d0ae-111">0</span><span class="sxs-lookup"><span data-stu-id="0d0ae-111">0</span></span>|<span data-ttu-id="0d0ae-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="0d0ae-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="0d0ae-113">allBlocked</span></span>|<span data-ttu-id="0d0ae-114">1</span><span class="sxs-lookup"><span data-stu-id="0d0ae-114">1</span></span>|<span data-ttu-id="0d0ae-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="0d0ae-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="0d0ae-116">preschoolers</span></span>|<span data-ttu-id="0d0ae-117">2</span><span class="sxs-lookup"><span data-stu-id="0d0ae-117">2</span></span>|<span data-ttu-id="0d0ae-118">P のクラス分けは、preschoolers</span><span class="sxs-lookup"><span data-stu-id="0d0ae-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="0d0ae-119">children</span><span class="sxs-lookup"><span data-stu-id="0d0ae-119">children</span></span>|<span data-ttu-id="0d0ae-120">3</span><span class="sxs-lookup"><span data-stu-id="0d0ae-120">3</span></span>|<span data-ttu-id="0d0ae-121">子で 14 C のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="0d0ae-122">全般</span><span class="sxs-lookup"><span data-stu-id="0d0ae-122">general</span></span>|<span data-ttu-id="0d0ae-123">4</span><span class="sxs-lookup"><span data-stu-id="0d0ae-123">4</span></span>|<span data-ttu-id="0d0ae-124">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="0d0ae-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="0d0ae-125">parentalGuidance</span></span>|<span data-ttu-id="0d0ae-126">5</span><span class="sxs-lookup"><span data-stu-id="0d0ae-126">5</span></span>|<span data-ttu-id="0d0ae-127">PG クラス分けが若い視聴者を推奨します。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="0d0ae-128">成熟</span><span class="sxs-lookup"><span data-stu-id="0d0ae-128">mature</span></span>|<span data-ttu-id="0d0ae-129">6</span><span class="sxs-lookup"><span data-stu-id="0d0ae-129">6</span></span>|<span data-ttu-id="0d0ae-130">ビューアー 15 以上の M クラス分けをお勧め</span><span class="sxs-lookup"><span data-stu-id="0d0ae-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="0d0ae-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="0d0ae-131">agesAbove15</span></span>|<span data-ttu-id="0d0ae-132">7</span><span class="sxs-lookup"><span data-stu-id="0d0ae-132">7</span></span>|<span data-ttu-id="0d0ae-133">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="0d0ae-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="0d0ae-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="0d0ae-135">8</span><span class="sxs-lookup"><span data-stu-id="0d0ae-135">8</span></span>|<span data-ttu-id="0d0ae-136">AV15 + 分類が 15、成人向け暴力に固有であるユーザーに適していません。</span><span class="sxs-lookup"><span data-stu-id="0d0ae-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



