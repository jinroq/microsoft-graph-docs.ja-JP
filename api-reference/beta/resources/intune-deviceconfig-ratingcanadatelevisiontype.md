---
title: ratingCanadaTelevisionType 列挙型
description: カナダでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fa3989f4fe1324f404a16603f357a81136e1d9e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806973"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="32294-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="32294-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="32294-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32294-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32294-106">カナダでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="32294-106">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="32294-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="32294-107">Members</span></span>
|<span data-ttu-id="32294-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="32294-108">Member</span></span>|<span data-ttu-id="32294-109">値</span><span class="sxs-lookup"><span data-stu-id="32294-109">Value</span></span>|<span data-ttu-id="32294-110">説明</span><span class="sxs-lookup"><span data-stu-id="32294-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32294-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="32294-111">allAllowed</span></span>|<span data-ttu-id="32294-112">.0</span><span class="sxs-lookup"><span data-stu-id="32294-112">0</span></span>|<span data-ttu-id="32294-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="32294-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="32294-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="32294-114">allBlocked</span></span>|<span data-ttu-id="32294-115">1-d</span><span class="sxs-lookup"><span data-stu-id="32294-115">1</span></span>|<span data-ttu-id="32294-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="32294-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="32294-117">children</span><span class="sxs-lookup"><span data-stu-id="32294-117">children</span></span>|<span data-ttu-id="32294-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="32294-118">2</span></span>|<span data-ttu-id="32294-119">C の分類は、2 ~ 7 年の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="32294-119">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="32294-120">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="32294-120">childrenAbove8</span></span>|<span data-ttu-id="32294-121">1/3</span><span class="sxs-lookup"><span data-stu-id="32294-121">3</span></span>|<span data-ttu-id="32294-122">C8 の分類は、8才を超える子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="32294-122">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="32294-123">元帳</span><span class="sxs-lookup"><span data-stu-id="32294-123">general</span></span>|<span data-ttu-id="32294-124">2/4</span><span class="sxs-lookup"><span data-stu-id="32294-124">4</span></span>|<span data-ttu-id="32294-125">G 分類は、一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="32294-125">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="32294-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="32294-126">parentalGuidance</span></span>|<span data-ttu-id="32294-127">5</span><span class="sxs-lookup"><span data-stu-id="32294-127">5</span></span>|<span data-ttu-id="32294-128">PG、キッズのガイダンス</span><span class="sxs-lookup"><span data-stu-id="32294-128">PG, Parental Guidance</span></span>|
|<span data-ttu-id="32294-129">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="32294-129">agesAbove14</span></span>|<span data-ttu-id="32294-130">シックス</span><span class="sxs-lookup"><span data-stu-id="32294-130">6</span></span>|<span data-ttu-id="32294-131">14以上の分類は、14才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="32294-131">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="32294-132">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="32294-132">agesAbove18</span></span>|<span data-ttu-id="32294-133">7</span><span class="sxs-lookup"><span data-stu-id="32294-133">7</span></span>|<span data-ttu-id="32294-134">18以上の分類は、18才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="32294-134">The 18+ classification is intended for viewers ages 18 and older</span></span>|





