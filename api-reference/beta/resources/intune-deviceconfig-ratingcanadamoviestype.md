---
title: ratingCanadaMoviesType 列挙型
description: 映画がカナダでのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f35289348dbe94b5be3aa5a1d96709de8e8869
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398409"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="d1702-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1702-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="d1702-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1702-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1702-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1702-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1702-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1702-107">映画がカナダでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="d1702-107">Movies rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="d1702-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1702-108">Members</span></span>
|<span data-ttu-id="d1702-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1702-109">Member</span></span>|<span data-ttu-id="d1702-110">値</span><span class="sxs-lookup"><span data-stu-id="d1702-110">Value</span></span>|<span data-ttu-id="d1702-111">説明</span><span class="sxs-lookup"><span data-stu-id="d1702-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1702-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d1702-112">allAllowed</span></span>|<span data-ttu-id="d1702-113">0</span><span class="sxs-lookup"><span data-stu-id="d1702-113">0</span></span>|<span data-ttu-id="d1702-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="d1702-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="d1702-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d1702-115">allBlocked</span></span>|<span data-ttu-id="d1702-116">1</span><span class="sxs-lookup"><span data-stu-id="d1702-116">1</span></span>|<span data-ttu-id="d1702-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="d1702-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="d1702-118">全般</span><span class="sxs-lookup"><span data-stu-id="d1702-118">general</span></span>|<span data-ttu-id="d1702-119">2</span><span class="sxs-lookup"><span data-stu-id="d1702-119">2</span></span>|<span data-ttu-id="d1702-120">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="d1702-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="d1702-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d1702-121">parentalGuidance</span></span>|<span data-ttu-id="d1702-122">3</span><span class="sxs-lookup"><span data-stu-id="d1702-122">3</span></span>|<span data-ttu-id="d1702-123">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="d1702-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="d1702-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="d1702-124">agesAbove14</span></span>|<span data-ttu-id="d1702-125">4</span><span class="sxs-lookup"><span data-stu-id="d1702-125">4</span></span>|<span data-ttu-id="d1702-126">14A 分類が 14 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="d1702-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="d1702-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="d1702-127">agesAbove18</span></span>|<span data-ttu-id="d1702-128">5</span><span class="sxs-lookup"><span data-stu-id="d1702-128">5</span></span>|<span data-ttu-id="d1702-129">18A 分類が 18 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="d1702-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="d1702-130">制限</span><span class="sxs-lookup"><span data-stu-id="d1702-130">restricted</span></span>|<span data-ttu-id="d1702-131">6</span><span class="sxs-lookup"><span data-stu-id="d1702-131">6</span></span>|<span data-ttu-id="d1702-132">R のクラス分けは、18 年間に限定され、古い</span><span class="sxs-lookup"><span data-stu-id="d1702-132">The R classification is restricted to 18 years and older</span></span>|




