---
title: ratingNewZealandMoviesType 列挙型
description: 映画がニュージーランドでのラベルの評価
ms.openlocfilehash: eb32d047c4c24e2848e71ab7cc0947d57048d75d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066642"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="c9736-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c9736-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="c9736-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9736-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9736-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9736-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9736-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9736-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9736-107">映画がニュージーランドでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="c9736-107">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="c9736-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9736-108">Members</span></span>
|<span data-ttu-id="c9736-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9736-109">Member</span></span>|<span data-ttu-id="c9736-110">値</span><span class="sxs-lookup"><span data-stu-id="c9736-110">Value</span></span>|<span data-ttu-id="c9736-111">説明</span><span class="sxs-lookup"><span data-stu-id="c9736-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9736-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="c9736-112">allAllowed</span></span>|<span data-ttu-id="c9736-113">0</span><span class="sxs-lookup"><span data-stu-id="c9736-113">0</span></span>|<span data-ttu-id="c9736-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="c9736-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="c9736-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="c9736-115">allBlocked</span></span>|<span data-ttu-id="c9736-116">1</span><span class="sxs-lookup"><span data-stu-id="c9736-116">1</span></span>|<span data-ttu-id="c9736-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="c9736-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="c9736-118">全般</span><span class="sxs-lookup"><span data-stu-id="c9736-118">general</span></span>|<span data-ttu-id="c9736-119">2</span><span class="sxs-lookup"><span data-stu-id="c9736-119">2</span></span>|<span data-ttu-id="c9736-120">一般的な対象ユーザーに適した</span><span class="sxs-lookup"><span data-stu-id="c9736-120">Suitable for general audience</span></span>|
|<span data-ttu-id="c9736-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="c9736-121">parentalGuidance</span></span>|<span data-ttu-id="c9736-122">3</span><span class="sxs-lookup"><span data-stu-id="c9736-122">3</span></span>|<span data-ttu-id="c9736-123">PG クラス分けは、保護者による制限を推奨します。</span><span class="sxs-lookup"><span data-stu-id="c9736-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="c9736-124">成熟</span><span class="sxs-lookup"><span data-stu-id="c9736-124">mature</span></span>|<span data-ttu-id="c9736-125">4</span><span class="sxs-lookup"><span data-stu-id="c9736-125">4</span></span>|<span data-ttu-id="c9736-126">M のクラス分けが 18 歳以上向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="c9736-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="c9736-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="c9736-127">agesAbove13</span></span>|<span data-ttu-id="c9736-128">5</span><span class="sxs-lookup"><span data-stu-id="c9736-128">5</span></span>|<span data-ttu-id="c9736-129">R13 のクラス分けは 13 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="c9736-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="c9736-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="c9736-130">agesAbove15</span></span>|<span data-ttu-id="c9736-131">6</span><span class="sxs-lookup"><span data-stu-id="c9736-131">6</span></span>|<span data-ttu-id="c9736-132">R15 の各分類は、15 年以上の担当者と制限</span><span class="sxs-lookup"><span data-stu-id="c9736-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="c9736-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="c9736-133">agesAbove16</span></span>|<span data-ttu-id="c9736-134">7</span><span class="sxs-lookup"><span data-stu-id="c9736-134">7</span></span>|<span data-ttu-id="c9736-135">R16 クラス分けは 16 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="c9736-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="c9736-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="c9736-136">agesAbove18</span></span>|<span data-ttu-id="c9736-137">8</span><span class="sxs-lookup"><span data-stu-id="c9736-137">8</span></span>|<span data-ttu-id="c9736-138">R18 の分類は 18 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="c9736-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="c9736-139">制限</span><span class="sxs-lookup"><span data-stu-id="c9736-139">restricted</span></span>|<span data-ttu-id="c9736-140">9</span><span class="sxs-lookup"><span data-stu-id="c9736-140">9</span></span>|<span data-ttu-id="c9736-141">R 分類が特定の対象ユーザーに限定されます。</span><span class="sxs-lookup"><span data-stu-id="c9736-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="c9736-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="c9736-142">agesAbove16Restricted</span></span>|<span data-ttu-id="c9736-143">10</span><span class="sxs-lookup"><span data-stu-id="c9736-143">10</span></span>|<span data-ttu-id="c9736-144">RP16 分類には、視聴者と共に、親または成人向けコンテンツを 16 が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9736-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





