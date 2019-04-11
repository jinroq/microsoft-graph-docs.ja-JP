---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a65d8b272e99a3a8432214b3ac51916bc6e9f50
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784050"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="af92b-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="af92b-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="af92b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af92b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af92b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af92b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af92b-106">オーストラリアでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="af92b-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="af92b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="af92b-107">Members</span></span>
|<span data-ttu-id="af92b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="af92b-108">Member</span></span>|<span data-ttu-id="af92b-109">値</span><span class="sxs-lookup"><span data-stu-id="af92b-109">Value</span></span>|<span data-ttu-id="af92b-110">説明</span><span class="sxs-lookup"><span data-stu-id="af92b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af92b-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="af92b-111">allAllowed</span></span>|<span data-ttu-id="af92b-112">.0</span><span class="sxs-lookup"><span data-stu-id="af92b-112">0</span></span>|<span data-ttu-id="af92b-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="af92b-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="af92b-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="af92b-114">allBlocked</span></span>|<span data-ttu-id="af92b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="af92b-115">1</span></span>|<span data-ttu-id="af92b-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="af92b-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="af92b-117">prespreser</span><span class="sxs-lookup"><span data-stu-id="af92b-117">preschoolers</span></span>|<span data-ttu-id="af92b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="af92b-118">2</span></span>|<span data-ttu-id="af92b-119">P 分類は、preschoolers に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="af92b-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="af92b-120">children</span><span class="sxs-lookup"><span data-stu-id="af92b-120">children</span></span>|<span data-ttu-id="af92b-121">1/3</span><span class="sxs-lookup"><span data-stu-id="af92b-121">3</span></span>|<span data-ttu-id="af92b-122">C の分類は、14の下の子を対象としています。</span><span class="sxs-lookup"><span data-stu-id="af92b-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="af92b-123">元帳</span><span class="sxs-lookup"><span data-stu-id="af92b-123">general</span></span>|<span data-ttu-id="af92b-124">2/4</span><span class="sxs-lookup"><span data-stu-id="af92b-124">4</span></span>|<span data-ttu-id="af92b-125">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="af92b-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="af92b-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="af92b-126">parentalGuidance</span></span>|<span data-ttu-id="af92b-127">5</span><span class="sxs-lookup"><span data-stu-id="af92b-127">5</span></span>|<span data-ttu-id="af92b-128">閲覧者には PG 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="af92b-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="af92b-129">度</span><span class="sxs-lookup"><span data-stu-id="af92b-129">mature</span></span>|<span data-ttu-id="af92b-130">シックス</span><span class="sxs-lookup"><span data-stu-id="af92b-130">6</span></span>|<span data-ttu-id="af92b-131">15を超える閲覧者には M 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="af92b-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="af92b-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="af92b-132">agesAbove15</span></span>|<span data-ttu-id="af92b-133">7</span><span class="sxs-lookup"><span data-stu-id="af92b-133">7</span></span>|<span data-ttu-id="af92b-134">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="af92b-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="af92b-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="af92b-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="af92b-136">~</span><span class="sxs-lookup"><span data-stu-id="af92b-136">8</span></span>|<span data-ttu-id="af92b-137">AV15 + 分類は、15の下の閲覧者には適していません。成人の暴力に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="af92b-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





