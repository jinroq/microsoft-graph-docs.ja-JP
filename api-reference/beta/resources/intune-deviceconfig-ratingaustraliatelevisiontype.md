---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアでのテレビコンテンツの評価のラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69fdd926d02a2ae150f10a0d911854538a5d2f69
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368360"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="15350-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="15350-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="15350-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15350-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15350-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15350-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15350-106">オーストラリアでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="15350-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="15350-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="15350-107">Members</span></span>
|<span data-ttu-id="15350-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="15350-108">Member</span></span>|<span data-ttu-id="15350-109">値</span><span class="sxs-lookup"><span data-stu-id="15350-109">Value</span></span>|<span data-ttu-id="15350-110">説明</span><span class="sxs-lookup"><span data-stu-id="15350-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15350-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="15350-111">allAllowed</span></span>|<span data-ttu-id="15350-112">.0</span><span class="sxs-lookup"><span data-stu-id="15350-112">0</span></span>|<span data-ttu-id="15350-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="15350-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="15350-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="15350-114">allBlocked</span></span>|<span data-ttu-id="15350-115">1-d</span><span class="sxs-lookup"><span data-stu-id="15350-115">1</span></span>|<span data-ttu-id="15350-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="15350-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="15350-117">prespreser</span><span class="sxs-lookup"><span data-stu-id="15350-117">preschoolers</span></span>|<span data-ttu-id="15350-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="15350-118">2</span></span>|<span data-ttu-id="15350-119">P 分類は、preschoolers に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="15350-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="15350-120">children</span><span class="sxs-lookup"><span data-stu-id="15350-120">children</span></span>|<span data-ttu-id="15350-121">1/3</span><span class="sxs-lookup"><span data-stu-id="15350-121">3</span></span>|<span data-ttu-id="15350-122">C の分類は、14の下の子を対象としています。</span><span class="sxs-lookup"><span data-stu-id="15350-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="15350-123">元帳</span><span class="sxs-lookup"><span data-stu-id="15350-123">general</span></span>|<span data-ttu-id="15350-124">2/4</span><span class="sxs-lookup"><span data-stu-id="15350-124">4</span></span>|<span data-ttu-id="15350-125">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="15350-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="15350-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="15350-126">parentalGuidance</span></span>|<span data-ttu-id="15350-127">5</span><span class="sxs-lookup"><span data-stu-id="15350-127">5</span></span>|<span data-ttu-id="15350-128">閲覧者には PG 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="15350-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="15350-129">度</span><span class="sxs-lookup"><span data-stu-id="15350-129">mature</span></span>|<span data-ttu-id="15350-130">シックス</span><span class="sxs-lookup"><span data-stu-id="15350-130">6</span></span>|<span data-ttu-id="15350-131">15を超える閲覧者には M 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="15350-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="15350-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="15350-132">agesAbove15</span></span>|<span data-ttu-id="15350-133">7</span><span class="sxs-lookup"><span data-stu-id="15350-133">7</span></span>|<span data-ttu-id="15350-134">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="15350-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="15350-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="15350-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="15350-136">8 </span><span class="sxs-lookup"><span data-stu-id="15350-136">8</span></span>|<span data-ttu-id="15350-137">AV15 + 分類は、15の下の閲覧者には適していません。成人の暴力に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="15350-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



