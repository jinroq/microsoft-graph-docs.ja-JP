---
title: ratingNewZealandMoviesType 列挙型
description: ニュージーランドでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e66a3443de86332b17f017d4768b9e983fb16241
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556957"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="2ba34-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2ba34-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="2ba34-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ba34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba34-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ba34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba34-106">ニュージーランドでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="2ba34-106">Movies rating labels in New Zealand</span></span>

## <a name="members"></a><span data-ttu-id="2ba34-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2ba34-107">Members</span></span>
|<span data-ttu-id="2ba34-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2ba34-108">Member</span></span>|<span data-ttu-id="2ba34-109">値</span><span class="sxs-lookup"><span data-stu-id="2ba34-109">Value</span></span>|<span data-ttu-id="2ba34-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ba34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba34-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="2ba34-111">allAllowed</span></span>|<span data-ttu-id="2ba34-112">.0</span><span class="sxs-lookup"><span data-stu-id="2ba34-112">0</span></span>|<span data-ttu-id="2ba34-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="2ba34-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="2ba34-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="2ba34-114">allBlocked</span></span>|<span data-ttu-id="2ba34-115">1 </span><span class="sxs-lookup"><span data-stu-id="2ba34-115">1</span></span>|<span data-ttu-id="2ba34-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="2ba34-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="2ba34-117">元帳</span><span class="sxs-lookup"><span data-stu-id="2ba34-117">general</span></span>|<span data-ttu-id="2ba34-118">2 </span><span class="sxs-lookup"><span data-stu-id="2ba34-118">2</span></span>|<span data-ttu-id="2ba34-119">一般的な対象ユーザーに適している</span><span class="sxs-lookup"><span data-stu-id="2ba34-119">Suitable for general audience</span></span>|
|<span data-ttu-id="2ba34-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="2ba34-120">parentalGuidance</span></span>|<span data-ttu-id="2ba34-121">3 </span><span class="sxs-lookup"><span data-stu-id="2ba34-121">3</span></span>|<span data-ttu-id="2ba34-122">PG の分類では、保護者による指導を推奨</span><span class="sxs-lookup"><span data-stu-id="2ba34-122">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="2ba34-123">度</span><span class="sxs-lookup"><span data-stu-id="2ba34-123">mature</span></span>|<span data-ttu-id="2ba34-124">4 </span><span class="sxs-lookup"><span data-stu-id="2ba34-124">4</span></span>|<span data-ttu-id="2ba34-125">M 分類は、成熟した対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="2ba34-125">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="2ba34-126">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="2ba34-126">agesAbove13</span></span>|<span data-ttu-id="2ba34-127">5 </span><span class="sxs-lookup"><span data-stu-id="2ba34-127">5</span></span>|<span data-ttu-id="2ba34-128">R13 の分類は、13才以上に制限されます。</span><span class="sxs-lookup"><span data-stu-id="2ba34-128">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="2ba34-129">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="2ba34-129">agesAbove15</span></span>|<span data-ttu-id="2ba34-130">6 </span><span class="sxs-lookup"><span data-stu-id="2ba34-130">6</span></span>|<span data-ttu-id="2ba34-131">R15 の分類は、15年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="2ba34-131">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="2ba34-132">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="2ba34-132">agesAbove16</span></span>|<span data-ttu-id="2ba34-133">7 </span><span class="sxs-lookup"><span data-stu-id="2ba34-133">7</span></span>|<span data-ttu-id="2ba34-134">R16 の分類は、16年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="2ba34-134">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="2ba34-135">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="2ba34-135">agesAbove18</span></span>|<span data-ttu-id="2ba34-136">8 </span><span class="sxs-lookup"><span data-stu-id="2ba34-136">8</span></span>|<span data-ttu-id="2ba34-137">R18 の分類は、18年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="2ba34-137">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="2ba34-138">しか</span><span class="sxs-lookup"><span data-stu-id="2ba34-138">restricted</span></span>|<span data-ttu-id="2ba34-139">9 </span><span class="sxs-lookup"><span data-stu-id="2ba34-139">9</span></span>|<span data-ttu-id="2ba34-140">R 分類は特定の対象ユーザーに制限されています。</span><span class="sxs-lookup"><span data-stu-id="2ba34-140">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="2ba34-141">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="2ba34-141">agesAbove16Restricted</span></span>|<span data-ttu-id="2ba34-142">10  </span><span class="sxs-lookup"><span data-stu-id="2ba34-142">10</span></span>|<span data-ttu-id="2ba34-143">RP16 分類には、16以下の閲覧者が親または成人と共に必要</span><span class="sxs-lookup"><span data-stu-id="2ba34-143">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





