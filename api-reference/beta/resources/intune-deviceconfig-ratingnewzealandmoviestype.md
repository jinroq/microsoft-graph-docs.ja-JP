---
title: ratingNewZealandMoviesType 列挙型
description: ニュージーランドでの映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df996a3267cc31b80456b74ca6002d3a95467e79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368206"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="15692-103">ratingNewZealandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="15692-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="15692-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15692-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15692-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15692-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15692-106">ニュージーランドでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="15692-106">Movies rating labels in New Zealand</span></span>

## <a name="members"></a><span data-ttu-id="15692-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="15692-107">Members</span></span>
|<span data-ttu-id="15692-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="15692-108">Member</span></span>|<span data-ttu-id="15692-109">値</span><span class="sxs-lookup"><span data-stu-id="15692-109">Value</span></span>|<span data-ttu-id="15692-110">説明</span><span class="sxs-lookup"><span data-stu-id="15692-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15692-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="15692-111">allAllowed</span></span>|<span data-ttu-id="15692-112">.0</span><span class="sxs-lookup"><span data-stu-id="15692-112">0</span></span>|<span data-ttu-id="15692-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="15692-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="15692-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="15692-114">allBlocked</span></span>|<span data-ttu-id="15692-115">1-d</span><span class="sxs-lookup"><span data-stu-id="15692-115">1</span></span>|<span data-ttu-id="15692-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="15692-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="15692-117">元帳</span><span class="sxs-lookup"><span data-stu-id="15692-117">general</span></span>|<span data-ttu-id="15692-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="15692-118">2</span></span>|<span data-ttu-id="15692-119">一般的な対象ユーザーに適している</span><span class="sxs-lookup"><span data-stu-id="15692-119">Suitable for general audience</span></span>|
|<span data-ttu-id="15692-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="15692-120">parentalGuidance</span></span>|<span data-ttu-id="15692-121">1/3</span><span class="sxs-lookup"><span data-stu-id="15692-121">3</span></span>|<span data-ttu-id="15692-122">PG の分類では、保護者による指導を推奨</span><span class="sxs-lookup"><span data-stu-id="15692-122">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="15692-123">度</span><span class="sxs-lookup"><span data-stu-id="15692-123">mature</span></span>|<span data-ttu-id="15692-124">2/4</span><span class="sxs-lookup"><span data-stu-id="15692-124">4</span></span>|<span data-ttu-id="15692-125">M 分類は、成熟した対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="15692-125">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="15692-126">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="15692-126">agesAbove13</span></span>|<span data-ttu-id="15692-127">5</span><span class="sxs-lookup"><span data-stu-id="15692-127">5</span></span>|<span data-ttu-id="15692-128">R13 の分類は、13才以上に制限されます。</span><span class="sxs-lookup"><span data-stu-id="15692-128">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="15692-129">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="15692-129">agesAbove15</span></span>|<span data-ttu-id="15692-130">シックス</span><span class="sxs-lookup"><span data-stu-id="15692-130">6</span></span>|<span data-ttu-id="15692-131">R15 の分類は、15年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="15692-131">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="15692-132">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="15692-132">agesAbove16</span></span>|<span data-ttu-id="15692-133">7</span><span class="sxs-lookup"><span data-stu-id="15692-133">7</span></span>|<span data-ttu-id="15692-134">R16 の分類は、16年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="15692-134">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="15692-135">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="15692-135">agesAbove18</span></span>|<span data-ttu-id="15692-136">8 </span><span class="sxs-lookup"><span data-stu-id="15692-136">8</span></span>|<span data-ttu-id="15692-137">R18 の分類は、18年以上に制限されています。</span><span class="sxs-lookup"><span data-stu-id="15692-137">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="15692-138">しか</span><span class="sxs-lookup"><span data-stu-id="15692-138">restricted</span></span>|<span data-ttu-id="15692-139">9 </span><span class="sxs-lookup"><span data-stu-id="15692-139">9</span></span>|<span data-ttu-id="15692-140">R 分類は特定の対象ユーザーに制限されています。</span><span class="sxs-lookup"><span data-stu-id="15692-140">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="15692-141">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="15692-141">agesAbove16Restricted</span></span>|<span data-ttu-id="15692-142">10 </span><span class="sxs-lookup"><span data-stu-id="15692-142">10</span></span>|<span data-ttu-id="15692-143">RP16 分類には、16以下の閲覧者が親または成人と共に必要</span><span class="sxs-lookup"><span data-stu-id="15692-143">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|



