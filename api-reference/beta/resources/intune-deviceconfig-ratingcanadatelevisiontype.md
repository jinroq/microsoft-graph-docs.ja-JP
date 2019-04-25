---
title: ratingCanadaTelevisionType 列挙型
description: カナダでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fa3989f4fe1324f404a16603f357a81136e1d9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566676"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="ae626-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ae626-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="ae626-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae626-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae626-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae626-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae626-106">カナダでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="ae626-106">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="ae626-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae626-107">Members</span></span>
|<span data-ttu-id="ae626-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae626-108">Member</span></span>|<span data-ttu-id="ae626-109">値</span><span class="sxs-lookup"><span data-stu-id="ae626-109">Value</span></span>|<span data-ttu-id="ae626-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae626-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae626-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="ae626-111">allAllowed</span></span>|<span data-ttu-id="ae626-112">.0</span><span class="sxs-lookup"><span data-stu-id="ae626-112">0</span></span>|<span data-ttu-id="ae626-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="ae626-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="ae626-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="ae626-114">allBlocked</span></span>|<span data-ttu-id="ae626-115">1 </span><span class="sxs-lookup"><span data-stu-id="ae626-115">1</span></span>|<span data-ttu-id="ae626-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="ae626-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="ae626-117">children</span><span class="sxs-lookup"><span data-stu-id="ae626-117">children</span></span>|<span data-ttu-id="ae626-118">2 </span><span class="sxs-lookup"><span data-stu-id="ae626-118">2</span></span>|<span data-ttu-id="ae626-119">C の分類は、2 ~ 7 年の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="ae626-119">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="ae626-120">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="ae626-120">childrenAbove8</span></span>|<span data-ttu-id="ae626-121">3 </span><span class="sxs-lookup"><span data-stu-id="ae626-121">3</span></span>|<span data-ttu-id="ae626-122">C8 の分類は、8才を超える子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="ae626-122">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="ae626-123">元帳</span><span class="sxs-lookup"><span data-stu-id="ae626-123">general</span></span>|<span data-ttu-id="ae626-124">4 </span><span class="sxs-lookup"><span data-stu-id="ae626-124">4</span></span>|<span data-ttu-id="ae626-125">G 分類は、一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="ae626-125">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="ae626-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="ae626-126">parentalGuidance</span></span>|<span data-ttu-id="ae626-127">5 </span><span class="sxs-lookup"><span data-stu-id="ae626-127">5</span></span>|<span data-ttu-id="ae626-128">PG、キッズのガイダンス</span><span class="sxs-lookup"><span data-stu-id="ae626-128">PG, Parental Guidance</span></span>|
|<span data-ttu-id="ae626-129">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="ae626-129">agesAbove14</span></span>|<span data-ttu-id="ae626-130">6 </span><span class="sxs-lookup"><span data-stu-id="ae626-130">6</span></span>|<span data-ttu-id="ae626-131">14以上の分類は、14才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="ae626-131">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="ae626-132">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="ae626-132">agesAbove18</span></span>|<span data-ttu-id="ae626-133">7 </span><span class="sxs-lookup"><span data-stu-id="ae626-133">7</span></span>|<span data-ttu-id="ae626-134">18以上の分類は、18才以上の閲覧者を対象としています。</span><span class="sxs-lookup"><span data-stu-id="ae626-134">The 18+ classification is intended for viewers ages 18 and older</span></span>|





