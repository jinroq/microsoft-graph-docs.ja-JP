---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3db2989c7cc61eec2cbd736c336c222c23e9a5fe
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252967"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="cb2c0-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="cb2c0-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="cb2c0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb2c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb2c0-105">オーストラリアでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="cb2c0-105">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="cb2c0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="cb2c0-106">Members</span></span>
|<span data-ttu-id="cb2c0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cb2c0-107">Member</span></span>|<span data-ttu-id="cb2c0-108">値</span><span class="sxs-lookup"><span data-stu-id="cb2c0-108">Value</span></span>|<span data-ttu-id="cb2c0-109">説明</span><span class="sxs-lookup"><span data-stu-id="cb2c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb2c0-110">allallowed</span><span class="sxs-lookup"><span data-stu-id="cb2c0-110">allAllowed</span></span>|<span data-ttu-id="cb2c0-111">.0</span><span class="sxs-lookup"><span data-stu-id="cb2c0-111">0</span></span>|<span data-ttu-id="cb2c0-112">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="cb2c0-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="cb2c0-113">allblocked</span><span class="sxs-lookup"><span data-stu-id="cb2c0-113">allBlocked</span></span>|<span data-ttu-id="cb2c0-114">1-d</span><span class="sxs-lookup"><span data-stu-id="cb2c0-114">1</span></span>|<span data-ttu-id="cb2c0-115">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="cb2c0-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="cb2c0-116">prespreser</span><span class="sxs-lookup"><span data-stu-id="cb2c0-116">preschoolers</span></span>|<span data-ttu-id="cb2c0-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="cb2c0-117">2</span></span>|<span data-ttu-id="cb2c0-118">P 分類は、preschoolers に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="cb2c0-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="cb2c0-119">children</span><span class="sxs-lookup"><span data-stu-id="cb2c0-119">children</span></span>|<span data-ttu-id="cb2c0-120">1/3</span><span class="sxs-lookup"><span data-stu-id="cb2c0-120">3</span></span>|<span data-ttu-id="cb2c0-121">C の分類は、14の下の子を対象としています。</span><span class="sxs-lookup"><span data-stu-id="cb2c0-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="cb2c0-122">元帳</span><span class="sxs-lookup"><span data-stu-id="cb2c0-122">general</span></span>|<span data-ttu-id="cb2c0-123">2/4</span><span class="sxs-lookup"><span data-stu-id="cb2c0-123">4</span></span>|<span data-ttu-id="cb2c0-124">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="cb2c0-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="cb2c0-125">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="cb2c0-125">parentalGuidance</span></span>|<span data-ttu-id="cb2c0-126">5</span><span class="sxs-lookup"><span data-stu-id="cb2c0-126">5</span></span>|<span data-ttu-id="cb2c0-127">閲覧者には PG 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="cb2c0-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="cb2c0-128">度</span><span class="sxs-lookup"><span data-stu-id="cb2c0-128">mature</span></span>|<span data-ttu-id="cb2c0-129">シックス</span><span class="sxs-lookup"><span data-stu-id="cb2c0-129">6</span></span>|<span data-ttu-id="cb2c0-130">15を超える閲覧者には M 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="cb2c0-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="cb2c0-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="cb2c0-131">agesAbove15</span></span>|<span data-ttu-id="cb2c0-132">7</span><span class="sxs-lookup"><span data-stu-id="cb2c0-132">7</span></span>|<span data-ttu-id="cb2c0-133">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="cb2c0-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="cb2c0-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="cb2c0-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="cb2c0-135">~</span><span class="sxs-lookup"><span data-stu-id="cb2c0-135">8</span></span>|<span data-ttu-id="cb2c0-136">AV15 + 分類は、15の下の閲覧者には適していません。成人の暴力に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="cb2c0-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



