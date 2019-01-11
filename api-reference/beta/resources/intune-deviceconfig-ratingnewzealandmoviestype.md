---
title: ratingNewZealandMoviesType 列挙型
description: 映画がニュージーランドでのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 220348375503cca6ab42a9573b8ed5b5850192e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884022"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="a6871-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a6871-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="a6871-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6871-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6871-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6871-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6871-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6871-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6871-107">映画がニュージーランドでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="a6871-107">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="a6871-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6871-108">Members</span></span>
|<span data-ttu-id="a6871-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6871-109">Member</span></span>|<span data-ttu-id="a6871-110">値</span><span class="sxs-lookup"><span data-stu-id="a6871-110">Value</span></span>|<span data-ttu-id="a6871-111">説明</span><span class="sxs-lookup"><span data-stu-id="a6871-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6871-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a6871-112">allAllowed</span></span>|<span data-ttu-id="a6871-113">0</span><span class="sxs-lookup"><span data-stu-id="a6871-113">0</span></span>|<span data-ttu-id="a6871-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="a6871-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="a6871-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a6871-115">allBlocked</span></span>|<span data-ttu-id="a6871-116">1</span><span class="sxs-lookup"><span data-stu-id="a6871-116">1</span></span>|<span data-ttu-id="a6871-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="a6871-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="a6871-118">全般</span><span class="sxs-lookup"><span data-stu-id="a6871-118">general</span></span>|<span data-ttu-id="a6871-119">2</span><span class="sxs-lookup"><span data-stu-id="a6871-119">2</span></span>|<span data-ttu-id="a6871-120">一般的な対象ユーザーに適した</span><span class="sxs-lookup"><span data-stu-id="a6871-120">Suitable for general audience</span></span>|
|<span data-ttu-id="a6871-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="a6871-121">parentalGuidance</span></span>|<span data-ttu-id="a6871-122">3</span><span class="sxs-lookup"><span data-stu-id="a6871-122">3</span></span>|<span data-ttu-id="a6871-123">PG クラス分けは、保護者による制限を推奨します。</span><span class="sxs-lookup"><span data-stu-id="a6871-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="a6871-124">成熟</span><span class="sxs-lookup"><span data-stu-id="a6871-124">mature</span></span>|<span data-ttu-id="a6871-125">4</span><span class="sxs-lookup"><span data-stu-id="a6871-125">4</span></span>|<span data-ttu-id="a6871-126">M のクラス分けが 18 歳以上向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="a6871-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="a6871-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="a6871-127">agesAbove13</span></span>|<span data-ttu-id="a6871-128">5</span><span class="sxs-lookup"><span data-stu-id="a6871-128">5</span></span>|<span data-ttu-id="a6871-129">R13 のクラス分けは 13 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="a6871-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="a6871-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="a6871-130">agesAbove15</span></span>|<span data-ttu-id="a6871-131">6</span><span class="sxs-lookup"><span data-stu-id="a6871-131">6</span></span>|<span data-ttu-id="a6871-132">R15 の各分類は、15 年以上の担当者と制限</span><span class="sxs-lookup"><span data-stu-id="a6871-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="a6871-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="a6871-133">agesAbove16</span></span>|<span data-ttu-id="a6871-134">7</span><span class="sxs-lookup"><span data-stu-id="a6871-134">7</span></span>|<span data-ttu-id="a6871-135">R16 クラス分けは 16 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="a6871-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="a6871-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="a6871-136">agesAbove18</span></span>|<span data-ttu-id="a6871-137">8</span><span class="sxs-lookup"><span data-stu-id="a6871-137">8</span></span>|<span data-ttu-id="a6871-138">R18 の分類は 18 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="a6871-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="a6871-139">制限</span><span class="sxs-lookup"><span data-stu-id="a6871-139">restricted</span></span>|<span data-ttu-id="a6871-140">9</span><span class="sxs-lookup"><span data-stu-id="a6871-140">9</span></span>|<span data-ttu-id="a6871-141">R 分類が特定の対象ユーザーに限定されます。</span><span class="sxs-lookup"><span data-stu-id="a6871-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="a6871-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="a6871-142">agesAbove16Restricted</span></span>|<span data-ttu-id="a6871-143">10</span><span class="sxs-lookup"><span data-stu-id="a6871-143">10</span></span>|<span data-ttu-id="a6871-144">RP16 分類には、視聴者と共に、親または成人向けコンテンツを 16 が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6871-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





