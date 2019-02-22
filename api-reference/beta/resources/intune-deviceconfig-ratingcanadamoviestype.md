---
title: ratingCanadaMoviesType 列挙型
description: カナダでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a1ebcc17e324cc617235761be499f56a1a17ffe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142589"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="8ab10-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8ab10-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="8ab10-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ab10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ab10-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ab10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab10-106">カナダでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="8ab10-106">Movies rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="8ab10-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8ab10-107">Members</span></span>
|<span data-ttu-id="8ab10-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8ab10-108">Member</span></span>|<span data-ttu-id="8ab10-109">値</span><span class="sxs-lookup"><span data-stu-id="8ab10-109">Value</span></span>|<span data-ttu-id="8ab10-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ab10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab10-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="8ab10-111">allAllowed</span></span>|<span data-ttu-id="8ab10-112">.0</span><span class="sxs-lookup"><span data-stu-id="8ab10-112">0</span></span>|<span data-ttu-id="8ab10-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="8ab10-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="8ab10-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="8ab10-114">allBlocked</span></span>|<span data-ttu-id="8ab10-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8ab10-115">1</span></span>|<span data-ttu-id="8ab10-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="8ab10-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="8ab10-117">元帳</span><span class="sxs-lookup"><span data-stu-id="8ab10-117">general</span></span>|<span data-ttu-id="8ab10-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8ab10-118">2</span></span>|<span data-ttu-id="8ab10-119">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="8ab10-119">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="8ab10-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="8ab10-120">parentalGuidance</span></span>|<span data-ttu-id="8ab10-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8ab10-121">3</span></span>|<span data-ttu-id="8ab10-122">PG 分類は、保護者によるガイダンスをアドバイスします。</span><span class="sxs-lookup"><span data-stu-id="8ab10-122">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="8ab10-123">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="8ab10-123">agesAbove14</span></span>|<span data-ttu-id="8ab10-124">2/4</span><span class="sxs-lookup"><span data-stu-id="8ab10-124">4</span></span>|<span data-ttu-id="8ab10-125">14A の分類は、14才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="8ab10-125">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="8ab10-126">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="8ab10-126">agesAbove18</span></span>|<span data-ttu-id="8ab10-127">5</span><span class="sxs-lookup"><span data-stu-id="8ab10-127">5</span></span>|<span data-ttu-id="8ab10-128">18a 分類は18またはそれ以前の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="8ab10-128">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="8ab10-129">しか</span><span class="sxs-lookup"><span data-stu-id="8ab10-129">restricted</span></span>|<span data-ttu-id="8ab10-130">シックス</span><span class="sxs-lookup"><span data-stu-id="8ab10-130">6</span></span>|<span data-ttu-id="8ab10-131">R 分類は18年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="8ab10-131">The R classification is restricted to 18 years and older</span></span>|




