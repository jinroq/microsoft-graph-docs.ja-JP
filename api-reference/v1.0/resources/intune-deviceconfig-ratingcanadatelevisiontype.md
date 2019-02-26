---
title: ratingCanadaTelevisionType 列挙型
description: カナダでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2f8f8815df519f5107360924cfa8532856db77f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263484"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="2a22f-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2a22f-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="2a22f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a22f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a22f-105">カナダでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="2a22f-105">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="2a22f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2a22f-106">Members</span></span>
|<span data-ttu-id="2a22f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2a22f-107">Member</span></span>|<span data-ttu-id="2a22f-108">値</span><span class="sxs-lookup"><span data-stu-id="2a22f-108">Value</span></span>|<span data-ttu-id="2a22f-109">説明</span><span class="sxs-lookup"><span data-stu-id="2a22f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a22f-110">allallowed</span><span class="sxs-lookup"><span data-stu-id="2a22f-110">allAllowed</span></span>|<span data-ttu-id="2a22f-111">.0</span><span class="sxs-lookup"><span data-stu-id="2a22f-111">0</span></span>|<span data-ttu-id="2a22f-112">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="2a22f-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="2a22f-113">allblocked</span><span class="sxs-lookup"><span data-stu-id="2a22f-113">allBlocked</span></span>|<span data-ttu-id="2a22f-114">1-d</span><span class="sxs-lookup"><span data-stu-id="2a22f-114">1</span></span>|<span data-ttu-id="2a22f-115">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="2a22f-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="2a22f-116">children</span><span class="sxs-lookup"><span data-stu-id="2a22f-116">children</span></span>|<span data-ttu-id="2a22f-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="2a22f-117">2</span></span>|<span data-ttu-id="2a22f-118">C の分類は、2 ~ 7 年の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="2a22f-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="2a22f-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="2a22f-119">childrenAbove8</span></span>|<span data-ttu-id="2a22f-120">1/3</span><span class="sxs-lookup"><span data-stu-id="2a22f-120">3</span></span>|<span data-ttu-id="2a22f-121">C8 の分類は、8才を超える子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="2a22f-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="2a22f-122">元帳</span><span class="sxs-lookup"><span data-stu-id="2a22f-122">general</span></span>|<span data-ttu-id="2a22f-123">2/4</span><span class="sxs-lookup"><span data-stu-id="2a22f-123">4</span></span>|<span data-ttu-id="2a22f-124">G 分類は、一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="2a22f-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="2a22f-125">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="2a22f-125">parentalGuidance</span></span>|<span data-ttu-id="2a22f-126">5</span><span class="sxs-lookup"><span data-stu-id="2a22f-126">5</span></span>|<span data-ttu-id="2a22f-127">PG、キッズのガイダンス</span><span class="sxs-lookup"><span data-stu-id="2a22f-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="2a22f-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="2a22f-128">agesAbove14</span></span>|<span data-ttu-id="2a22f-129">シックス</span><span class="sxs-lookup"><span data-stu-id="2a22f-129">6</span></span>|<span data-ttu-id="2a22f-130">14以上の分類は、14才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="2a22f-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="2a22f-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="2a22f-131">agesAbove18</span></span>|<span data-ttu-id="2a22f-132">7</span><span class="sxs-lookup"><span data-stu-id="2a22f-132">7</span></span>|<span data-ttu-id="2a22f-133">18以上の分類は、18才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="2a22f-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



