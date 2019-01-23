---
title: ratingNewZealandMoviesType 列挙型
description: 映画がニュージーランドでのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b60bb2d443763115bb547c254ab086b171033658
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402945"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="95b09-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="95b09-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="95b09-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95b09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95b09-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95b09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95b09-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95b09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b09-107">映画がニュージーランドでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="95b09-107">Movies rating labels in New Zealand</span></span>

## <a name="members"></a><span data-ttu-id="95b09-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="95b09-108">Members</span></span>
|<span data-ttu-id="95b09-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="95b09-109">Member</span></span>|<span data-ttu-id="95b09-110">値</span><span class="sxs-lookup"><span data-stu-id="95b09-110">Value</span></span>|<span data-ttu-id="95b09-111">説明</span><span class="sxs-lookup"><span data-stu-id="95b09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b09-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="95b09-112">allAllowed</span></span>|<span data-ttu-id="95b09-113">0</span><span class="sxs-lookup"><span data-stu-id="95b09-113">0</span></span>|<span data-ttu-id="95b09-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="95b09-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="95b09-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="95b09-115">allBlocked</span></span>|<span data-ttu-id="95b09-116">1</span><span class="sxs-lookup"><span data-stu-id="95b09-116">1</span></span>|<span data-ttu-id="95b09-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="95b09-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="95b09-118">全般</span><span class="sxs-lookup"><span data-stu-id="95b09-118">general</span></span>|<span data-ttu-id="95b09-119">2</span><span class="sxs-lookup"><span data-stu-id="95b09-119">2</span></span>|<span data-ttu-id="95b09-120">一般的な対象ユーザーに適した</span><span class="sxs-lookup"><span data-stu-id="95b09-120">Suitable for general audience</span></span>|
|<span data-ttu-id="95b09-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="95b09-121">parentalGuidance</span></span>|<span data-ttu-id="95b09-122">3</span><span class="sxs-lookup"><span data-stu-id="95b09-122">3</span></span>|<span data-ttu-id="95b09-123">PG クラス分けは、保護者による制限を推奨します。</span><span class="sxs-lookup"><span data-stu-id="95b09-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="95b09-124">成熟</span><span class="sxs-lookup"><span data-stu-id="95b09-124">mature</span></span>|<span data-ttu-id="95b09-125">4</span><span class="sxs-lookup"><span data-stu-id="95b09-125">4</span></span>|<span data-ttu-id="95b09-126">M のクラス分けが 18 歳以上向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="95b09-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="95b09-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="95b09-127">agesAbove13</span></span>|<span data-ttu-id="95b09-128">5</span><span class="sxs-lookup"><span data-stu-id="95b09-128">5</span></span>|<span data-ttu-id="95b09-129">R13 のクラス分けは 13 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="95b09-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="95b09-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="95b09-130">agesAbove15</span></span>|<span data-ttu-id="95b09-131">6</span><span class="sxs-lookup"><span data-stu-id="95b09-131">6</span></span>|<span data-ttu-id="95b09-132">R15 の各分類は、15 年以上の担当者と制限</span><span class="sxs-lookup"><span data-stu-id="95b09-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="95b09-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="95b09-133">agesAbove16</span></span>|<span data-ttu-id="95b09-134">7</span><span class="sxs-lookup"><span data-stu-id="95b09-134">7</span></span>|<span data-ttu-id="95b09-135">R16 クラス分けは 16 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="95b09-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="95b09-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="95b09-136">agesAbove18</span></span>|<span data-ttu-id="95b09-137">8</span><span class="sxs-lookup"><span data-stu-id="95b09-137">8</span></span>|<span data-ttu-id="95b09-138">R18 の分類は 18 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="95b09-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="95b09-139">制限</span><span class="sxs-lookup"><span data-stu-id="95b09-139">restricted</span></span>|<span data-ttu-id="95b09-140">9</span><span class="sxs-lookup"><span data-stu-id="95b09-140">9</span></span>|<span data-ttu-id="95b09-141">R 分類が特定の対象ユーザーに限定されます。</span><span class="sxs-lookup"><span data-stu-id="95b09-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="95b09-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="95b09-142">agesAbove16Restricted</span></span>|<span data-ttu-id="95b09-143">10</span><span class="sxs-lookup"><span data-stu-id="95b09-143">10</span></span>|<span data-ttu-id="95b09-144">RP16 分類には、視聴者と共に、親または成人向けコンテンツを 16 が必要です。</span><span class="sxs-lookup"><span data-stu-id="95b09-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|




