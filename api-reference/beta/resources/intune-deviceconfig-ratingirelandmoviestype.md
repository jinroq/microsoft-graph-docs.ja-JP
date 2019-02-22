---
title: ratingIrelandMoviesType 列挙型
description: アイルランドでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59659848237dd75eea69aa93fb07badfc2434563
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139460"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="ed68a-103">ratingIrelandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ed68a-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="ed68a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed68a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed68a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed68a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed68a-106">アイルランドでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="ed68a-106">Movies rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="ed68a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed68a-107">Members</span></span>
|<span data-ttu-id="ed68a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed68a-108">Member</span></span>|<span data-ttu-id="ed68a-109">値</span><span class="sxs-lookup"><span data-stu-id="ed68a-109">Value</span></span>|<span data-ttu-id="ed68a-110">説明</span><span class="sxs-lookup"><span data-stu-id="ed68a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed68a-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="ed68a-111">allAllowed</span></span>|<span data-ttu-id="ed68a-112">.0</span><span class="sxs-lookup"><span data-stu-id="ed68a-112">0</span></span>|<span data-ttu-id="ed68a-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="ed68a-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="ed68a-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="ed68a-114">allBlocked</span></span>|<span data-ttu-id="ed68a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ed68a-115">1</span></span>|<span data-ttu-id="ed68a-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="ed68a-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="ed68a-117">元帳</span><span class="sxs-lookup"><span data-stu-id="ed68a-117">general</span></span>|<span data-ttu-id="ed68a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ed68a-118">2</span></span>|<span data-ttu-id="ed68a-119">学校の年齢の子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="ed68a-119">Suitable for children of school going age</span></span>|
|<span data-ttu-id="ed68a-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="ed68a-120">parentalGuidance</span></span>|<span data-ttu-id="ed68a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ed68a-121">3</span></span>|<span data-ttu-id="ed68a-122">PG 分類は、保護者によるガイダンスをアドバイスします。</span><span class="sxs-lookup"><span data-stu-id="ed68a-122">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="ed68a-123">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="ed68a-123">agesAbove12</span></span>|<span data-ttu-id="ed68a-124">2/4</span><span class="sxs-lookup"><span data-stu-id="ed68a-124">4</span></span>|<span data-ttu-id="ed68a-125">12a の分類は、12才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="ed68a-125">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="ed68a-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="ed68a-126">agesAbove15</span></span>|<span data-ttu-id="ed68a-127">5</span><span class="sxs-lookup"><span data-stu-id="ed68a-127">5</span></span>|<span data-ttu-id="ed68a-128">15A 分類は、15才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="ed68a-128">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="ed68a-129">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="ed68a-129">agesAbove16</span></span>|<span data-ttu-id="ed68a-130">シックス</span><span class="sxs-lookup"><span data-stu-id="ed68a-130">6</span></span>|<span data-ttu-id="ed68a-131">16以上の16の分類は、16才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="ed68a-131">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="ed68a-132">保護者</span><span class="sxs-lookup"><span data-stu-id="ed68a-132">adults</span></span>|<span data-ttu-id="ed68a-133">7</span><span class="sxs-lookup"><span data-stu-id="ed68a-133">7</span></span>|<span data-ttu-id="ed68a-134">18分類、成人向けにのみ適している</span><span class="sxs-lookup"><span data-stu-id="ed68a-134">The 18 classification, suitable only for adults</span></span>|




