---
title: ratingUnitedStatesMoviesType 列挙型
description: 米国での映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b32de63fe5b559b76a0de0ca2471230c8f637406
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944846"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="faaad-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="faaad-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="faaad-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faaad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faaad-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="faaad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faaad-106">米国での映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="faaad-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="faaad-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="faaad-107">Members</span></span>
|<span data-ttu-id="faaad-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="faaad-108">Member</span></span>|<span data-ttu-id="faaad-109">値</span><span class="sxs-lookup"><span data-stu-id="faaad-109">Value</span></span>|<span data-ttu-id="faaad-110">説明</span><span class="sxs-lookup"><span data-stu-id="faaad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faaad-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="faaad-111">allAllowed</span></span>|<span data-ttu-id="faaad-112">.0</span><span class="sxs-lookup"><span data-stu-id="faaad-112">0</span></span>|<span data-ttu-id="faaad-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="faaad-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="faaad-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="faaad-114">allBlocked</span></span>|<span data-ttu-id="faaad-115">1-d</span><span class="sxs-lookup"><span data-stu-id="faaad-115">1</span></span>|<span data-ttu-id="faaad-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="faaad-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="faaad-117">元帳</span><span class="sxs-lookup"><span data-stu-id="faaad-117">general</span></span>|<span data-ttu-id="faaad-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="faaad-118">2</span></span>|<span data-ttu-id="faaad-119">G、すべての年齢が許可</span><span class="sxs-lookup"><span data-stu-id="faaad-119">G, all ages admitted</span></span>|
|<span data-ttu-id="faaad-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="faaad-120">parentalGuidance</span></span>|<span data-ttu-id="faaad-121">1/3</span><span class="sxs-lookup"><span data-stu-id="faaad-121">3</span></span>|<span data-ttu-id="faaad-122">PG では、一部の素材が子供に適さない場合があります。</span><span class="sxs-lookup"><span data-stu-id="faaad-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="faaad-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="faaad-123">parentalGuidance13</span></span>|<span data-ttu-id="faaad-124">2/4</span><span class="sxs-lookup"><span data-stu-id="faaad-124">4</span></span>|<span data-ttu-id="faaad-125">PG13 では、いくつかの素材が13の子に対して不適切な場合があります。</span><span class="sxs-lookup"><span data-stu-id="faaad-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="faaad-126">しか</span><span class="sxs-lookup"><span data-stu-id="faaad-126">restricted</span></span>|<span data-ttu-id="faaad-127">5</span><span class="sxs-lookup"><span data-stu-id="faaad-127">5</span></span>|<span data-ttu-id="faaad-128">R、17の下の閲覧者には、親または成人のガーディアンが必要です</span><span class="sxs-lookup"><span data-stu-id="faaad-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="faaad-129">保護者</span><span class="sxs-lookup"><span data-stu-id="faaad-129">adults</span></span>|<span data-ttu-id="faaad-130">シックス</span><span class="sxs-lookup"><span data-stu-id="faaad-130">6</span></span>|<span data-ttu-id="faaad-131">NC17、大人のみ</span><span class="sxs-lookup"><span data-stu-id="faaad-131">NC17, adults only</span></span>|




