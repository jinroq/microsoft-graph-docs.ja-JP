---
title: ratingGermanyMoviesType 列挙型
description: 映画のドイツのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dfa8211b562fac95e5c325c9afe682c38e5272db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395875"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="7c302-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7c302-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="7c302-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c302-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c302-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c302-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c302-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c302-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c302-107">映画のドイツのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="7c302-107">Movies rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="7c302-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c302-108">Members</span></span>
|<span data-ttu-id="7c302-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c302-109">Member</span></span>|<span data-ttu-id="7c302-110">値</span><span class="sxs-lookup"><span data-stu-id="7c302-110">Value</span></span>|<span data-ttu-id="7c302-111">説明</span><span class="sxs-lookup"><span data-stu-id="7c302-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c302-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="7c302-112">allAllowed</span></span>|<span data-ttu-id="7c302-113">0</span><span class="sxs-lookup"><span data-stu-id="7c302-113">0</span></span>|<span data-ttu-id="7c302-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="7c302-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="7c302-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="7c302-115">allBlocked</span></span>|<span data-ttu-id="7c302-116">1</span><span class="sxs-lookup"><span data-stu-id="7c302-116">1</span></span>|<span data-ttu-id="7c302-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="7c302-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="7c302-118">全般</span><span class="sxs-lookup"><span data-stu-id="7c302-118">general</span></span>|<span data-ttu-id="7c302-119">2</span><span class="sxs-lookup"><span data-stu-id="7c302-119">2</span></span>|<span data-ttu-id="7c302-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="7c302-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="7c302-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="7c302-121">agesAbove6</span></span>|<span data-ttu-id="7c302-122">3</span><span class="sxs-lookup"><span data-stu-id="7c302-122">3</span></span>|<span data-ttu-id="7c302-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="7c302-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="7c302-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="7c302-124">agesAbove12</span></span>|<span data-ttu-id="7c302-125">4</span><span class="sxs-lookup"><span data-stu-id="7c302-125">4</span></span>|<span data-ttu-id="7c302-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="7c302-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="7c302-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="7c302-127">agesAbove16</span></span>|<span data-ttu-id="7c302-128">5</span><span class="sxs-lookup"><span data-stu-id="7c302-128">5</span></span>|<span data-ttu-id="7c302-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="7c302-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="7c302-130">大人</span><span class="sxs-lookup"><span data-stu-id="7c302-130">adults</span></span>|<span data-ttu-id="7c302-131">6</span><span class="sxs-lookup"><span data-stu-id="7c302-131">6</span></span>|<span data-ttu-id="7c302-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="7c302-132">Ab 18 Jahren, adults only</span></span>|




