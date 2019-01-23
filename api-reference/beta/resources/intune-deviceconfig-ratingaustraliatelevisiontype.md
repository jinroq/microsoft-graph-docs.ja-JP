---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアのテレビのコンテンツの規制ラベル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 148e8c1bb12f8563261402b98e4ff0552e83f3f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392893"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="e3d90-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3d90-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="e3d90-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3d90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3d90-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3d90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3d90-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3d90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3d90-107">オーストラリアのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="e3d90-107">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="e3d90-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3d90-108">Members</span></span>
|<span data-ttu-id="e3d90-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3d90-109">Member</span></span>|<span data-ttu-id="e3d90-110">値</span><span class="sxs-lookup"><span data-stu-id="e3d90-110">Value</span></span>|<span data-ttu-id="e3d90-111">説明</span><span class="sxs-lookup"><span data-stu-id="e3d90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d90-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e3d90-112">allAllowed</span></span>|<span data-ttu-id="e3d90-113">0</span><span class="sxs-lookup"><span data-stu-id="e3d90-113">0</span></span>|<span data-ttu-id="e3d90-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="e3d90-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="e3d90-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e3d90-115">allBlocked</span></span>|<span data-ttu-id="e3d90-116">1</span><span class="sxs-lookup"><span data-stu-id="e3d90-116">1</span></span>|<span data-ttu-id="e3d90-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="e3d90-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="e3d90-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="e3d90-118">preschoolers</span></span>|<span data-ttu-id="e3d90-119">2</span><span class="sxs-lookup"><span data-stu-id="e3d90-119">2</span></span>|<span data-ttu-id="e3d90-120">P のクラス分けは、preschoolers</span><span class="sxs-lookup"><span data-stu-id="e3d90-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="e3d90-121">children</span><span class="sxs-lookup"><span data-stu-id="e3d90-121">children</span></span>|<span data-ttu-id="e3d90-122">3</span><span class="sxs-lookup"><span data-stu-id="e3d90-122">3</span></span>|<span data-ttu-id="e3d90-123">子で 14 C のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="e3d90-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="e3d90-124">全般</span><span class="sxs-lookup"><span data-stu-id="e3d90-124">general</span></span>|<span data-ttu-id="e3d90-125">4</span><span class="sxs-lookup"><span data-stu-id="e3d90-125">4</span></span>|<span data-ttu-id="e3d90-126">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="e3d90-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="e3d90-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e3d90-127">parentalGuidance</span></span>|<span data-ttu-id="e3d90-128">5</span><span class="sxs-lookup"><span data-stu-id="e3d90-128">5</span></span>|<span data-ttu-id="e3d90-129">PG クラス分けが若い視聴者を推奨します。</span><span class="sxs-lookup"><span data-stu-id="e3d90-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="e3d90-130">成熟</span><span class="sxs-lookup"><span data-stu-id="e3d90-130">mature</span></span>|<span data-ttu-id="e3d90-131">6</span><span class="sxs-lookup"><span data-stu-id="e3d90-131">6</span></span>|<span data-ttu-id="e3d90-132">ビューアー 15 以上の M クラス分けをお勧め</span><span class="sxs-lookup"><span data-stu-id="e3d90-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="e3d90-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="e3d90-133">agesAbove15</span></span>|<span data-ttu-id="e3d90-134">7</span><span class="sxs-lookup"><span data-stu-id="e3d90-134">7</span></span>|<span data-ttu-id="e3d90-135">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="e3d90-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="e3d90-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="e3d90-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="e3d90-137">8</span><span class="sxs-lookup"><span data-stu-id="e3d90-137">8</span></span>|<span data-ttu-id="e3d90-138">AV15 + 分類が 15、成人向け暴力に固有であるユーザーに適していません。</span><span class="sxs-lookup"><span data-stu-id="e3d90-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|




