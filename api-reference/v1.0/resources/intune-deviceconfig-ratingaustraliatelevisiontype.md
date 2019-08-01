---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 04e58fd72f4b09ebd914f0dc69049e21c7f676a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027966"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="e136f-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e136f-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="e136f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e136f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e136f-105">オーストラリアでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="e136f-105">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="e136f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e136f-106">Members</span></span>
|<span data-ttu-id="e136f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e136f-107">Member</span></span>|<span data-ttu-id="e136f-108">値</span><span class="sxs-lookup"><span data-stu-id="e136f-108">Value</span></span>|<span data-ttu-id="e136f-109">説明</span><span class="sxs-lookup"><span data-stu-id="e136f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e136f-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e136f-110">allAllowed</span></span>|<span data-ttu-id="e136f-111">.0</span><span class="sxs-lookup"><span data-stu-id="e136f-111">0</span></span>|<span data-ttu-id="e136f-112">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="e136f-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="e136f-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e136f-113">allBlocked</span></span>|<span data-ttu-id="e136f-114">1-d</span><span class="sxs-lookup"><span data-stu-id="e136f-114">1</span></span>|<span data-ttu-id="e136f-115">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="e136f-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="e136f-116">prespreser</span><span class="sxs-lookup"><span data-stu-id="e136f-116">preschoolers</span></span>|<span data-ttu-id="e136f-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e136f-117">2</span></span>|<span data-ttu-id="e136f-118">P 分類は、preschoolers に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="e136f-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="e136f-119">children</span><span class="sxs-lookup"><span data-stu-id="e136f-119">children</span></span>|<span data-ttu-id="e136f-120">1/3</span><span class="sxs-lookup"><span data-stu-id="e136f-120">3</span></span>|<span data-ttu-id="e136f-121">C の分類は、14の下の子を対象としています。</span><span class="sxs-lookup"><span data-stu-id="e136f-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="e136f-122">元帳</span><span class="sxs-lookup"><span data-stu-id="e136f-122">general</span></span>|<span data-ttu-id="e136f-123">2/4</span><span class="sxs-lookup"><span data-stu-id="e136f-123">4</span></span>|<span data-ttu-id="e136f-124">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="e136f-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="e136f-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e136f-125">parentalGuidance</span></span>|<span data-ttu-id="e136f-126">5</span><span class="sxs-lookup"><span data-stu-id="e136f-126">5</span></span>|<span data-ttu-id="e136f-127">閲覧者には PG 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="e136f-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="e136f-128">度</span><span class="sxs-lookup"><span data-stu-id="e136f-128">mature</span></span>|<span data-ttu-id="e136f-129">シックス</span><span class="sxs-lookup"><span data-stu-id="e136f-129">6</span></span>|<span data-ttu-id="e136f-130">15を超える閲覧者には M 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="e136f-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="e136f-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="e136f-131">agesAbove15</span></span>|<span data-ttu-id="e136f-132">7</span><span class="sxs-lookup"><span data-stu-id="e136f-132">7</span></span>|<span data-ttu-id="e136f-133">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="e136f-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="e136f-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="e136f-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="e136f-135">8 </span><span class="sxs-lookup"><span data-stu-id="e136f-135">8</span></span>|<span data-ttu-id="e136f-136">AV15 + 分類は、15の下の閲覧者には適していません。成人の暴力に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="e136f-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



