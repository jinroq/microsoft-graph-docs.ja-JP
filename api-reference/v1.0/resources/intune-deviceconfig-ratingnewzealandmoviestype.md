---
title: ratingNewZealandMoviesType 列挙型
description: 映画がニュージーランドでのラベルの評価
ms.openlocfilehash: 2c8e1d6564760cb7539e8e4c01167e5473b3fe18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020917"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="f82da-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f82da-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="f82da-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f82da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f82da-105">映画がニュージーランドでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="f82da-105">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="f82da-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f82da-106">Members</span></span>
|<span data-ttu-id="f82da-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f82da-107">Member</span></span>|<span data-ttu-id="f82da-108">値</span><span class="sxs-lookup"><span data-stu-id="f82da-108">Value</span></span>|<span data-ttu-id="f82da-109">説明</span><span class="sxs-lookup"><span data-stu-id="f82da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f82da-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f82da-110">allAllowed</span></span>|<span data-ttu-id="f82da-111">0</span><span class="sxs-lookup"><span data-stu-id="f82da-111">0</span></span>|<span data-ttu-id="f82da-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="f82da-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="f82da-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f82da-113">allBlocked</span></span>|<span data-ttu-id="f82da-114">1</span><span class="sxs-lookup"><span data-stu-id="f82da-114">1</span></span>|<span data-ttu-id="f82da-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="f82da-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="f82da-116">全般</span><span class="sxs-lookup"><span data-stu-id="f82da-116">general</span></span>|<span data-ttu-id="f82da-117">2</span><span class="sxs-lookup"><span data-stu-id="f82da-117">2</span></span>|<span data-ttu-id="f82da-118">一般的な対象ユーザーに適した</span><span class="sxs-lookup"><span data-stu-id="f82da-118">Suitable for general audience</span></span>|
|<span data-ttu-id="f82da-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="f82da-119">parentalGuidance</span></span>|<span data-ttu-id="f82da-120">3</span><span class="sxs-lookup"><span data-stu-id="f82da-120">3</span></span>|<span data-ttu-id="f82da-121">PG クラス分けは、保護者による制限を推奨します。</span><span class="sxs-lookup"><span data-stu-id="f82da-121">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="f82da-122">成熟</span><span class="sxs-lookup"><span data-stu-id="f82da-122">mature</span></span>|<span data-ttu-id="f82da-123">4</span><span class="sxs-lookup"><span data-stu-id="f82da-123">4</span></span>|<span data-ttu-id="f82da-124">M のクラス分けが 18 歳以上向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="f82da-124">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="f82da-125">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="f82da-125">agesAbove13</span></span>|<span data-ttu-id="f82da-126">5</span><span class="sxs-lookup"><span data-stu-id="f82da-126">5</span></span>|<span data-ttu-id="f82da-127">R13 のクラス分けは 13 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="f82da-127">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="f82da-128">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="f82da-128">agesAbove15</span></span>|<span data-ttu-id="f82da-129">6</span><span class="sxs-lookup"><span data-stu-id="f82da-129">6</span></span>|<span data-ttu-id="f82da-130">R15 の各分類は、15 年以上の担当者と制限</span><span class="sxs-lookup"><span data-stu-id="f82da-130">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="f82da-131">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="f82da-131">agesAbove16</span></span>|<span data-ttu-id="f82da-132">7</span><span class="sxs-lookup"><span data-stu-id="f82da-132">7</span></span>|<span data-ttu-id="f82da-133">R16 クラス分けは 16 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="f82da-133">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="f82da-134">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f82da-134">agesAbove18</span></span>|<span data-ttu-id="f82da-135">8</span><span class="sxs-lookup"><span data-stu-id="f82da-135">8</span></span>|<span data-ttu-id="f82da-136">R18 の分類は 18 年間の担当者と制限されました。</span><span class="sxs-lookup"><span data-stu-id="f82da-136">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="f82da-137">制限</span><span class="sxs-lookup"><span data-stu-id="f82da-137">restricted</span></span>|<span data-ttu-id="f82da-138">9</span><span class="sxs-lookup"><span data-stu-id="f82da-138">9</span></span>|<span data-ttu-id="f82da-139">R 分類が特定の対象ユーザーに限定されます。</span><span class="sxs-lookup"><span data-stu-id="f82da-139">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="f82da-140">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="f82da-140">agesAbove16Restricted</span></span>|<span data-ttu-id="f82da-141">10</span><span class="sxs-lookup"><span data-stu-id="f82da-141">10</span></span>|<span data-ttu-id="f82da-142">RP16 分類には、視聴者と共に、親または成人向けコンテンツを 16 が必要です。</span><span class="sxs-lookup"><span data-stu-id="f82da-142">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|



