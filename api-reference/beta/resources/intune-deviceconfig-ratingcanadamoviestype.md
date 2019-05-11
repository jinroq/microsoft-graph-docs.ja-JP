---
title: ratingCanadaMoviesType 列挙型
description: カナダでの映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dcb5612be1045c2c99e760ca4056e1f00004367
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950978"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="551e6-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="551e6-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="551e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="551e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="551e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="551e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="551e6-106">カナダでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="551e6-106">Movies rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="551e6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="551e6-107">Members</span></span>
|<span data-ttu-id="551e6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="551e6-108">Member</span></span>|<span data-ttu-id="551e6-109">値</span><span class="sxs-lookup"><span data-stu-id="551e6-109">Value</span></span>|<span data-ttu-id="551e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="551e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="551e6-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="551e6-111">allAllowed</span></span>|<span data-ttu-id="551e6-112">.0</span><span class="sxs-lookup"><span data-stu-id="551e6-112">0</span></span>|<span data-ttu-id="551e6-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="551e6-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="551e6-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="551e6-114">allBlocked</span></span>|<span data-ttu-id="551e6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="551e6-115">1</span></span>|<span data-ttu-id="551e6-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="551e6-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="551e6-117">元帳</span><span class="sxs-lookup"><span data-stu-id="551e6-117">general</span></span>|<span data-ttu-id="551e6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="551e6-118">2</span></span>|<span data-ttu-id="551e6-119">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="551e6-119">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="551e6-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="551e6-120">parentalGuidance</span></span>|<span data-ttu-id="551e6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="551e6-121">3</span></span>|<span data-ttu-id="551e6-122">PG 分類は、保護者によるガイダンスをアドバイスします。</span><span class="sxs-lookup"><span data-stu-id="551e6-122">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="551e6-123">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="551e6-123">agesAbove14</span></span>|<span data-ttu-id="551e6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="551e6-124">4</span></span>|<span data-ttu-id="551e6-125">14A の分類は、14才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="551e6-125">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="551e6-126">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="551e6-126">agesAbove18</span></span>|<span data-ttu-id="551e6-127">5</span><span class="sxs-lookup"><span data-stu-id="551e6-127">5</span></span>|<span data-ttu-id="551e6-128">18A 分類は18またはそれ以前の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="551e6-128">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="551e6-129">しか</span><span class="sxs-lookup"><span data-stu-id="551e6-129">restricted</span></span>|<span data-ttu-id="551e6-130">シックス</span><span class="sxs-lookup"><span data-stu-id="551e6-130">6</span></span>|<span data-ttu-id="551e6-131">R 分類は18年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="551e6-131">The R classification is restricted to 18 years and older</span></span>|




