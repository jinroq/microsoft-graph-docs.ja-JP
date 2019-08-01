---
title: ratingCanadaTelevisionType 列挙型
description: カナダでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a8dcf918ff5297be45e0954a43c0503798efcc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027959"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="defe3-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="defe3-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="defe3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="defe3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="defe3-105">カナダでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="defe3-105">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="defe3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="defe3-106">Members</span></span>
|<span data-ttu-id="defe3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="defe3-107">Member</span></span>|<span data-ttu-id="defe3-108">値</span><span class="sxs-lookup"><span data-stu-id="defe3-108">Value</span></span>|<span data-ttu-id="defe3-109">説明</span><span class="sxs-lookup"><span data-stu-id="defe3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="defe3-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="defe3-110">allAllowed</span></span>|<span data-ttu-id="defe3-111">.0</span><span class="sxs-lookup"><span data-stu-id="defe3-111">0</span></span>|<span data-ttu-id="defe3-112">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="defe3-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="defe3-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="defe3-113">allBlocked</span></span>|<span data-ttu-id="defe3-114">1-d</span><span class="sxs-lookup"><span data-stu-id="defe3-114">1</span></span>|<span data-ttu-id="defe3-115">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="defe3-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="defe3-116">children</span><span class="sxs-lookup"><span data-stu-id="defe3-116">children</span></span>|<span data-ttu-id="defe3-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="defe3-117">2</span></span>|<span data-ttu-id="defe3-118">C の分類は、2 ~ 7 年の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="defe3-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="defe3-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="defe3-119">childrenAbove8</span></span>|<span data-ttu-id="defe3-120">1/3</span><span class="sxs-lookup"><span data-stu-id="defe3-120">3</span></span>|<span data-ttu-id="defe3-121">C8 の分類は、8才を超える子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="defe3-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="defe3-122">元帳</span><span class="sxs-lookup"><span data-stu-id="defe3-122">general</span></span>|<span data-ttu-id="defe3-123">2/4</span><span class="sxs-lookup"><span data-stu-id="defe3-123">4</span></span>|<span data-ttu-id="defe3-124">G 分類は、一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="defe3-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="defe3-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="defe3-125">parentalGuidance</span></span>|<span data-ttu-id="defe3-126">5</span><span class="sxs-lookup"><span data-stu-id="defe3-126">5</span></span>|<span data-ttu-id="defe3-127">PG、キッズのガイダンス</span><span class="sxs-lookup"><span data-stu-id="defe3-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="defe3-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="defe3-128">agesAbove14</span></span>|<span data-ttu-id="defe3-129">シックス</span><span class="sxs-lookup"><span data-stu-id="defe3-129">6</span></span>|<span data-ttu-id="defe3-130">14以上の分類は、14才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="defe3-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="defe3-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="defe3-131">agesAbove18</span></span>|<span data-ttu-id="defe3-132">7</span><span class="sxs-lookup"><span data-stu-id="defe3-132">7</span></span>|<span data-ttu-id="defe3-133">18以上の分類は、18才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="defe3-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



