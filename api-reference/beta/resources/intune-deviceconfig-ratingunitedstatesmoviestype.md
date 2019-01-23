---
title: ratingUnitedStatesMoviesType 列挙型
description: 映画が米国でのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c14fcc87c949e3f16403ca4654ec987423f8b647
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412227"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="1732a-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1732a-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="1732a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1732a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1732a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1732a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1732a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1732a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1732a-107">映画が米国でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="1732a-107">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="1732a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1732a-108">Members</span></span>
|<span data-ttu-id="1732a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1732a-109">Member</span></span>|<span data-ttu-id="1732a-110">値</span><span class="sxs-lookup"><span data-stu-id="1732a-110">Value</span></span>|<span data-ttu-id="1732a-111">説明</span><span class="sxs-lookup"><span data-stu-id="1732a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1732a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="1732a-112">allAllowed</span></span>|<span data-ttu-id="1732a-113">0</span><span class="sxs-lookup"><span data-stu-id="1732a-113">0</span></span>|<span data-ttu-id="1732a-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="1732a-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="1732a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="1732a-115">allBlocked</span></span>|<span data-ttu-id="1732a-116">1</span><span class="sxs-lookup"><span data-stu-id="1732a-116">1</span></span>|<span data-ttu-id="1732a-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="1732a-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="1732a-118">全般</span><span class="sxs-lookup"><span data-stu-id="1732a-118">general</span></span>|<span data-ttu-id="1732a-119">2</span><span class="sxs-lookup"><span data-stu-id="1732a-119">2</span></span>|<span data-ttu-id="1732a-120">G、すべての年代の参加を許可</span><span class="sxs-lookup"><span data-stu-id="1732a-120">G, all ages admitted</span></span>|
|<span data-ttu-id="1732a-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="1732a-121">parentalGuidance</span></span>|<span data-ttu-id="1732a-122">3</span><span class="sxs-lookup"><span data-stu-id="1732a-122">3</span></span>|<span data-ttu-id="1732a-123">PG、可能性がありますだと内容が子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="1732a-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="1732a-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="1732a-124">parentalGuidance13</span></span>|<span data-ttu-id="1732a-125">4</span><span class="sxs-lookup"><span data-stu-id="1732a-125">4</span></span>|<span data-ttu-id="1732a-126">PG13、いくつかの材料があります 13 才未満の子供に適切です</span><span class="sxs-lookup"><span data-stu-id="1732a-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="1732a-127">制限</span><span class="sxs-lookup"><span data-stu-id="1732a-127">restricted</span></span>|<span data-ttu-id="1732a-128">5</span><span class="sxs-lookup"><span data-stu-id="1732a-128">5</span></span>|<span data-ttu-id="1732a-129">親または大人の同伴に付属する R、17 歳未満の閲覧者が必要な</span><span class="sxs-lookup"><span data-stu-id="1732a-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="1732a-130">大人</span><span class="sxs-lookup"><span data-stu-id="1732a-130">adults</span></span>|<span data-ttu-id="1732a-131">6</span><span class="sxs-lookup"><span data-stu-id="1732a-131">6</span></span>|<span data-ttu-id="1732a-132">NC17、成人のみ</span><span class="sxs-lookup"><span data-stu-id="1732a-132">NC17, adults only</span></span>|




