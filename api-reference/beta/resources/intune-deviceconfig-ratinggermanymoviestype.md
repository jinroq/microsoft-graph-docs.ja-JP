---
title: ratingGermanyMoviesType 列挙型
description: ドイツでの映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64aada06052f2cf65598a545b3965459e30e0d6f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950985"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="06f4b-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="06f4b-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="06f4b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06f4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06f4b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06f4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06f4b-106">ドイツでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="06f4b-106">Movies rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="06f4b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="06f4b-107">Members</span></span>
|<span data-ttu-id="06f4b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="06f4b-108">Member</span></span>|<span data-ttu-id="06f4b-109">値</span><span class="sxs-lookup"><span data-stu-id="06f4b-109">Value</span></span>|<span data-ttu-id="06f4b-110">説明</span><span class="sxs-lookup"><span data-stu-id="06f4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f4b-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="06f4b-111">allAllowed</span></span>|<span data-ttu-id="06f4b-112">.0</span><span class="sxs-lookup"><span data-stu-id="06f4b-112">0</span></span>|<span data-ttu-id="06f4b-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="06f4b-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="06f4b-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="06f4b-114">allBlocked</span></span>|<span data-ttu-id="06f4b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="06f4b-115">1</span></span>|<span data-ttu-id="06f4b-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="06f4b-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="06f4b-117">元帳</span><span class="sxs-lookup"><span data-stu-id="06f4b-117">general</span></span>|<span data-ttu-id="06f4b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="06f4b-118">2</span></span>|<span data-ttu-id="06f4b-119">Ab 0 Jahren、年齢制限なし</span><span class="sxs-lookup"><span data-stu-id="06f4b-119">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="06f4b-120">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="06f4b-120">agesAbove6</span></span>|<span data-ttu-id="06f4b-121">1/3</span><span class="sxs-lookup"><span data-stu-id="06f4b-121">3</span></span>|<span data-ttu-id="06f4b-122">Ab 6 Jahren、才を過ぎた</span><span class="sxs-lookup"><span data-stu-id="06f4b-122">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="06f4b-123">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="06f4b-123">agesAbove12</span></span>|<span data-ttu-id="06f4b-124">2/4</span><span class="sxs-lookup"><span data-stu-id="06f4b-124">4</span></span>|<span data-ttu-id="06f4b-125">Ab 12 Jahren、12才以上</span><span class="sxs-lookup"><span data-stu-id="06f4b-125">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="06f4b-126">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="06f4b-126">agesAbove16</span></span>|<span data-ttu-id="06f4b-127">5</span><span class="sxs-lookup"><span data-stu-id="06f4b-127">5</span></span>|<span data-ttu-id="06f4b-128">Ab 16 Jahren、16才以上</span><span class="sxs-lookup"><span data-stu-id="06f4b-128">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="06f4b-129">保護者</span><span class="sxs-lookup"><span data-stu-id="06f4b-129">adults</span></span>|<span data-ttu-id="06f4b-130">シックス</span><span class="sxs-lookup"><span data-stu-id="06f4b-130">6</span></span>|<span data-ttu-id="06f4b-131">Ab 18 Jahren、大人のみ</span><span class="sxs-lookup"><span data-stu-id="06f4b-131">Ab 18 Jahren, adults only</span></span>|




